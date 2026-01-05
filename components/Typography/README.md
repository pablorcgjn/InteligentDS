# Typography Component

Componente de tipografía para renderizar texto con estilos consistentes del sistema de diseño.

## Uso

```html
<ds-typography variant="title-hero">Título Principal</ds-typography>
```

## Props

| Prop | Type | Default | Descripción |
|------|------|---------|-------------|
| `variant` | Typography Variant | `'body-base'` | Variante de tipografía |
| `color` | `string` | `'inherit'` | Color del texto (CSS color) |
| `weight` | `string` | `'normal'` | Peso de la fuente (CSS font-weight) |

## Variantes Disponibles

### Títulos
- `title-hero` - 3.6rem, peso 700, para héroes de página
- `title-page` - 2.8rem, peso 700, para títulos de página
- `subtitle` - 1.5rem, peso 600, para subtítulos
- `heading` - 1.25rem, peso 700, para encabezados
- `subheading` - 1.125rem, peso 600, para sub-encabezados

### Cuerpo
- `body-base` - 1rem, peso 400, texto base
- `body-small` - 0.875rem, peso 400, texto pequeño
- `body-strong` - Peso 700, texto en negrita
- `body-emphasis` - Estilo itálico, texto enfatizado
- `body-link` - Estilo de enlace con color primario
- `body-code` - Estilo de código con fuente monoespaciada
- `input` - 1rem, peso 400, para campos de entrada

## Ejemplos

### Títulos

```html
<ds-typography variant="title-hero">Título Hero</ds-typography>
<ds-typography variant="title-page">Título de Página</ds-typography>
<ds-typography variant="subtitle">Subtítulo</ds-typography>
```

### Cuerpo de Texto

```html
<ds-typography variant="body-base">Texto base normal</ds-typography>
<ds-typography variant="body-small">Texto pequeño</ds-typography>
<ds-typography variant="body-strong">Texto en negrita</ds-typography>
```

### Con Colores Personalizados

```html
<ds-typography variant="heading" color="#FF0000">Encabezado Rojo</ds-typography>
<ds-typography variant="body-base" color="var(--custom-color)">Texto con variable CSS</ds-typography>
```

### Código y Enlaces

```html
<ds-typography variant="body-code">const variable = 'value';</ds-typography>
<ds-typography variant="body-link">Enlace de navegación</ds-typography>
```

## Tokens de Diseño

Este componente utiliza tokens de diseño para mantener la consistencia:
- Variables CSS para colores (`--ds-color-primary`, `--ds-color-background-secondary`)
- Escalas de tamaño consistentes
- Alturas de línea optimizadas para legibilidad
- Letter-spacing apropiado para cada tamaño
