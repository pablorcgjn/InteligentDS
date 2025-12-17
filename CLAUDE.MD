# DS-Simple - Design System

## Project Overview
DS-Simple is a design system project aimed at providing a simple, reusable component library and design tokens for consistent UI development.

## Project Structure
```
DS-Simple/
├── README.md           # Project documentation
└── CLAUDE.MD          # AI assistant context (this file)
```

## Purpose
This design system aims to:
- Provide reusable UI components
- Establish consistent design patterns
- Maintain design tokens (colors, spacing, typography)
- Ensure accessibility and best practices

## Development Guidelines

### Code Style
- Follow consistent naming conventions
- Write clean, self-documenting code
- Keep components small and focused
- Prioritize accessibility (a11y)

### Component Development
When creating components:
1. Start with semantic HTML
2. Apply styling through design tokens
3. Ensure keyboard navigation support
4. Add ARIA labels where needed
5. Test across different screen sizes

### Design Tokens
Design tokens should include:
- **Colors**: Primary, secondary, neutral palettes
- **Typography**: Font families, sizes, weights, line heights
- **Spacing**: Consistent spacing scale
- **Breakpoints**: Responsive design breakpoints
- **Shadows**: Elevation system
- **Border Radius**: Consistent corner rounding

## Working with This Project

### Getting Started
This project is in early stages. Key next steps may include:
- Setting up a build system (Vite, Webpack, etc.)
- Choosing a component framework (React, Vue, Web Components, etc.)
- Establishing design token structure
- Creating component documentation

### File Organization (Recommended)
```
src/
├── components/        # UI components
├── tokens/           # Design tokens
├── utils/            # Utility functions
└── styles/           # Global styles
```

## Conventions

### Naming
- Use descriptive, clear names
- Components: PascalCase (e.g., `Button`, `Card`)
- Utilities: camelCase (e.g., `formatDate`, `validateEmail`)
- Constants: UPPER_SNAKE_CASE (e.g., `PRIMARY_COLOR`)

### Git Workflow
- Work on feature branches
- Write clear commit messages
- Keep commits atomic and focused

## Notes for AI Assistants

### Context
- This is a design system project (sistema de diseño)
- Currently in early/setup phase
- No build system or dependencies configured yet

### When Making Changes
- Ask about framework/tooling preferences before adding dependencies
- Follow design system best practices
- Consider component reusability and composability
- Maintain consistency with existing patterns
- Document new components and patterns

### Priority Considerations
1. **Accessibility**: Ensure all components are accessible
2. **Consistency**: Maintain design token usage
3. **Simplicity**: Keep the API simple and intuitive
4. **Performance**: Optimize for bundle size and runtime
5. **Documentation**: Keep documentation up to date

## Future Considerations
- Component library structure
- Build and bundling setup
- Testing strategy (unit, visual regression)
- Documentation site (Storybook, custom docs)
- Versioning and release process
- Package distribution (npm, etc.)
