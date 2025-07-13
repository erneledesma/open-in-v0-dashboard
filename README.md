# Open-in-v0 Dashboard

Dashboard moderno construido con Next.js 15, Tailwind CSS, shadcn/ui y Recharts.

## Descripción

Este proyecto es un dashboard interactivo y responsivo que incluye:
- Sidebar de navegación
- Header con toggle de modo claro/oscuro
- Tarjetas de resumen
- Gráfica de visitantes interactiva
- Tabla de datos editable y drag & drop
- Soporte completo para dark mode siguiendo el diseño de [shadcn/ui](https://ui.shadcn.com/themes)

## Tecnologías principales
- [Next.js 15](https://nextjs.org/)
- [React 19](https://react.dev/)
- [Tailwind CSS 3](https://tailwindcss.com/)
- [shadcn/ui](https://ui.shadcn.com/)
- [Recharts](https://recharts.org/)
- [next-themes](https://github.com/pacocoursey/next-themes) (soporte dark mode)
- [@dnd-kit](https://dndkit.com/) (drag & drop en tabla)

## Instalación

1. Clona el repositorio:
   ```sh
git clone <repo-url>
cd open-in-v0
```
2. Instala las dependencias:
   ```sh
yarn install
# o npm install
```
3. Inicia el servidor de desarrollo:
   ```sh
yarn dev
# o npm run dev
```
4. Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

## Scripts disponibles
- `yarn dev` — Inicia el servidor de desarrollo
- `yarn build` — Compila la app para producción
- `yarn start` — Inicia la app en modo producción
- `yarn lint` — Linting del código

## Estructura del proyecto

```
open-in-v0/
├── app/
│   ├── dashboard/
│   │   ├── data.json         # Datos de ejemplo para la tabla
│   │   └── page.tsx         # Página principal del dashboard
│   ├── globals.css          # Estilos globales y variables CSS
│   └── layout.tsx           # Layout global con ThemeProvider
├── components/
│   ├── app-sidebar.tsx      # Sidebar de navegación
│   ├── chart-area-interactive.tsx # Gráfica interactiva
│   ├── data-table.tsx       # Tabla de datos con drag & drop
│   ├── section-cards.tsx    # Tarjetas de resumen
│   ├── site-header.tsx      # Header con toggle dark mode
│   └── ui/                  # Componentes UI reutilizables (shadcn/ui)
├── hooks/                   # Custom hooks
├── lib/                     # Utilidades
├── public/                  # Imágenes y assets
├── styles/                  # Estilos adicionales
├── tailwind.config.ts       # Configuración de Tailwind
├── package.json             # Dependencias y scripts
└── README.md                # (Este archivo)
```

## Características principales

### 1. Sidebar de navegación
- Acceso rápido a secciones principales, documentos y usuario.
- Íconos de [lucide-react](https://lucide.dev/).

### 2. Header con toggle de dark mode
- Cambia entre modo claro y oscuro con un solo clic.
- Persistencia automática según preferencia del sistema.

### 3. Tarjetas de resumen
- Muestran métricas clave como ingresos, clientes, cuentas activas y crecimiento.

### 4. Gráfica interactiva
- Visualización de visitantes por día (desktop y mobile).
- Filtros de rango de tiempo (últimos 7, 30, 90 días).
- Colores adaptados a dark/light mode.

### 5. Tabla de datos editable
- Visualiza y edita datos de secciones/documentos.
- Drag & drop para reordenar filas.
- Selección múltiple y acciones rápidas.

### 6. Soporte completo para dark mode
- Basado en variables CSS y clases de Tailwind.
- Toggle en el header usando [next-themes](https://github.com/pacocoursey/next-themes).
- Totalmente personalizable desde `app/globals.css` y `tailwind.config.ts`.

## Ejemplo de datos (tabla)

```json
[
  {
    "id": 1,
    "header": "Cover page",
    "type": "Cover page",
    "status": "In Process",
    "target": "18",
    "limit": "5",
    "reviewer": "Eddie Lake"
  },
  ...
]
```

## Personalización
- Puedes modificar los colores y variables en `app/globals.css`.
- Agrega o edita componentes en la carpeta `components/`.
- Cambia la estructura de navegación en `components/app-sidebar.tsx`.

## Créditos
- UI inspirada y basada en [shadcn/ui](https://ui.shadcn.com/themes)
- Gráficos por [Recharts](https://recharts.org/)
- Drag & drop por [dnd-kit](https://dndkit.com/)

---

¡Listo para usar y personalizar! 🚀 