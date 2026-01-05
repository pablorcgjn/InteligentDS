# Button Component

Componente de botón reutilizable y accesible implementado como Web Component.

## Uso

```html
<ds-button variant="primary" size="md">Click me</ds-button>
```

## Props

| Prop | Type | Default | Descripción |
|------|------|---------|-------------|
| `variant` | `'primary' \| 'secondary' \| 'danger' \| 'ghost'` | `'primary'` | Variante visual del botón |
| `size` | `'sm' \| 'md' \| 'lg'` | `'md'` | Tamaño del botón |
| `disabled` | `boolean` | `false` | Deshabilita el botón |
| `type` | `'button' \| 'submit' \| 'reset'` | `'button'` | Tipo de botón HTML |

## Ejemplos

### Variantes

```html
<ds-button variant="primary">Primary</ds-button>
<ds-button variant="secondary">Secondary</ds-button>
<ds-button variant="danger">Danger</ds-button>
<ds-button variant="ghost">Ghost</ds-button>
```

### Tamaños

```html
<ds-button size="sm">Small</ds-button>
<ds-button size="md">Medium</ds-button>
<ds-button size="lg">Large</ds-button>
```

### Estados

```html
<ds-button disabled>Disabled</ds-button>
```

## Accesibilidad

- Soporte completo de navegación por teclado
- Estados de focus visibles
- Atributo `disabled` respetado
- Eventos de click propagados correctamente
