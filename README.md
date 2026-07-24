# African Pool Pros — UI & Sprites (Design Handoff)

## Overview
This document captures the visual design requirements and handoff for African Pool Pros, a Unity-based mobile 8‑ball pool game. Deliverables: a Figma-based UI kit (preferred) plus exported production-ready sprites (PNG/SVG) ready for Unity import.

## Design Goals
- Dark/charcoal backgrounds with gold/amber primary accent (#F2B705).
- African-themed branding with glowing card/panel style and rounded rectangles.
- Reusable components with variants (default / pressed / disabled / locked / selected).
- Provide assets and documentation so Unity integration requires minimal rework.

## Scoped Screens
Master set: 16 screens. Four reference screens define the system:
- Home / Lobby
- Avatar Store
- Clubs
- World Leaderboard
These cover shared components: buttons, icons, panels, badges, avatar frames, cards and states.

## Recommended Tooling
- Figma (preferred): components, variants, shared styles, batch export (1x/2x/3x), SVG + PNG.
- Illustrator allowed but Figma is best for component-driven handoff.

## Deliverables
### 1) Source files
- 1 Figma file (or .ai) with all screens at master canvas 1920×1080 @1x (landscape).
- Every UI element as named layers/components (not flattened).
- Style guide page: color palette, typography, spacing/grid, corner radii, shadows/glows.
- Component library page: buttons (all states), cards, badges, icons, panels.

### 2) Exported production sprites (Unity-ready)
- PNG‑24 with transparency; icons also as SVG.
- Export densities: @1x, @2x, @3x. Filenames: [screen]_[element]_[state]@[density].png
  Example: home_btn_play1v1_default@2x.png
- 9-slice ready: provide raw un‑stretched sources and suggested slice insets for panels/buttons.
- Sprite sheets optional: either deliver packed sheets (with slice map) or individual sprites—confirm packing preference with developer.

## Resolution & Scaling
- Master canvas: 1920×1080 px @1x (landscape). Provide @1x/@2x/@3x exports.
- Icons: consistent bounding boxes (e.g., 128×128 px) for uniform scaling.

## Asset Checklist (from reference screens)
- Profile avatar frame (rank star, level ring)
- XP progress bar (bg + fill)
- Coin icon & currency pill
- Top nav icons: leaderboard, daily gift, missions (+counter badges), add-coins, cart
- Mode cards: Play 1v1, Switch Player, Play with Friends, Practice (icons + distinct accents)
- Sidebar quick-access: Clubs, Shop, Avatar Store, Ranks & Badges, Settings
- Weekly Club War banner, Season pass promo card
- Social icons: Discord, Facebook, YouTube, Instagram
- Avatar Store: category sidebar icons, rarity tags (New/Hot), rarity colors (Legendary gold, Epic purple, Rare blue, Common grey), avatar card frames, preview/purchase panel
- Clubs: crest templates, flags, members, level-required badge icons (7 tiers), Join/Full/Request button states
- Leaderboard: podium frames (1/2/3), rank badges, table row template, tier legend

## Interaction States
All interactive elements require: Default, Pressed, Disabled/Locked, and Selected/Highlighted (where applicable).

## Style Reference
- Palette: charcoal/black backgrounds; primary gold/amber #F2B705; supporting blue/green/red/purple.
- Rounded rectangle cards with consistent corner radius and soft outer glow.
- Icon style: flat/duotone, slight glow, consistent stroke weight.
- Rarity color system must be consistent across store and leaderboard.

## File Naming Convention
Use: [screen]_[element]_[state]@[density].png
Examples:
- home_btn_play1v1_default@2x.png
- store_badge_legendary@3x.png

## Handoff Checklist
- Figma source + component library and style guide.
- Exported PNGs (1x/2x/3x) and SVGs for icons.
- 9-slice source images with suggested Unity slice insets.
- Sprite sheets OR individual sprites with note on preferred packing.
- Assets index (CSV/JSON) mapping asset filenames to components/usages.
- README (this file).

## Unity Import Recommendations
- Texture Type: Sprite (2D and UI)
- Compression: None or high-quality—prefer lossless for crisp UI.
- Mesh Type: Full Rect
- Filter Mode: Bilinear (or Point for pixel-style assets)
- Provide suggested Pixel Per Unit for icon sets when required.

## Developer Questions to Confirm
- Use Unity Sprite Atlas or pre-packed sheets?
- Preferred naming tweaks or extra densities?

## Licensing & Attribution
List any 3rd-party fonts, icons, or paid assets included and their licenses in the final deliverable.

---
Any edits or additions requested by the developer/designer should be added to this README and the Figma file before final handoff.
