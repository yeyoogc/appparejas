# App de Parejas 💕

App de pareja completa — comparte momentos, recuerdos y sentimientos con tu persona favorita.

## Stack técnico

- **Frontend:** React 18 + Vite + React Router
- **Backend:** Firebase (Auth, Realtime Database, Cloud Functions, Hosting)
- **PWA:** vite-plugin-pwa (installable, offline-capable)
- **UI:** CSS Modules + Glassmorphism design system
- **Animaciones:** Framer Motion
- **Iconos:** Lucide React
- **Fechas:** date-fns

## Características

- 🔐 Autenticación (registro, login)
- 💑 Sistema de parejas con códigos de invitación
- 📅 Contador de días juntos
- ❤️ Razones por las que te quiero (CRUD + aleatorio)
- ⭐ Recuerdos compartidos
- 🗺️ Planes y metas juntos
- 🎵 Canciones con enlaces a streaming
- 💭 Sentimientos en tiempo real
- 🎬 Lista de películas con selector aleatorio
- 📡 Estado en vivo
- 💌 Notas de amor
- 🔔 Notificaciones push (FCM)

## Primeros pasos

```bash
# 1. Instalar dependencias
npm install
cd functions && npm install && cd ..

# 2. Configurar variables de entorno
cp .env.example .env.local
# Rellena las variables con tu configuración de Firebase

# 3. Desarrollo local
npm run dev

# 4. Deploy
npm run deploy
```

## Estructura del proyecto

```
src/
├── main.jsx              # Entry point
├── App.jsx               # Router + guards
├── lib/
│   └── firebase.js       # Firebase config
├── contexts/
│   ├── AuthContext.jsx    # Autenticación
│   └── CoupleContext.jsx  # Gestión de pareja
├── layouts/
│   └── AppLayout.jsx     # Layout con bottom nav
├── components/
│   └── BottomNav.jsx     # Navegación inferior
├── pages/
│   ├── auth/             # Login, Register, Join
│   ├── HomePage.jsx      # Dashboard principal
│   ├── ReasonsPage.jsx   # Razones
│   ├── MemoriesPage.jsx  # Recuerdos
│   ├── PlansPage.jsx     # Planes
│   ├── SongsPage.jsx     # Canciones
│   ├── FeelingsPage.jsx  # Sentimientos
│   ├── MoviesPage.jsx    # Películas
│   ├── StatusPage.jsx    # Estado en vivo
│   ├── NotesPage.jsx     # Notas de amor
│   └── SettingsPage.jsx  # Ajustes
└── styles/
    └── globals.css       # Design system
functions/
└── index.js              # Cloud Functions (push notifications)
```
