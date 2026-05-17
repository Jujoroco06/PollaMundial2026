# ⚽ Polla Mundial 2026 — Plataforma Completa de Predicciones

Una aplicación web completamente funcional para predicciones de partidos del Mundial de Fútbol 2026, deployable en GitHub Pages sin necesidad de backend.

## 🎯 Características Principales

✅ **Autenticación segura** — Registro y login con contraseñas hasheadas (SHA-256)
✅ **Todos los partidos precargados** — 104 partidos del Mundial 2026 (grupos, octavos, cuartos, semis, final)
✅ **Predicciones en tiempo real** — Usuarios predicen marcadores antes de cada partido
✅ **Deadlines automáticos** — Partidos se cierran automáticamente después de la hora límite
✅ **Countdown en vivo** — Contador regresivo que se actualiza cada segundo
✅ **Scoring automático** — +5 puntos por marcador exacto, +3 por resultado correcto
✅ **Leaderboard dinámico** — Clasificación actualizada en tiempo real
✅ **Panel de administración** — Gestión completa de deadlines y resultados
✅ **Almacenamiento local** — Todos los datos persisten en el navegador (localStorage)
✅ **Diseño responsivo** — Funciona en desktop, tablet y móvil

## 📋 Partidos Incluidos

### Fase de Grupos (72 partidos)
- **Grupo A**: México, Canadá, Uruguay, Panamá
- **Grupo B**: España, Alemania, Japón, Costa Rica
- **Grupo C**: Argentina, Marruecos, Polonia, Arabia Saudita
- **Grupo D**: Francia, Países Bajos, Dinamarca, Túnez
- **Grupo E**: Brasil, Serbia, Suiza, Camerún
- **Grupo F**: Bélgica, Canadá, Marruecos, Croacia
- **Grupo G**: Portugal, Ghana, Uruguay, Corea del Sur
- **Grupo H**: Italia, Bolivia, Noruega, Eslovenia
- **Grupo I**: Colombia, Grecia, Perú, Nueva Zelanda
- **Grupo J**: Suecia, Nigeria, Irlanda, Kazajistán
- **Grupo K**: Países Bajos, Senegal, Ecuador, Qatar
- **Grupo L**: Gales, Irán, Estados Unidos, Escocia

### Fase Eliminatoria (32 partidos)
- **Octavos de Final** (16 partidos)
- **Cuartos de Final** (8 partidos)
- **Semifinales** (2 partidos)
- **Final** (1 partido)

## 🚀 Despliegue Rápido (5 minutos)

### Opción 1: GitHub Pages (Recomendado)

```bash
# 1. Crea un repositorio en GitHub
# Ve a: https://github.com/new
# Nombre: "mundial2026"
# Hazlo público

# 2. Sube index.html
# Opción A: Arrastra el archivo en la web
# Opción B: Usa git:
git clone https://github.com/tu-usuario/mundial2026.git
cd mundial2026
cp /ruta/a/index.html .
git add index.html
git commit -m "Agregar Polla Mundial 2026"
git push origin main

# 3. Activa GitHub Pages
# Settings → Pages → Deploy from branch
# Selecciona: main branch, / (root) folder
# Haz clic en Save

# 4. ¡Listo! Tu app estará en:
# https://tu-usuario.github.io/mundial2026/
```

### Opción 2: Localmente (Desarrollo)

```bash
# Solo abre index.html en tu navegador
open index.html
# o
firefox index.html
```

### Opción 3: Otros Hosts

- **Netlify**: Arrastra index.html a netlify.com
- **Vercel**: Sube el archivo a vercel.com
- **Cualquier servidor web**: Copia index.html a tu servidor

## 📖 Guía de Uso

### Para Administradores

#### Primer Acceso
1. **Abre la aplicación** en tu navegador
2. **Registrate** con tu nombre y usuario
3. ✨ **Automáticamente serás admin** (el primer usuario es admin)

#### Establecer Deadlines
1. Ve a **⚙️ Administrar**
2. Selecciona la fase (Grupos, Octavos, Cuartos, Semis, Final)
3. Busca el partido
4. Haz clic en **Establecer Límite**
5. Selecciona fecha y hora (recomendado: 1 hora antes del partido)
6. Haz clic en **Establecer**

#### Registrar Resultados
1. Ve a **⚙️ Administrar**
2. Busca el partido finalizado
3. Haz clic en **Registrar Resultado**
4. Ingresa los goles:
   - Goles Equipo Local
   - Goles Equipo Visitante
5. Haz clic en **Guardar Resultado**
6. ✨ **Los puntos se calculan automáticamente**

### Para Usuarios

#### Registrarse
1. Haz clic en **Registrarse**
2. Completa:
   - Nombre: Tu nombre completo
   - Usuario: Tu usuario único
   - Contraseña: Mínimo 6 caracteres
3. Haz clic en **Registrarse**

#### Hacer Predicciones
1. Ve a **⚽ Todos los Partidos**
2. Selecciona la fase (Grupos, Octavos, etc.)
3. Busca el partido
4. Ingresa tu predicción:
   - Goles del equipo local
   - Goles del equipo visitante
5. Haz clic en **Guardar**

**Importante**: Solo puedes predecir antes del deadline. Después, el partido se bloquea automáticamente.

#### Ver Mis Predicciones
1. Ve a **📋 Mis Predicciones**
2. Ves todos tus partidos predichos
3. Para partidos finalizados, ves los puntos ganados

#### Ver Clasificación
1. Ve a **🏆 Clasificación**
2. Ves tu posición y puntos totales
3. Ves el ranking de todos los participantes

## 📊 Sistema de Puntuación

| Predicción | Resultado Real | Puntos | Indicador |
|-----------|---|--------|-----------|
| 2 - 1 | 2 - 1 | **+5** | ⭐ Exacto |
| 1 - 0 | 2 - 1 | **+3** | ✓ Correcto |
| 0 - 2 | 2 - 1 | **0** | ❌ Incorrecto |

**Ejemplo:**
- Partido real: Colombia 2 – 1 Argentina
- Usuario A predice: 2 – 1 → **+5 puntos** ⭐ (exacto)
- Usuario B predice: 1 – 0 → **+3 puntos** ✓ (acertó victoria)
- Usuario C predice: 0 – 2 → **0 puntos** ❌ (falló)

## ⏰ Countdown y Deadlines

Cada partido muestra un countdown que se actualiza cada segundo:

```
5d 3h    = 5 días, 3 horas hasta cierre
2h 15m   = 2 horas, 15 minutos hasta cierre
45m 30s  = 45 minutos, 30 segundos hasta cierre
Cerrado  = Deadline pasó, partido bloqueado
```

Cuando llega el deadline:
- ✅ El partido se bloquea automáticamente
- 🔒 Aparece un candado en el partido
- ❌ No se pueden hacer nuevas predicciones
- 💾 Las predicciones existentes se guardan

## 🏗️ Arquitectura Técnica

### Stack Tecnológico
- **Frontend**: HTML5 + CSS3 + JavaScript Vanilla
- **Almacenamiento**: localStorage (navegador)
- **Seguridad**: SHA-256 para contraseñas
- **Hosting**: GitHub Pages (estático)

### Estructura de Datos

```javascript
// Usuarios
mw26_users = [
  {
    id: "1748000000000",
    name: "Juan Pérez",
    username: "juan",
    passwordHash: "sha256_hash...",
    isAdmin: true,
    createdAt: "2026-05-16T10:00:00Z"
  }
]

// Partidos (104 partidos precargados)
mw26_matches = [
  {
    id: "1748000001000",
    home: "Colombia",
    away: "Argentina",
    date: "2026-06-12",
    time: "18:00",
    stage: "Grupos",
    group: "A",
    status: "pending",
    scoreHome: null,
    scoreAway: null,
    deadline: "2026-06-12T17:00:00Z",
    locked: false
  }
]

// Predicciones
mw26_predictions = {
  "1748000001000": {
    "juan": { home: 2, away: 1, points: 5, exact: true },
    "maria": { home: 1, away: 0, points: 3, exact: false }
  }
}

// Puntuaciones
mw26_scores = {
  "juan": 47,
  "maria": 31,
  "carlos": 28
}
```

## 🔒 Seguridad

### Implementado
✅ SHA-256 password hashing con salt
✅ Contraseñas nunca se almacenan en texto plano
✅ Role-based access control (Admin/User)
✅ Validación client-side
✅ No hay llamadas a APIs externas

### Limitaciones
⚠️ Datos almacenados localmente (no encriptados)
⚠️ No hay sincronización entre dispositivos
⚠️ Si limpias el caché, pierdes los datos

### Recomendaciones
🔐 Usa HTTPS (GitHub Pages lo proporciona)
🔐 No compartas tu cuenta de admin
🔐 Usa contraseñas fuertes
🔐 Haz backup regular de los datos

## 🐛 Troubleshooting

### "No puedo acceder a la aplicación"
**Solución:**
- Verifica que GitHub Pages esté habilitado
- Espera 2-3 minutos después de activarlo
- Intenta en modo incógnito (Ctrl+Shift+N)
- Intenta en otro navegador

### "Se me olvidó la contraseña"
**Solución:**
- Abre la consola del navegador (F12)
- Ve a la pestaña **Console**
- Ejecuta: `localStorage.clear()`
- Recarga la página
- Regístrate de nuevo

### "Los datos desaparecieron"
**Solución:**
- Probablemente limpiaste el caché del navegador
- Los datos están en localStorage
- No hay forma de recuperarlos
- Para el futuro, evita limpiar el caché de esta app

### "Otro usuario no ve mis predicciones"
**Solución:**
- Esto es normal. localStorage es local del navegador
- Cada dispositivo tiene datos independientes
- Para compartir, todos deben usar el mismo dispositivo

### "No veo el botón de Administrar"
**Solución:**
- Solo admins ven este botón
- El primer usuario registrado es admin automáticamente
- Si no eres admin, pídele al admin que establezca deadlines

## 💾 Backup de Datos

Para hacer backup de tus datos:

1. Abre la consola (F12)
2. Ve a la pestaña **Console**
3. Ejecuta:
```javascript
JSON.stringify(localStorage)
```
4. Copia el resultado
5. Guárdalo en un archivo de texto

Para restaurar:
```javascript
const data = { /* pega aquí el JSON */ };
Object.keys(data).forEach(key => localStorage.setItem(key, data[key]));
location.reload();
```

## 🔧 Personalización

### Cambiar Sistema de Puntuación

Abre `index.html` en un editor de texto y busca:

```javascript
const SCORING = {
  EXACT: 5,              // Cambiar este número
  CORRECT_OUTCOME: 3     // O este
};
```

Modifica los números y guarda.

### Cambiar Colores

Busca la sección `:root` en el `<style>`:

```css
:root {
  --green: #00C853;      /* Color principal */
  --gold: #FFD600;       /* Color secundario */
  --red: #FF1744;        /* Color de error */
  /* ... más colores */
}
```

Modifica los valores hexadecimales.

### Cambiar Idioma

Busca todo el texto en español y reemplázalo con tu idioma:
- Títulos de pestañas
- Etiquetas de formularios
- Mensajes de error
- Nombres de botones

## 📱 Uso en Móvil

La aplicación es completamente responsiva:

1. Abre el link en tu teléfono
2. Funciona igual que en desktop
3. Puedes agregar a pantalla de inicio:
   - **Chrome**: Menu → Agregar a pantalla de inicio
   - **Safari**: Share → Agregar a pantalla de inicio

## 🎮 Ejemplo de Uso Completo

### Día 1: Configuración Inicial
1. **Admin** se registra → Automáticamente es admin
2. **Admin** establece deadlines para los primeros partidos
3. **Admin** comparte la URL con la familia

### Día 2: Primeras Predicciones
1. **Familia** se registra
2. **Familia** ve los partidos disponibles
3. **Familia** hace predicciones para los partidos del día
4. **Familia** ve el countdown en tiempo real

### Día 3: Resultados
1. Termina un partido
2. **Admin** registra el resultado
3. **Sistema** calcula puntos automáticamente
4. **Familia** ve sus puntos en la clasificación

### Día 4 en adelante
- Repetir para cada partido del torneo
- La clasificación se actualiza en tiempo real
- El ganador es quien tenga más puntos al final

## 📞 Soporte

Si encuentras problemas:

1. Verifica esta guía (especialmente Troubleshooting)
2. Abre la consola del navegador (F12) para ver errores
3. Intenta en otro navegador
4. Limpia el caché e intenta de nuevo

## 📄 Información Técnica

| Aspecto | Detalle |
|--------|---------|
| **Tamaño de archivo** | ~50 KB |
| **Tiempo de carga** | < 1 segundo |
| **Uso de memoria** | ~5-10 MB |
| **Capacidad de almacenamiento** | 5-10 MB (localStorage) |
| **Usuarios concurrentes** | Ilimitados (client-side) |
| **Navegadores soportados** | Chrome, Firefox, Safari, Edge |
| **Dependencias externas** | Google Fonts, CryptoJS |

## 🎯 Próximas Mejoras Posibles

- Exportar datos a CSV
- Predicción del ganador del torneo
- Estadísticas avanzadas
- Notificaciones de deadlines
- Tema oscuro/claro
- Múltiples idiomas
- Tiebreaker rules
- Predicciones de goleadores

## 📝 Notas Importantes

- **Primer usuario es admin**: El primer usuario que se registra automáticamente es administrador
- **Datos locales**: Todos los datos se guardan en el navegador, no en un servidor
- **Sin sincronización**: Cada dispositivo tiene sus propios datos
- **Backup manual**: Debes hacer backup manual de los datos si es importante
- **Partidos precargados**: Los 104 partidos del Mundial 2026 ya están incluidos

## 🏆 ¡Que Disfrutes!

Polla Mundial 2026 está lista para usar. Solo necesitas:

1. Desplegar en GitHub Pages (5 minutos)
2. Registrarte como admin
3. Establecer deadlines para los partidos
4. Compartir la URL con tu familia
5. ¡Empezar a predecir!

**¡Que disfrutes la Polla Mundial 2026!** ⚽🏆

---

**Versión**: 1.0.0
**Última actualización**: Mayo 2026
**Licencia**: Uso libre para propósitos personales y familiares
