# Rulebook Company Design System Guide

## Color Palette

### Primary Colors
```css
--primary: #14B8A6;        /* Teal - Main brand color */
--primary-light: #5EEAD4;  /* Light Teal - Accents, highlights */
--primary-dark: #0F766E;   /* Dark Teal - Hover states, depth */
```

### Neutral Colors
```css
/* Light Mode */
--text-primary: #1F2937;   /* Dark Gray - Primary text */
--text-secondary: #6B7280; /* Medium Gray - Secondary text */
--background: #FFFFFF;     /* White - Main background */
--background-alt: #F9FAFB; /* Off-white - Alternate background */

/* Dark Mode */
--text-primary-dark: #F9FAFB;   /* Off-white - Primary text */
--text-secondary-dark: #D1D5DB; /* Light Gray - Secondary text */
--background-dark: #111827;     /* Near Black - Main background */
--background-alt-dark: #1F2937; /* Dark Gray - Alternate background */
```

### Semantic Colors
```css
--success: #10B981;   /* Green */
--warning: #F59E0B;   /* Amber */
--error: #EF4444;     /* Red */
--info: #3B82F6;      /* Blue */
```

### Opacity Variations
```css
--primary-opacity-10: rgba(20, 184, 166, 0.1);
--primary-opacity-20: rgba(20, 184, 166, 0.2);
--primary-opacity-50: rgba(20, 184, 166, 0.5);
```

## Typography

### Font Families
```css
--font-primary: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
--font-mono: 'SF Mono', 'Monaco', 'Inconsolata', 'Fira Code', monospace;
```

### Font Sizes
```css
--text-xs: 0.75rem;    /* 12px */
--text-sm: 0.875rem;   /* 14px */
--text-base: 1rem;     /* 16px */
--text-lg: 1.125rem;   /* 18px - Used in logos */
--text-xl: 1.25rem;    /* 20px */
--text-2xl: 1.5rem;    /* 24px */
--text-3xl: 1.875rem;  /* 30px */
--text-4xl: 2.25rem;   /* 36px */
--text-5xl: 3rem;      /* 48px */
```

### Font Weights
```css
--font-normal: 400;
--font-medium: 500;
--font-semibold: 600;
--font-bold: 700;      /* Used in branding */
```

### Line Heights
```css
--leading-tight: 1.25;
--leading-normal: 1.5;
--leading-relaxed: 1.75;
```

## Spacing System

### Scale (Based on 4px baseline)
```css
--space-0: 0;
--space-1: 0.25rem;   /* 4px */
--space-2: 0.5rem;    /* 8px */
--space-3: 0.75rem;   /* 12px */
--space-4: 1rem;      /* 16px */
--space-5: 1.25rem;   /* 20px */
--space-6: 1.5rem;    /* 24px */
--space-8: 2rem;      /* 32px */
--space-10: 2.5rem;   /* 40px */
--space-12: 3rem;     /* 48px */
--space-16: 4rem;     /* 64px */
--space-20: 5rem;     /* 80px */
--space-24: 6rem;     /* 96px */
```

## Border Radius

```css
--radius-none: 0;
--radius-sm: 0.125rem;    /* 2px */
--radius-base: 0.25rem;   /* 4px */
--radius-md: 0.375rem;    /* 6px */
--radius-lg: 0.5rem;      /* 8px */
--radius-xl: 0.75rem;     /* 12px */
--radius-2xl: 1rem;       /* 16px */
--radius-3xl: 1.5rem;     /* 24px */
--radius-full: 9999px;    /* Circular */
```

## Shadows

```css
--shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
--shadow-base: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px -1px rgba(0, 0, 0, 0.1);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -2px rgba(0, 0, 0, 0.1);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgba(0, 0, 0, 0.1);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1);
--shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
```

## Components

### Buttons

#### Primary Button
```css
.btn-primary {
  background-color: #14B8A6;
  color: #FFFFFF;
  font-weight: 600;
  padding: 0.75rem 1.5rem;
  border-radius: 0.5rem;
  transition: all 0.2s ease;
}

.btn-primary:hover {
  background-color: #0F766E;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}
```

#### Secondary Button
```css
.btn-secondary {
  background-color: transparent;
  color: #14B8A6;
  border: 2px solid #14B8A6;
  font-weight: 600;
  padding: 0.75rem 1.5rem;
  border-radius: 0.5rem;
  transition: all 0.2s ease;
}

.btn-secondary:hover {
  background-color: rgba(20, 184, 166, 0.1);
}
```

### Cards

```css
.card {
  background-color: #FFFFFF;
  border-radius: 0.75rem;
  padding: 1.5rem;
  box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.1);
  transition: box-shadow 0.2s ease;
}

.card:hover {
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}
```

### Input Fields

```css
.input {
  background-color: #FFFFFF;
  border: 1px solid #D1D5DB;
  border-radius: 0.5rem;
  padding: 0.75rem 1rem;
  font-size: 1rem;
  transition: all 0.2s ease;
}

.input:focus {
  outline: none;
  border-color: #14B8A6;
  box-shadow: 0 0 0 3px rgba(20, 184, 166, 0.1);
}
```

### Navigation

```css
.nav-link {
  color: #6B7280;
  font-weight: 500;
  padding: 0.5rem 1rem;
  transition: color 0.2s ease;
}

.nav-link:hover {
  color: #14B8A6;
}

.nav-link-active {
  color: #14B8A6;
  font-weight: 600;
}
```

## Logo Specifications

### Light Mode Logo
- **Dimensions**: 240px × 32px
- **Icon Color**: #14B8A6 (with 0.1 opacity background)
- **Text Color**: #1F2937
- **Font**: system-ui, -apple-system, sans-serif
- **Font Size**: 18px
- **Font Weight**: 700

### Dark Mode Logo
- **Dimensions**: 240px × 32px
- **Icon Color**: #5EEAD4 (with 0.2 opacity background)
- **Text Color**: #F9FAFB
- **Font**: system-ui, -apple-system, sans-serif
- **Font Size**: 18px
- **Font Weight**: 700

### Favicon
- **Dimensions**: 32px × 32px
- **Background**: #14B8A6 (circular, radius 15px)
- **Icon**: White document/book shape
- **Style**: Minimalist, centered

## Transitions & Animations

```css
/* Standard Transition */
--transition-base: all 0.2s ease;

/* Specific Transitions */
--transition-colors: color 0.2s ease, background-color 0.2s ease;
--transition-shadow: box-shadow 0.2s ease;
--transition-transform: transform 0.2s ease;
```

### Common Animation Patterns
```css
/* Hover Scale */
.hover-scale:hover {
  transform: scale(1.02);
}

/* Fade In */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Slide Up */
@keyframes slideUp {
  from { transform: translateY(10px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}
```

## Layout

### Container Widths
```css
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1536px;
```

### Breakpoints
```css
--breakpoint-sm: 640px;
--breakpoint-md: 768px;
--breakpoint-lg: 1024px;
--breakpoint-xl: 1280px;
--breakpoint-2xl: 1536px;
```

### Grid System
```css
.grid-2 { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1.5rem; }
.grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }
.grid-4 { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1.5rem; }
```

## Iconography

### Icon System
- **Style**: Outlined/stroke-based icons
- **Stroke Width**: 1.5px
- **Size Scale**: 16px, 20px, 24px, 32px
- **Color**: Matches text color or primary brand color

### Common Icons Used
- Document/Book (brand identity)
- Chart/Analytics
- Shield/Security
- Clock/Time
- Arrow/Navigation
- Check/Success indicators

## Accessibility

### Focus States
```css
:focus-visible {
  outline: 2px solid #14B8A6;
  outline-offset: 2px;
}
```

### Color Contrast Ratios
- Primary text on white: 13.6:1 (WCAG AAA)
- Primary brand on white: 3.2:1 (WCAG AA for large text)
- Links maintain 4.5:1 minimum

### Interactive Element Sizes
- Minimum touch target: 44px × 44px
- Button padding: minimum 12px vertical, 24px horizontal

## Design Principles

### 1. **Professional & Trustworthy**
- Clean, minimal design
- Consistent use of teal/green (trust, stability)
- Clear typography hierarchy

### 2. **Data-Focused**
- Emphasis on readability
- Monospace fonts for code/data
- Clear visual hierarchy for information

### 3. **Modern & Accessible**
- System fonts for performance
- Strong contrast ratios
- Clear focus indicators
- Responsive design patterns

### 4. **Fintech/Compliance Aesthetic**
- Professional color palette
- Documentation-style iconography
- Clean, structured layouts
- Emphasis on clarity and precision

## Usage Guidelines

### Do's
✓ Use the teal (#14B8A6) as the primary accent color
✓ Maintain consistent spacing using the 4px baseline
✓ Use system fonts for optimal performance
✓ Ensure 4.5:1 contrast ratio minimum for text
✓ Apply subtle shadows for depth
✓ Use the book/document iconography for brand consistency

### Don'ts
✗ Don't use colors outside the defined palette
✗ Don't mix different border radius scales
✗ Don't use decorative fonts
✗ Don't reduce spacing below the defined scale
✗ Don't use heavy animations on data-heavy pages
✗ Don't compromise accessibility for aesthetics

## File References

- **Logo (Light)**: `/logo/light.svg`
- **Logo (Dark)**: `/logo/dark.svg`
- **Favicon**: `/favicon.svg`
- **Color Config**: `docs.json` → colors section

## Version

Design System v1.0 - Last updated: February 2026
