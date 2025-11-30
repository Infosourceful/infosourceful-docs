# Color Palette Reference

> **Note:** This is an internal reference document, not published to the public documentation site.

This document catalogs the color palette used across the Infosourceful application and website. All colors are defined as CSS custom properties (variables) in `apps/desktop/src/styles/colors.css` for easy theming and consistency.

## Main Color Palette

### Background Colors

- **`--bg-main`**: `#FFFFFF` (White)
  - Main background color

- **`--bg-surface`**: `#FFFFFF` (White)
  - Used for cards and panes

- **`--bg-elevated`**: `#F8F5EE` (Parchment)
  - Elevated panels like mind map and sidebar

- **`--bg-hover`**: `#F5F1EA`
  - Hover surface states

### Text Colors

- **`--text-main`**: `#1A1A1A` (Graphite)
  - Primary text color

- **`--text-muted`**: `#4A4A4A`
  - Secondary text color

- **`--text-very-muted`**: `#6F6F6F`
  - Tertiary text color

### Accent Colors

- **`--accent-primary`**: `#C47B3C` (Copper)
  - Used for buttons, highlights, and selection states

- **`--accent-secondary`**: `#364B63` (Slate Blue)
  - Used for links and secondary actions

- **`--accent-soft`**: `#7A8F7E` (Lichen)
  - Used for tags/pills and soft states

- **`--accent-green`**: `#9FB5A8` (Lighter Lichen)
  - Used for format facets

### Border Colors

- **`--border-subtle`**: `#1A1A1A` (Graphite)
  - Subtle borders

- **`--border-strong`**: `#1A1A1A` (Graphite)
  - Strong borders

## Confidence Band Colors

Defined in `confidence.css`:

- **High Confidence**: `#3b82f6` (Blue)
- **Medium Confidence**: `#f59e0b` (Amber)
- **Low Confidence**: `#6b7280` (Gray)

## Ecofact Type Colors

Defined in `ecofactData.ts`:

### High Confidence (Blue - `#3b82f6`)
- Autosave
- Thumbnail
- Sync Artifact

### Low Confidence (Gray - `#6b7280`)
- Temp File
- Cache Residue
- Metadata Residue
- Sidecar

### Medium Confidence (Amber - `#f59e0b`)
- Partial Write
- Backup Fragment

### Error State (Red - `#ef4444`)
- Failed Conversion

## Special Component Colors

### Table Colors
- **Header Background**: `#E6C4A1` (Tan/Beige)
- **Header Text**: `#4B2C12` (Dark Brown)

### Error States
- **Error Background**: `#f8d7da` (Light Red)
- **Error Text**: `#721c24` (Dark Red)

### Warning States
- **Warning Background**: `rgba(196, 123, 60, 0.15)` (Copper with 15% opacity)
- **Warning Border**: `rgba(196, 123, 60, 0.3)` (Copper with 30% opacity)

## Mind Map Node Colors

- **`--node`**: `rgba(54, 75, 99, 0.1)` (Slate Blue with 10% opacity)
- **`--node-active`**: `rgba(54, 75, 99, 0.2)` (Slate Blue with 20% opacity)
- **`--node-facet`**: `rgba(54, 75, 99, 0.15)` (Slate Blue with 15% opacity)
- **`--node-filter`**: `rgba(54, 75, 99, 0.12)` (Slate Blue with 12% opacity)
- **`--node-metric`**: `rgba(196, 123, 60, 0.15)` (Copper with 15% opacity)

## Dark Mode Support

The `colors.css` file includes dark mode variants under `[data-theme="dark"]` with adjusted backgrounds and borders for dark theme support. All color variables are redefined for dark mode to ensure proper contrast and readability.

## Implementation Notes

- All colors are defined as CSS custom properties (CSS variables) in `apps/desktop/src/styles/colors.css`
- This allows for easy theming and consistency across the application
- Dark mode support is implemented through theme-specific variable overrides
- Color usage should follow the semantic naming conventions (e.g., `--accent-primary` for primary actions, not arbitrary color values)

