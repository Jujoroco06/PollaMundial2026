# ⚽ Polla Familiar — Mundial 2026
## Arquitectura Completa + Guía de Despliegue

---

## 📐 Arquitectura del Sistema

```
┌─────────────────────────────────────────────────────────────────┐
│                     GITHUB PAGES (Frontend)                     │
│                                                                 │
│  index.html  ◄──── Todo en un solo archivo HTML/CSS/JS         │
│    ├─ AuthModule       (registro, login, sesión JWT)            │
│    ├─ LeaderboardModule (clasificación en tiempo real)          │
│    ├─ MatchesModule    (listado de partidos + predicciones)     │
│    ├─ PredictionsModule (formulario de predicciones)            │
│    └─ AdminModule      (panel exclusivo de administrador)       │
│                                                                 │
│  Persistencia:  localStorage  (modo standalone sin backend)    │
│  Seguridad:     SHA-256 + salt para contraseñas                │
└──────────────────────────┬──────────────────────────────────────┘
                           │ HTTP REST (JWT Bearer token)
                           │ (cuando se conecta al backend Java)
┌──────────────────────────▼──────────────────────────────────────┐
│               BACKEND Java / Spring Boot 3.2                    │
│                                                                 │
│  AuthController    → POST /api/auth/register                   │
│                    → POST /api/auth/login                      │
│                                                                 │
│  MatchController   → GET  /api/matches              (público)  │
│                    → POST /api/matches              (admin)    │
│                    → PUT  /api/matches/{id}/result  (admin)    │
│                                                                 │
│  PredictionController → GET  /api/predictions/mine             │
│                       → PUT  /api/predictions/{matchId}        │
│                                                                 │
│  LeaderboardController → GET /api/leaderboard       (público)  │
│                                                                 │
│  ScoreService  ←─ lógica centralizada de puntuación            │
│    ├─ Resultado exacto:    +5 puntos                           │
│    └─ Resultado correcto:  +3 puntos                           │
└──────────────────────────┬──────────────────────────────────────┘
                           │ JPA / Hibernate
┌──────────────────────────▼──────────────────────────────────────┐
│           BASE DE DATOS (H2 dev / PostgreSQL prod)              │
│                                                                 │
│  users       │ id, name, username, password_hash, is_admin     │
│  matches     │ id, home_team, away_team, datetime, stage,      │
│              │ status, score_home, score_away                  │
│  predictions │ id, match_id, user_id, pred_home, pred_away,   │
│              │ points_awarded, exact, scored                   │
│  score_entries│ id, user_id, match_id, points, reason         │
└─────────────────────────────────────────────────────────────────┘
```

---

## 🎯 Sistema de Puntuación

| Resultado | Puntos |
|-----------|--------|
| Acierta el resultado (G/E/P) | **+3 pts** |
| Marcador exacto | **+5 pts** |
| Resultado incorrecto | 0 pts |

**Ejemplo:**
- Partido real: Colombia 2 – 1 Argentina
- Usuario A predice: 2 – 1 → **+5 pts** (exacto)
- Usuario B predice: 1 – 0 → **+3 pts** (acertó victoria Colombia)
- Usuario C predice: 0 – 2 → **0 pts** (falló)

---

## 🚀 Modo 1: Solo GitHub Pages (sin backend)

La aplicación **funciona completamente sin backend**. Usa `localStorage` del navegador.

### Pasos:
```bash
# 1. Fork o crea un repositorio en GitHub
# 2. Sube index.html al repositorio
# 3. Ve a Settings → Pages → Source: Deploy from branch → main
# 4. ¡Listo! Tu app estará en: https://tu-usuario.github.io/tu-repo/
```

### Limitaciones del modo standalone:
- Los datos están en el navegador de cada usuario (no se comparten entre dispositivos)
- **Solución:** El administrador gestiona todo desde su dispositivo; comparte la URL con todos

---

## 🖥️ Modo 2: Con Backend Java (Recomendado para producción)

### Requisitos
- Java 21+
- Maven 3.9+
- PostgreSQL (o cualquier BD SQL)

### Configuración (`application.properties`):
```properties
# Server
server.port=8080

# Database (PostgreSQL en producción)
spring.datasource.url=jdbc:postgresql://localhost:5432/mundial2026
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=false

# JWT — CAMBIA ESTE SECRET EN PRODUCCIÓN
jwt.secret=cambia_esto_por_una_clave_segura_de_al_menos_32_chars
jwt.expiration-ms=86400000

# CORS — ajusta al dominio de GitHub Pages
app.cors.allowed-origins=https://tu-usuario.github.io
```

### Despliegue del Backend:
```bash
# Construir
mvn clean package -DskipTests

# Ejecutar
java -jar target/mundial2026-api-1.0.0.jar

# O con Docker:
docker build -t mundial2026-api .
docker run -p 8080:8080 mundial2026-api
```

### Conectar el Frontend al Backend:
Agrega esta variable al inicio del `<script>` en `index.html`:
```javascript
const API_URL = 'https://tu-backend.railway.app/api'; // o tu dominio
```

**Opciones de hosting gratuito para el backend:**
- **Railway.app** — gratis hasta cierto límite, muy fácil con Spring Boot
- **Render.com** — plan gratuito disponible
- **Fly.io** — generoso nivel gratuito
- **Oracle Cloud Free Tier** — VM gratuita permanente

---

## 🔒 Seguridad implementada

### Frontend (standalone):
- Contraseñas hasheadas con **SHA-256 + salt** antes de guardar en localStorage
- Nunca se almacena la contraseña en texto plano
- Validación de roles en cada acción

### Backend Java:
- Contraseñas con **BCrypt** (12 rounds) — estándar de la industria
- **JWT stateless** — sin sesiones en servidor
- **Spring Security** con roles ADMIN / USER
- `@PreAuthorize("hasRole('ADMIN')")` en endpoints sensibles
- Validación con Bean Validation (`@NotBlank`, `@Min`, `@Pattern`)
- CORS configurado por dominio
- Audit trail de todas las transacciones de puntos

---

## 📊 Estructura de Datos (localStorage)

```json
// mw26_users
[{
  "id": "1748000000000",
  "name": "Juanito Pérez",
  "username": "juanito",
  "passwordHash": "sha256_hash_here",
  "isAdmin": true,
  "createdAt": "2026-05-16T10:00:00Z"
}]

// mw26_matches
[{
  "id": "1748000001000",
  "home": "Colombia",
  "away": "Ecuador",
  "date": "2026-06-12",
  "time": "18:00",
  "stage": "Grupos",
  "group": "C",
  "status": "finished",
  "scoreHome": 2,
  "scoreAway": 1
}]

// mw26_predictions
{
  "1748000001000": {
    "juanito": { "home": 2, "away": 1, "points": 5, "exact": true },
    "maria":   { "home": 1, "away": 0, "points": 3, "exact": false }
  }
}

// mw26_scores
{ "juanito": 47, "maria": 31, "carlos": 28 }
```

---

## 🏗️ Cómo usar la aplicación

### Para el Administrador:
1. Regístrate primero (el primer usuario registrado es admin automáticamente)
2. Ve a **⚙️ Administrar** → Agrega los partidos del Mundial
3. Comparte la URL con la familia
4. Cuando termine cada partido → Registrar Resultado → ¡Los puntos se calculan solos!

### Para los Participantes:
1. Regístrate con nombre y usuario
2. Ve a **📋 Mis predicciones** antes de cada partido
3. Introduce el marcador que predices y guarda
4. Sigue la **🏆 Clasificación** en tiempo real

---

## 📅 Partidos del Mundial 2026

El torneo se jugará en **Estados Unidos, México y Canadá** con **48 selecciones**.
Fases: Grupos (108 partidos) → Octavos → Cuartos → Semis → Final.

El administrador carga los partidos manualmente desde el panel de administración.

---

## 🔧 Personalización

- **Cambiar puntuación:** Edita las constantes en `ScoreService.java`:
  ```java
  public static final int POINTS_EXACT_SCORE    = 5;
  public static final int POINTS_CORRECT_OUTCOME = 3;
  ```
  O en el frontend (función `registerResult()`): `pts = 5` y `pts = 3`.

- **Agregar más roles:** Extiende el enum y la lógica en `SecurityConfig.java`.

- **Predicción del ganador del torneo:** Agrega un campo extra al modelo `User`.
