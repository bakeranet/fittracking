# FitTrack — Tu plan de transformación 🏋️

PWA (Progressive Web App) para controlar tu pérdida de grasa: peso, entrenos, comidas y notas.

## Despliegue en GitHub Pages

### Opción 1: Desde la web de GitHub (sin terminal)

1. Ve a [github.com/new](https://github.com/new) y crea un repositorio (ej: `fittrack`)
2. Sube todos los archivos de esta carpeta arrastrándolos
3. Ve a **Settings → Pages → Source** y selecciona `main` (o `master`) branch
4. Tu app estará en: `https://tu-usuario.github.io/fittrack/`

### Opción 2: Desde terminal

```bash
cd fitness-pwa
git init
git add .
git commit -m "FitTrack PWA"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/fittrack.git
git push -u origin main
```

Luego activa GitHub Pages en Settings → Pages → Source: `main`.

## Instalar como app

Una vez desplegada, abre la URL en tu móvil:

- **iOS**: Safari → botón compartir → "Añadir a pantalla de inicio"
- **Android**: Chrome → menú ⋮ → "Instalar aplicación" o "Añadir a pantalla de inicio"

## Estructura

```
fitness-pwa/
├── index.html       ← App completa (HTML + CSS + JS)
├── manifest.json    ← Configuración PWA
├── sw.js            ← Service Worker (funciona offline)
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

## Características

- **Dashboard**: peso actual, progreso, gráfica de evolución, entrenos de la semana
- **Peso**: registro diario con historial
- **Comidas**: checklist de 6 comidas por día con adherencia semanal
- **Notas**: diario libre para apuntar cómo te sientes
- **Offline**: funciona sin conexión tras la primera visita
- **Instalable**: se puede añadir a la pantalla de inicio como app nativa
- **Datos locales**: todo se guarda en localStorage, privado en tu dispositivo
