# Color Component

Componente para mostrar muestras de color del sistema de diseño con información y funcionalidad de copiado.

## Uso

```html
<ds-color color="#0066CC" name="Primary Blue" size="md"></ds-color>
```

## Props

| Prop | Type | Default | Descripción |
|------|------|---------|-------------|
| `color` | `string` | `'#000000'` | Valor del color (hex, rgb, hsl, etc.) |
| `name` | `string` | `'Color'` | Nombre descriptivo del color |
| `size` | `'sm' \| 'md' \| 'lg' \| 'xl'` | `'md'` | Tamaño de la muestra |

## Tamaños

- `sm` - 60px × 60px
- `md` - 100px × 100px
- `lg` - 150px × 150px
- `xl` - 200px × 200px

## Ejemplos

### Colores Primarios

```html
<ds-color color="#0066CC" name="Primary"></ds-color>
<ds-color color="#00CC66" name="Success"></ds-color>
<ds-color color="#CC6600" name="Warning"></ds-color>
<ds-color color="#CC0000" name="Danger"></ds-color>
```

### Diferentes Tamaños

```html
<ds-color color="#0066CC" name="Small" size="sm"></ds-color>
<ds-color color="#0066CC" name="Medium" size="md"></ds-color>
<ds-color color="#0066CC" name="Large" size="lg"></ds-color>
<ds-color color="#0066CC" name="Extra Large" size="xl"></ds-color>
```

### Formatos de Color

```html
<ds-color color="#0066CC" name="Hex"></ds-color>
<ds-color color="rgb(0, 102, 204)" name="RGB"></ds-color>
<ds-color color="hsl(210, 100%, 40%)" name="HSL"></ds-color>
<ds-color color="var(--primary-color)" name="CSS Variable"></ds-color>
```

## Funcionalidad

### Copiar al Portapapeles

Haz click en el valor del color para copiarlo automáticamente al portapapeles. El componente mostrará "Copiado!" temporalmente como confirmación.

### Estados Interactivos

- **Hover en la muestra**: Escala ligeramente el elemento
- **Hover en el valor**: Cambia el color del texto
- **Click en el valor**: Copia el color al portapapeles

## Casos de Uso

Este componente es ideal para:
- Paletas de colores del sistema de diseño
- Guías de estilo de marca
- Documentación de tokens de color
- Selectores de color visuales
- Referencias rápidas de colores
