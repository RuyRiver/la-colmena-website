# Project Structure

## File Organization
```
la-colmena-website/
├── la-colmena.html          # Main website file (contains all HTML/CSS)
├── package-lock.json        # NPM lock file (minimal dependencies)
└── .kiro/                   # Kiro AI assistant configuration
    ├── specs/               # Project specifications
    │   └── la-colmena-website/
    │       ├── requirements.md
    │       ├── design.md
    │       └── tasks.md
    └── steering/            # AI guidance documents
        ├── product.md
        ├── tech.md
        └── structure.md
```

## HTML Document Structure
The single `la-colmena.html` file follows this semantic structure:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <!-- Meta tags, Google Fonts, embedded CSS -->
</head>
<body>
    <header class="header">
        <!-- Sticky navigation with logo and menu -->
    </header>
    <main>
        <section id="inicio">         <!-- Hero section -->
        <section id="sobre-el-proyecto"> <!-- About -->
        <section id="propuestas">     <!-- Service offerings -->
        <section id="servicios">      <!-- Services -->
        <section id="equipo">         <!-- Team profiles -->
    </main>
    <footer id="contacto">            <!-- Contact info -->
</body>
</html>
```

## CSS Organization Within File
CSS is embedded in `<style>` tags in the `<head>` and organized as:

1. **CSS Custom Properties** (`:root` selector)
2. **Reset & Base Styles** (normalize, typography)
3. **Layout Components** (container, sections)
4. **Header & Navigation** (desktop + mobile)
5. **Hero Section** (full-screen layout)
6. **Content Sections** (about, services, team)
7. **Footer** (contact information)
8. **Media Queries** (responsive breakpoints)

## Content Sections
- **Header**: Logo + navigation (responsive hamburger menu)
- **Hero**: Full-screen intro with CTAs
- **About**: Project history and mission
- **Proposals**: 4-card grid of service offerings
- **Services**: Space rental, residencies, volunteer program
- **Team**: Profile cards for founders
- **Footer**: Contact info, social links, navigation

## Naming Conventions
- **CSS Classes**: Semantic, component-based (`.hero`, `.nav-link`, `.btn-primary`)
- **IDs**: Section anchors for navigation (`#inicio`, `#sobre-el-proyecto`)
- **CSS Variables**: Descriptive with prefixes (`--color-`, `--spacing-`, `--fuente-`)
- **File naming**: Lowercase with hyphens (`la-colmena.html`)

## Responsive Breakpoints
- **Mobile**: Base styles (320px+)
- **Tablet**: `@media (min-width: 768px)`
- **Desktop**: `@media (min-width: 1024px)`

## Content Language
All content is in Spanish, targeting the Valencia arts community and Spanish-speaking international volunteers.