# DS-Simple - Sistema de Diseño

## Descripción del Proyecto
DS-Simple es un sistema de diseño que proporciona una biblioteca de componentes reutilizables y tokens de diseño para un desarrollo UI consistente.

## Estructura del Proyecto
```
DS-Simple/
├── README.md           # Documentación del proyecto
└── CLAUDE.MD          # Contexto para asistentes IA (este archivo)
```

## Propósito
Este sistema de diseño tiene como objetivo:
- Proporcionar componentes UI reutilizables
- Establecer patrones de diseño consistentes
- Mantener tokens de diseño (colores, espaciado, tipografía)
- Garantizar accesibilidad y mejores prácticas

## Guías de Desarrollo

### Estilo de Código
- Seguir convenciones de nomenclatura consistentes
- Escribir código limpio y autodocumentado
- Mantener componentes pequeños y enfocados
- Priorizar la accesibilidad (a11y)

### Desarrollo de Componentes
Al crear componentes:
1. Comenzar con HTML semántico
2. Aplicar estilos a través de tokens de diseño
3. Asegurar soporte de navegación por teclado
4. Agregar etiquetas ARIA donde sea necesario
5. Probar en diferentes tamaños de pantalla

### Tokens de Diseño
Los tokens de diseño deben incluir:
- **Colores**: Paletas primarias, secundarias y neutrales
- **Tipografía**: Familias de fuentes, tamaños, pesos, alturas de línea
- **Espaciado**: Escala de espaciado consistente
- **Breakpoints**: Puntos de quiebre para diseño responsivo
- **Sombras**: Sistema de elevación
- **Border Radius**: Redondeo de esquinas consistente

## Trabajando con Este Proyecto

### Primeros Pasos
Este proyecto está en etapas iniciales. Los próximos pasos clave pueden incluir:
- Configurar un sistema de build (Vite, Webpack, etc.)
- Elegir un framework de componentes (React, Vue, Web Components, etc.)
- Establecer la estructura de tokens de diseño
- Crear documentación de componentes

### Organización de Archivos (Recomendada)
```
src/
├── components/        # Componentes UI
├── tokens/           # Tokens de diseño
├── utils/            # Funciones utilitarias
└── styles/           # Estilos globales
```

## Convenciones

### Nomenclatura
- Usar nombres descriptivos y claros
- Componentes: PascalCase (ej., `Button`, `Card`)
- Utilidades: camelCase (ej., `formatDate`, `validateEmail`)
- Constantes: UPPER_SNAKE_CASE (ej., `PRIMARY_COLOR`)

### Flujo de Git
- Trabajar en ramas de características
- Escribir mensajes de commit claros
- Mantener commits atómicos y enfocados

## Notas para Asistentes IA

### Contexto
- Este es un proyecto de sistema de diseño
- Actualmente en fase inicial/configuración
- Sin sistema de build o dependencias configuradas aún

### Al Realizar Cambios
- Preguntar sobre preferencias de framework/herramientas antes de agregar dependencias
- Seguir las mejores prácticas de sistemas de diseño
- Considerar la reutilización y composición de componentes
- Mantener consistencia con patrones existentes
- Documentar nuevos componentes y patrones

### Consideraciones Prioritarias
1. **Accesibilidad**: Asegurar que todos los componentes sean accesibles
2. **Consistencia**: Mantener el uso de tokens de diseño
3. **Simplicidad**: Mantener la API simple e intuitiva
4. **Rendimiento**: Optimizar para tamaño de bundle y tiempo de ejecución
5. **Documentación**: Mantener la documentación actualizada

## Consideraciones Futuras
- Estructura de biblioteca de componentes
- Configuración de build y empaquetado
- Estrategia de testing (unitarias, regresión visual)
- Sitio de documentación (Storybook, docs personalizados)
- Proceso de versionado y releases
- Distribución de paquetes (npm, etc.)
