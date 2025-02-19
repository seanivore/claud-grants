# Build Guide for $CLAUD Site

## Core Principles

### 1. Structural Consistency
- Use semantic HTML5 elements (`<header>`, `<main>`, `<section>`, `<footer>`)
- Maintain consistent class naming patterns
- Follow a clear container hierarchy
- Use BEM-like naming for complex components

### 2. Class Naming Conventions
```html
/* Base Layout Classes */
.section              /* Major content blocks with proper spacing */
.content-wrap         /* Standard width container (800px) */
.content-wrap-wide    /* Full width container with padding */
.grid-container       /* For grid-based layouts */

/* Component Classes */
.feature-card         /* Individual feature displays */
.animation-container  /* For physics/particle animations */
.neon-text           /* For glowing text effects */
```

### 3. Protected Elements
The following should not be modified:
- Color variables in `:root`
- Font families
- Base animation timings
- Core layout structure

## Build Phases

### Phase 1: Core Structure
1. Set up semantic HTML structure
2. Implement canvas layers
3. Create basic content containers
4. Add placeholder sections

### Phase 2: Content Integration
1. Convert markdown content to HTML
2. Implement grid layouts
3. Add animation containers
4. Structure technical examples

### Phase 3: Animation Integration
1. Set up canvas contexts
2. Implement physics system
3. Add particle effects
4. Test performance

### Phase 4: Polish & Optimization
1. Add responsive behaviors
2. Implement accessibility features
3. Optimize animations
4. Test cross-browser compatibility

## HTML Structure Example
```html
<body>
    <!-- Background Canvas -->
    <div class="canvas-container">
        <canvas id="background-canvas"></canvas>
    </div>

    <!-- Content Layer -->
    <main class="content-layer">
        <!-- Masthead -->
        <header class="masthead">
            <canvas id="masthead-canvas"></canvas>
        </header>

        <!-- Features Section -->
        <section class="section features">
            <div class="content-wrap">
                <h2>Core Features</h2>
            </div>
            <div class="content-wrap-wide">
                <div class="grid-container">
                    <!-- Feature cards -->
                </div>
            </div>
        </section>

        <!-- Technical Section -->
        <section class="section technical">
            <!-- Technical content -->
        </section>
    </main>
</body>
```

## CSS Guidelines

### 1. Layout Structure
- Use CSS Grid for complex layouts
- Flexbox for component-level alignment
- Maintain consistent spacing units
- Use relative units (rem, em) for spacing

### 2. Animation Performance
- Use `transform` and `opacity` for animations
- Implement `will-change` strategically
- Consider reduced-motion preferences
- Hardware acceleration for canvas elements

### 3. Responsive Design
- Mobile-first approach
- Breakpoints at standard device sizes
- Fluid typography
- Maintain animation performance across devices

## Permissions & Flexibility

### You May:
- Add new CSS classes as needed
- Extend existing animations
- Create additional container types
- Implement new interactive features
- Optimize performance
- Add accessibility features

### You Must:
- Maintain existing color schemes
- Keep core font choices
- Follow established naming patterns
- Preserve animation timing variables
- Keep the physics-based animation system

## Quality Standards
- Valid HTML5
- CSS property order consistency
- Proper nesting of selectors
- Clear component boundaries
- Performance-conscious animations
- Accessible interactive elements

## Reference Files
- `SPECIFICATIONS.md` for design requirements
- `animation-specifications.md` for animation details
- `styles.css` for current styling
- `index.html` for structure example 