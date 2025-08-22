# AcquiSense - Design Guidelines

## 🎨 Brand Identity & Visual System

### Brand Personality
**Core Values:**
- **Empathetic:** Understands the struggle of finding first customers
- **Confident:** Data-driven recommendations inspire trust
- **Accessible:** Complex AI analysis made simple and actionable
- **Results-focused:** Customer acquisition, not vanity metrics

**Brand Voice:**
- **Tone:** Friendly yet professional, like a knowledgeable peer
- **Language:** Clear, jargon-free, action-oriented
- **Messaging:** "From product to profit in 30 days"

### Logo & Typography

#### Logo Concept
- **Symbol:** Upward trending arrow combined with a network/connection icon
- **Colors:** Primary blue (#2563eb) with accent green (#10b981)
- **Style:** Modern, clean, scalable for web and mobile

#### Typography Hierarchy
```css
/* Primary Font: Inter (web-safe, excellent readability) */
--font-primary: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;

/* Headings */
h1: 32px, font-weight: 700, line-height: 1.2
h2: 24px, font-weight: 600, line-height: 1.3
h3: 20px, font-weight: 600, line-height: 1.4
h4: 18px, font-weight: 500, line-height: 1.4

/* Body Text */
body: 16px, font-weight: 400, line-height: 1.6
small: 14px, font-weight: 400, line-height: 1.5
caption: 12px, font-weight: 500, line-height: 1.4
```

### Color Palette

#### Primary Colors
```css
/* Brand Colors */
--primary-blue: #2563eb;      /* Main CTA buttons, links */
--primary-blue-light: #3b82f6; /* Hover states */
--primary-blue-dark: #1d4ed8;  /* Active states */

--accent-green: #10b981;      /* Success states, positive metrics */
--accent-green-light: #34d399; /* Success backgrounds */
--accent-green-dark: #059669;  /* Success borders */

--accent-orange: #f59e0b;     /* Warning states, attention */
--accent-red: #ef4444;        /* Error states, negative metrics */
```

#### Neutral Colors
```css
/* Gray Scale */
--gray-50: #f9fafb;   /* Page backgrounds */
--gray-100: #f3f4f6;  /* Card backgrounds */
--gray-200: #e5e7eb;  /* Borders, dividers */
--gray-400: #9ca3af;  /* Placeholder text */
--gray-600: #4b5563;  /* Secondary text */
--gray-800: #1f2937;  /* Primary text */
--gray-900: #111827;  /* Headings */
```

### Component Design System

#### Buttons
```css
/* Primary Button */
.btn-primary {
  background: var(--primary-blue);
  color: white;
  padding: 12px 24px;
  border-radius: 8px;
  font-weight: 500;
  transition: all 0.2s ease;
}
.btn-primary:hover {
  background: var(--primary-blue-light);
  transform: translateY(-1px);
}

/* Secondary Button */
.btn-secondary {
  background: transparent;
  color: var(--primary-blue);
  border: 1px solid var(--primary-blue);
  padding: 12px 24px;
  border-radius: 8px;
}

/* Success Button */
.btn-success {
  background: var(--accent-green);
  color: white;
  padding: 12px 24px;
  border-radius: 8px;
}
```

#### Cards & Containers
```css
/* Main Content Cards */
.card {
  background: white;
  border: 1px solid var(--gray-200);
  border-radius: 12px;
  padding: 24px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}

/* Metric Cards */
.metric-card {
  background: white;
  border: 1px solid var(--gray-200);
  border-radius: 8px;
  padding: 20px;
  text-align: center;
}

/* Success Card (positive metrics) */
.success-card {
  background: var(--accent-green-light);
  border: 1px solid var(--accent-green);
  color: var(--accent-green-dark);
}
```

#### Form Elements
```css
/* Input Fields */
.input {
  border: 1px solid var(--gray-300);
  border-radius: 6px;
  padding: 10px 12px;
  font-size: 16px;
  transition: border-color 0.2s ease;
}
.input:focus {
  border-color: var(--primary-blue);
  outline: none;
  box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
}

/* Select Dropdowns */
.select {
  appearance: none;
  background: url('chevron-down.svg') no-repeat right 12px center;
  background-size: 16px;
  padding-right: 40px;
}
```

### Layout & Spacing

#### Grid System
```css
/* Container Max-widths */
.container-sm: max-width: 640px;
.container-md: max-width: 768px;
.container-lg: max-width: 1024px;
.container-xl: max-width: 1280px;

/* Spacing Scale (rem units) */
--space-1: 0.25rem;  /* 4px */
--space-2: 0.5rem;   /* 8px */
--space-3: 0.75rem;  /* 12px */
--space-4: 1rem;     /* 16px */
--space-6: 1.5rem;   /* 24px */
--space-8: 2rem;     /* 32px */
--space-12: 3rem;    /* 48px */
--space-16: 4rem;    /* 64px */
```

#### Navigation Layout
- **Header Height:** 64px
- **Sidebar Width:** 280px (desktop), collapsible on mobile
- **Main Content:** Centered with max-width: 1200px
- **Card Spacing:** 24px between cards

### Icons & Illustrations

#### Icon System
**Library:** Heroicons (outline style for consistency)
**Size Standards:**
- Small icons: 16px (inline with text)
- Medium icons: 20px (buttons, form elements)
- Large icons: 24px (headers, feature highlights)

#### Key Icons
- **Analysis:** TrendingUpIcon
- **Templates:** DocumentTextIcon
- **Dashboard:** ChartBarIcon
- **Settings:** CogIcon
- **Success:** CheckCircleIcon
- **Warning:** ExclamationTriangleIcon

### Data Visualization

#### Chart Colors
```css
/* Primary Data Series */
--chart-blue: #3b82f6;
--chart-green: #10b981;
--chart-orange: #f59e0b;
--chart-purple: #8b5cf6;
--chart-pink: #ec4899;

/* Background & Grid */
--chart-background: #fafafa;
--chart-grid: #e5e7eb;
--chart-text: #6b7280;
```

#### Chart Styles
- **Line Charts:** 2px stroke width, rounded line caps
- **Bar Charts:** 8px border radius on top corners
- **Progress Bars:** 8px height, rounded ends
- **Pie Charts:** 4px spacing between segments

### Mobile Design Principles

#### Responsive Breakpoints
```css
/* Mobile First Approach */
/* Mobile: default styles */
/* Tablet: 768px and up */
/* Desktop: 1024px and up */
/* Large Desktop: 1280px and up */

@media (min-width: 768px) { /* Tablet styles */ }
@media (min-width: 1024px) { /* Desktop styles */ }
@media (min-width: 1280px) { /* Large desktop */ }
```

#### Mobile-Specific Patterns
- **Navigation:** Hamburger menu with slide-out drawer
- **Cards:** Full-width with 16px side margins
- **Buttons:** Minimum 44px touch target
- **Forms:** Stack vertically, larger input fields

### Accessibility Guidelines

#### Color Contrast
- **Text on white:** Minimum 4.5:1 contrast ratio
- **Large text:** Minimum 3:1 contrast ratio
- **Interactive elements:** Clear focus indicators

#### Keyboard Navigation
- **Tab order:** Logical flow through interface
- **Focus indicators:** 2px blue outline
- **Skip links:** Available for screen readers

#### Screen Reader Support
- **Alt text:** All images and icons
- **ARIA labels:** Form elements and interactive components
- **Semantic HTML:** Proper heading hierarchy

### Animation & Micro-interactions

#### Transition Guidelines
```css
/* Standard transitions */
--transition-fast: 0.15s ease-out;
--transition-base: 0.2s ease-out;
--transition-slow: 0.3s ease-out;

/* Hover effects */
.interactive:hover {
  transform: translateY(-1px);
  transition: transform var(--transition-fast);
}

/* Loading states */
.loading {
  animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
```

#### Success Animations
- **Button clicks:** Brief scale animation (0.95x to 1x)
- **Form success:** Green checkmark fade-in
- **Data loading:** Skeleton screens, not spinners
- **Page transitions:** Subtle fade-in effects

### Error States & Empty States

#### Error Messages
```css
.error {
  background: #fef2f2;
  border: 1px solid #fecaca;
  color: #dc2626;
  padding: 12px;
  border-radius: 6px;
  font-size: 14px;
}
```

#### Empty States
- **No data:** Friendly illustration with clear CTA
- **Search results:** Helpful suggestions for refinement
- **Loading:** Skeleton screens matching final layout
- **Errors:** Clear explanation with next steps

### Performance Guidelines

#### Image Optimization
- **Format:** WebP with JPEG fallback
- **Sizing:** Responsive images with srcset
- **Loading:** Lazy loading for below-fold content
- **Compression:** 80% quality for photos, lossless for graphics

#### CSS Architecture
- **Methodology:** Tailwind CSS utility-first approach
- **Critical CSS:** Inline above-the-fold styles
- **Unused CSS:** Regular purging in production
- **Custom properties:** CSS variables for theme consistency