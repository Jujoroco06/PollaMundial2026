# ⚽ Polla Mundial 2026

Una aplicación web completamente funcional para predicciones de partidos del Mundial de Fútbol 2026, deployable en GitHub Pages sin necesidad de backend.

## 🎯 Características

- ✅ **Autenticación segura** con contraseñas hasheadas
- ✅ **Predicciones en tiempo real** antes de cada partido
- ✅ **Deadlines automáticos** que cierran partidos
- ✅ **Scoring automático**: +5 exacto, +3 resultado correcto
- ✅ **Leaderboard en vivo** con rankings actualizados
- ✅ **Panel de administración** para gestionar partidos
- ✅ **Almacenamiento local** (localStorage) — sin servidor necesario
- ✅ **Diseño responsivo** para móvil, tablet y desktop

## 🚀 Despliegue Rápido

### En GitHub Pages (Recomendado)

```bash
# 1. Crea un repositorio en GitHub
# 2. Sube index.html a la rama main
# 3. Ve a Settings → Pages → Deploy from branch (main)
# 4. Tu app estará en: https://tu-usuario.github.io/mundial2026/
```

**Tiempo total**: 5 minutos

### Localmente (Desarrollo)

```bash
# Solo abre index.html en tu navegador
open index.html
```

## 📖 Guía Rápida

### Para Administradores

1. **Registrate** (el primer usuario es admin automáticamente)
2. Ve a **⚙️ Administrar**
3. Agrega partidos con equipos, fechas y horas
4. Establece deadlines para cada partido
5. Registra resultados cuando terminen los partidos
6. Los puntos se calculan automáticamente

### Para Usuarios

1. **Registrate** con tu nombre de usuario
2. Ve a **⚽ Todos los Partidos**
3. Ingresa tus predicciones antes del deadline
4. Ve tu puntuación en **🏆 Clasificación**

## 📊 Sistema de Puntuación

| Resultado | Puntos |
|-----------|--------|
| Marcador exacto | **+5** |
| Resultado correcto (G/E/P) | **+3** |
| Incorrecto | **0** |

## 🔐 Seguridad

- Contraseñas hasheadas con SHA-256
- Datos almacenados localmente (no se envían a servidores)
- Cada navegador tiene sus propios datos
- Acceso basado en roles (admin/usuario)

## 📱 Compatibilidad

- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Navegadores móviles

## 📂 Estructura

```
mundial2026/
├── index.html           # Aplicación completa (HTML + CSS + JS)
├── DEPLOYMENT_GUIDE.md  # Guía detallada de despliegue
└── README.md            # Este archivo
```

## ⚙️ Configuración

### Cambiar Sistema de Puntuación

Abre `index.html` y busca:

```javascript
const SCORING = {
  EXACT: 5,              // Puntos por marcador exacto
  CORRECT_OUTCOME: 3     // Puntos por resultado correcto
};
```

Modifica los números según necesites.

## 🐛 Troubleshooting

**"No puedo acceder a la aplicación"**
- Verifica que GitHub Pages esté habilitado
- Espera 2-3 minutos después de activarlo

**"Se me olvidó la contraseña"**
- Abre la consola (F12) y ejecuta: `localStorage.clear()`
- Recarga y regístrate de nuevo

**"Los datos desaparecieron"**
- Probablemente limpiaste el caché del navegador
- Los datos están en localStorage y se pierden si limpias el caché


## 📝 Ejemplo de Uso

1. **Admin** se registra → automáticamente es admin
2. **Admin** agrega partidos: Colombia vs Argentina (12 jun, 18:00)
3. **Admin** establece deadline: 12 jun, 17:00
4. **Familia** se registra
5. **Familia** predice: Colombia 2 - Argentina 1
6. Termina el partido: resultado real 2 - 1
7. **Sistema** otorga +5 puntos (exacto)
8. **Familia** ve su puntuación en la clasificación

## 🎮 Características Avanzadas

### Countdown en Tiempo Real

Cada partido muestra un countdown que se actualiza cada segundo hasta el deadline.

### Bloqueo Automático

Después del deadline, el partido se bloquea automáticamente. Nadie puede hacer nuevas predicciones.

### Historial de Predicciones

En "Mis Predicciones" ves todas tus predicciones anteriores con los resultados y puntos ganados.

### Leaderboard Dinámico

La clasificación se actualiza en tiempo real cuando se registran resultados.

## 🌍 Despliegue Global

Esta aplicación funciona en cualquier lugar con internet:

- **GitHub Pages** (recomendado, gratuito)
- **Netlify** (gratuito)
- **Vercel** (gratuito)
- **Cualquier servidor web estático**

## 📄 Licencia

Uso libre para propósitos personales y familiares.

## 🙋 Preguntas Frecuentes

**¿Necesito un servidor?**
No, funciona 100% en el navegador con localStorage.

**¿Los datos se sincronizan entre dispositivos?**
No, cada navegador tiene sus propios datos. Para compartir, todos deben usar el mismo dispositivo.

**¿Puedo modificar la aplicación?**
Sí, es código abierto. Modifica `index.html` como necesites.

**¿Qué pasa si pierdo mis datos?**
Los datos están en localStorage. Si limpias el caché, se pierden. Haz backup regularmente.

---

**¿Necesitas ayuda?** Ver [DEPLOYMENT_GUIDE.md](./DEPLOYMENT_GUIDE.md) para la guía completa.

¡Que disfrutes la Polla Mundial 2026! ⚽🏆
