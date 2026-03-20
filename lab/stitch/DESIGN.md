# Design System Document

## 1. Overview & Creative North Star: "The Digital Curator"

This design system is built upon the concept of **"The Digital Curator."** In an era of AI noise, this system emphasizes "Identity-First" intelligence through clarity, intentionality, and high-end editorial aesthetics. It moves away from the "app-like" density of standard SaaS tools, opting instead for a spacious, gallery-like experience that feels both secure and human-centric.

The North Star is defined by **Sophisticated Transparency**. We utilize layered surfaces, glassmorphism, and a dominant use of negative space to suggest an environment that is open yet protected. By breaking the rigid, boxed grid with intentional asymmetry and high-contrast typography scales, we create a signature visual identity that signals premium intelligence.

---

## 2. Colors

The palette is rooted in a "Sophisticated Tech" ethos, using deep purples and monochromatic neutrals to establish a sense of authority and trust.

### Primary Accents & Interaction
*   **Primary (`#6334af`) & Primary-Container (`#7c4fc9`):** Our signature "Octo Purple." Use these for core brand moments and primary actions.
*   **The "Signature Gradient":** Main CTAs and Hero backgrounds should utilize a linear gradient from `primary` to `primary_container` at a 135-degree angle. This adds "soul" and depth that flat fills cannot achieve.

### Surface & Tonal Architecture
*   **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. Structural boundaries must be defined solely through background color shifts. For example, a `surface-container-low` section should sit directly against a `background` (`#fcf9f8`) to define its bounds.
*   **Surface Hierarchy:** Use the hierarchy from `surface-container-lowest` (pure white/highest elevation) to `surface-dim` to create a sense of physical layering.
*   **The Glass Rule:** For floating elements like navigation bars or hover-state cards, use `surface_container_lowest` at 80% opacity with a `backdrop-blur` of 20px. This creates a "frosted glass" effect that keeps the UI feeling integrated and lightweight.

---

## 3. Typography

The typography scale utilizes **Plus Jakarta Sans** for high-impact editorial moments and **Inter** for functional readability.

*   **Display (Plus Jakarta Sans):** Set at `3.5rem` (Large) to `2.25rem` (Small). These are the "headlines of the gallery." Use tight letter-spacing (-0.02em) and "Bold" weights to command attention.
*   **Headline & Title (Plus Jakarta Sans/Inter):** Headlines use Plus Jakarta Sans to maintain brand voice, while Titles shift to Inter for a more technical, "Identity-First" feel.
*   **Body & Labels (Inter):** All functional text uses Inter. Use `body-lg` (1rem) for primary narratives and `label-md` (0.75rem) for metadata.
*   **Hierarchy Note:** To achieve a premium look, increase the contrast between Display and Body. Large, bold headers paired with generous white space and smaller, well-leaded body text creates an "Executive Summary" feel.

---

## 4. Elevation & Depth

We reject the "Shadow-Box" aesthetic of the 2010s in favor of **Tonal Layering**.

*   **The Layering Principle:** Depth is achieved by stacking surface tokens.
    *   *Level 0 (Base):* `surface`
    *   *Level 1 (Sections):* `surface-container-low`
    *   *Level 2 (Cards/Interaction):* `surface-container-lowest`
*   **Ambient Shadows:** If an element must float (e.g., a modal), use a shadow with a blur radius of 40px-60px at 4%-6% opacity. The shadow color should be a tinted `primary` (purple-hued) rather than grey, simulating natural light passing through a prism.
*   **The Ghost Border Fallback:** If accessibility requires a stroke, use `outline_variant` at 15% opacity. High-contrast, 100% opaque borders are strictly forbidden.

---

## 5. Components

### Buttons
*   **Primary:** Gradient fill (`primary` to `primary_container`) with `on_primary` text. Roundedness: `full` or `xl`.
*   **Secondary:** `surface_container_highest` fill with `primary` text. No border.
*   **Tertiary:** Text-only with an underline that appears on hover using the `primary` color.

### Input Fields
*   **Style:** Minimalist. No background fill on default; only a `ghost border` at the bottom or a very subtle `surface_container_low` background. 
*   **Focus State:** The bottom border transforms into a 2px `primary` line. Use a subtle `primary` glow (low-opacity shadow).

### Cards & Lists
*   **Strict Rule:** No divider lines. Use `spacing-8` or `spacing-10` to separate list items. 
*   **Card Structure:** Use `surface_container_lowest` for cards. Interaction is signaled by a subtle scale-up (1.02x) and an increase in the ambient shadow, rather than a color change.

### Chips
*   **Style:** Use `secondary_container` for background with `on_secondary_container` text. Keep corners `full` to maintain a "pill" aesthetic that feels modern and approachable.

---

## 6. Do's and Don'ts

### Do
*   **DO** use asymmetric layouts. Align a headline to the far left while the body text sits in a 6-column grid on the right.
*   **DO** use "Breathing Room." If you think there is enough margin, add `spacing-4` more. 
*   **DO** use the `primary` purple sparingly as a "laser-focus" accent—for buttons, icons, or text highlights.

### Don't
*   **DON'T** use black (`#000000`) for text. Use `on_surface` (`#1b1c1c`) to maintain a softer, premium feel.
*   **DON'T** use 1px dividers to separate content. Use background tonal shifts or white space.
*   **DON'T** use standard "Drop Shadows." Use ambient, large-blur, tinted shadows only when elevation is functional.
*   **DON'T** crowd the interface. If a screen feels "busy," remove elements until only the core identity-driven action remains.