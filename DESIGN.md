---
version: alpha
name: BugZero IT Services Landing Page
description: A clean, corporate-focused landing page for IT managed services (infogérance) featuring a high-contrast blue and lime green palette, emphasizing reliability, security, and professionalism.
colors:
  primary: "#00AEEF"
  secondary: "#C4D600"
  surface-light: "#EEF9FF"
  surface-muted: "#F9FCE5"
  background: "#FFFFFF"
  background-alt: "#F9FAFB"
  text-main: "#171717"
  text-muted: "#525252"
  border: "#E5E5E5"
typography:
  family: "Inter, sans-serif"
  weights:
    regular: 400
    medium: 500
    semibold: 600
    bold: 700
  sizes:
    h1: "4.5rem"
    h2: "2.25rem"
    h3: "1.25rem"
    body-lg: "1.25rem"
    body-md: "1.125rem"
    body-sm: "0.875rem"
spacing:
  container: "max-w-7xl"
  section-py: "6rem"
  card-p: "2rem"
rounded:
  default: "0.375rem"
  large: "1rem"
  full: "9999px"
components:
  primary-button:
    bg: "{colors.primary}"
    text: "#FFFFFF"
    radius: "{rounded.default}"
    padding: "1rem 2rem"
  secondary-button:
    bg: "{colors.secondary}"
    text: "#171717"
    radius: "0.5rem"
  feature-card:
    bg: "#FFFFFF"
    border: "1px solid {colors.border}"
    shadow: "sm"
---

## Overview
The BugZero design language communicates stability and modern technical expertise. It utilizes a white-base layout with strategic applications of Azure Blue (#00AEEF) for primary actions and Lime Green (#C4D600) for secondary accents and trust signals. The interface is high-density but legible, using wide gutters, structured grids, and prominent status indicators (like the live system heartbeat) to reinforce the concept of "active monitoring."

## Colors
- **Primary Blue (#00AEEF)**: Used for the "BUG" portion of the logo, primary call-to-action buttons, icons, and text accents like "notre sérénité."
- **Accent Lime (#C4D600)**: Used for the "ZERO" portion of the logo, decorative borders on dashboard cards, trust icons (stars), and the primary "Audit" CTA in the footer.
- **Neutral Palette**: Ranges from deep charcoal (#171717) for headings to a light gray (#F9FAFB) for alternate section backgrounds.
- **Functional Tones**: Green (#22C55E) for "100% online" status indicators and light blue (#EEF9FF) for badge backgrounds.

## Typography
- **Primary Font**: Inter (via Google Fonts). System fallbacks include -apple-system and Roboto.
- **Headings**: Heavy weights (Bold 700) with tight tracking (`tracking-tight` and `tracking-tighter`).
- **Body Text**: Large, readable sizes (1.125rem) in Neutral-600 for high contrast without harshness.
- **Utility Text**: Uppercase, semibold tracking for badges and small labels to establish hierarchy.

## Layout
- **Grid System**: Standard 12-column logic implemented via Tailwind. Desktop uses `grid-cols-2` for hero and `grid-cols-3` for service and testimonial blocks.
- **Container**: Max width of 1280px (`max-w-7xl`) with 24px (`px-6`) side padding on mobile.
- **Spacing**: Generous vertical breathing room with 96px (`py-24`) to 128px (`py-32`) between major sections.
- **Sticky Elements**: The navigation bar is fixed to the top with a `backdrop-blur-md` and 95% opacity background.

## Elevation & Depth
- **Cards**: Minimal depth using `shadow-sm`. Interaction triggers a transition to `shadow-md` or `shadow-xl`.
- **Glassmorphism**: Applied to the navbar using `bg-white/95 backdrop-blur-md` to maintain context while scrolling.
- **Borders**: Thin 1px borders in Neutral-200/100 define containers rather than heavy drop shadows.

## Shapes
- **Component Radii**: Standard buttons use a subtle 6px radius (`rounded-md`). Service cards use a softer 12px radius (`rounded-xl`). The status dashboard card in the hero uses a 16px radius (`rounded-2xl`).
- **Pill Shapes**: Full rounding (`rounded-full`) reserved for decorative status badges and step indicators in the "How it works" section.

## Components
- **Navigation Bar**: High-contrast, height of 80px (`h-20`), containing a split-color logo and medium-weight text links.
- **Hero Card**: A sophisticated "System Status" mock-up card featuring a pulse animation, progress bars (placeholders), and a status toggle top-border in lime green.
- **Service Tiles**: White background tiles with colored icon containers (14x14 size) and bolded titles.
- **Step Indicators**: Large 96px (`w-24`) circular numbers connected by a light blue horizontal line on desktop.
- **Testimonial Blocks**: Light gray containers with a 5-star rating header and italicized typography for quotes.

## Page Sections

### Navigation
- **Composition**: Logo left, links center-right, CTA right.
- **Style**: White background, bottom border in Neutral-200.
- **Interactions**: Hover color shift on links to Primary Blue.

### Hero Section
- **Composition**: Split layout. Left side contains a pill-badge, h1, body text, and two large CTAs. Right side contains the simulated "System Status" dashboard.
- **Content Hierarchy**: Strong focus on the value proposition "notre sérénité."
- **Visuals**: A lime green top-border on the status card provides a unique visual anchor.

### Services / Expertises
- **Structure**: 3-column grid.
- **Styling**: Neutral-50 background to separate from the hero. Cards use standard icon-title-description vertical stack.

### Why Us (About)
- **Structure**: Two-column layout where the left column is `sticky` on desktop. Right column is a 2x2 grid of smaller feature cards.
- **Details**: Features a specific Azure Blue thick horizontal rule (w-20 h-1.5) as a divider.

### Methodology (How it Works)
- **Visual**: Three steps with large numbered circles. Step 2 is inverted (Primary Blue background) to draw the eye to the "Plan of Action."
- **Background**: Soft blue fill (#EEF9FF).

### Testimonials
- **Style**: Uses specific star icons in Lime Green. Neutral-50 rounded boxes provide a clean "feedback" aesthetic.

### Final CTA / Contact
- **Visual**: High-impact Primary Blue background with white text. The main button is Lime Green to ensure maximum conversion contrast.
- **Typography**: Expanded heading size (up to 6xl) for a bold finish.

## Motion & Interaction
- **Transitions**: Global `transition-colors` and `transition-all` on all buttons and links with a standard duration (approx 200ms).
- **Animations**:
  - **Pulse**: A `green-500` dot in the hero card uses `animate-pulse` to signify a live connection.
  - **Button Hover**: The primary CTA in the contact section uses `hover:-translate-y-1` to create a tactile lift effect.

## Do's and Don'ts
- **Do**: Use the split-color logo (BUG=Blue, ZERO=Lime) consistently.
- **Do**: Maintain the 15-minute response time and "Proximity" messaging as key differentiators.
- **Don't**: Use gradients; the brand relies on solid blocks of Azure Blue and Lime Green.
- **Don't**: Use sharp 0px corners; all interactive elements should have at least a `rounded-md` corner.

## Accessibility
- **Contrast**: High contrast text (Neutral-900 on White or White on Primary Blue) is used for readability.
- **Semantic HTML**: Uses `<nav>`, `<section>`, `<footer>`, and `<h1-h4>` tags for screen reader structure.
- **Icons**: Lucide icons are used with descriptive text labels in the UI to ensure meaning is not lost.

## Assets
1. Lucide Icons Library: `https://unpkg.com/lucide@latest`
2. Tailwind CSS: `https://cdn.tailwindcss.com`
3. Primary Font: `https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap`
4. Logo Favicon: `data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><rect width='100' height='100' rx='20' fill='%2300AEEF'/><text x='50' y='70' font-size='65' font-family='sans-serif' font-weight='bold' fill='white' text-anchor='middle'>B</text></svg>`
5. Internal Service Link: `/services`
6. Internal Contact Link: `/contact`

### Exported Codebase Asset Inventory
1. embed: https://fonts.gstatic.com
   Context: index.html: markup attribute; index.html: absolute url literal
2. embed: https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&amp;display=swap
   Context: index.html: markup attribute; index.html: absolute url literal
