# Intelligent Design System

Sistema de diseño inteligente integrado con Figma usando Code Connect.

## 📦 Estructura del Monorepo

Este repositorio está organizado como un monorepo usando **npm workspaces**:

```
inteligent-ds/
├── packages/
│   └── design-system/          # Sistema de diseño principal
│       ├── src/                # Componentes React
│       ├── scripts/            # Scripts de sincronización con Figma
│       ├── .storybook/         # Configuración de Storybook
│       └── figma.config.json   # Configuración de Code Connect
├── .github/
│   └── workflows/              # CI/CD workflows
├── package.json                # Configuración del workspace raíz
└── README.md                   # Este archivo
```

## 🚀 Inicio Rápido

### Instalación

```bash
# Instalar todas las dependencias del monorepo
npm install
```

### Comandos Principales

Desde la raíz del repositorio puedes ejecutar:

```bash
# Desarrollo
npm run dev                     # Iniciar Vite dev server
npm run storybook              # Iniciar Storybook

# Build
npm run build                  # Build app + Storybook

# Calidad de código
npm run lint                   # Ejecutar ESLint

# Sincronización con Figma
npm run tokens:rest            # Sincronizar tokens desde Figma REST API
npm run icons:rest             # Sincronizar iconos desde Figma REST API
npm run tokens                 # Sincronizar tokens (sin REST API)
npm run icons                  # Sincronizar iconos (sin REST API)
```

### Trabajar en el Design System

Para trabajar directamente en el paquete del design system:

```bash
cd packages/design-system
npm run storybook              # Iniciar Storybook
npm run dev                    # Iniciar Vite
```

## 🔗 Integración con Figma

Este proyecto usa **Figma Code Connect** para vincular componentes de Figma con su implementación en código.

### Configuración

1. Copia `.env-rename` a `.env` en la raíz del repositorio:
   ```bash
   cp .env-rename .env
   ```

2. Configura tus credenciales de Figma en `.env`:
   ```
   FIGMA_ACCESS_TOKEN=tu_token_aqui
   FIGMA_FILE_KEY=tu_file_key_aqui
   ```

### Sincronización

- **Tokens de diseño**: `npm run tokens:rest` - Sincroniza colores, tipografía y espaciado
- **Iconos**: `npm run icons:rest` - Genera componentes React desde iconos de Figma
- **Code Connect**: Los mappings se publican automáticamente al hacer merge a `main`

## 🎨 Storybook

Storybook está configurado para documentar todos los componentes del sistema de diseño.

```bash
# Desarrollo
npm run storybook

# Build
npm run storybook:build
```

URL local: http://localhost:6006/

## 📚 Documentación de Paquetes

- [Design System](./packages/design-system/README.md) - Documentación completa del sistema de diseño

## 🔄 CI/CD

El proyecto incluye workflows de GitHub Actions para:

- ✅ **PR Checks**: Verifica linting y build en cada PR
- 🚀 **Deploy to GitHub Pages**: Despliega automáticamente al hacer merge a `main`
- 🔗 **Code Connect Publish**: Publica automáticamente mappings a Figma
- 👀 **PR Previews**: Genera previews de Storybook en Netlify para cada PR

Ver [CI/CD Setup](./.github/CI-CD-SETUP.md) para más detalles.

## 🛠️ Tecnologías

- **React 18** - Framework de UI
- **TypeScript** - Tipado estático
- **Vite** - Build tool y dev server
- **Storybook 8** - Documentación de componentes
- **React Aria Components** - Componentes accesibles
- **Figma Code Connect** - Integración con Figma Dev Mode
- **npm Workspaces** - Gestión de monorepo

## 📄 Licencia

MIT
