# African Pool Pros — Tournament Card UI Template

## Overview
Reusable template structure for tournament/challenge cards in African Pool Pros. Designers can customize content, colors, and backgrounds while maintaining consistent layout and branding.

---

## Card Anatomy & Layout Structure

### Canvas Size
- **Width:** 480 px (mobile card)
- **Height:** 640 px (portrait)
- **Corner Radius:** 24 px (all corners)
- **Border:** 3 px solid gold/amber (#F2B705) with outer glow

### Layout Grid (8px baseline)
```
[Card Padding: 16px on all sides]

+--------Header Section (56px)--------+
| Level Icon (L)  |  Title  | Flag (R) |
+---[Background Image Area (280px)]--+
| (City/Landmark imagery)             |
+------Game Badge Section (60px)------+
| [Game Type Badge - Centered]        |
+----Rewards Section (80px)------+
| WIN              |    ENTRY         |
| [Icon] [Amount]  | [Icon] [Amount]  |
+--------Divider Line--------+
| [Rating Stars - Centered]   |
+----Difficulty Bar (40px)----+
| [Difficulty Badge]          |
+---Footer Section (32px)-----+
| [Player Count Icon] # Playing|
+-----------------------------+
```

---

## Component Breakdown

### 1. **Header Section (56px)**
Location: Top of card, 16px padding

#### Level Indicator (Left)
- **Size:** 48 x 48 px circle
- **Border:** 2 px gold (#F2B705)
- **Background:** Dark transparent with slight glow
- **Content:** White bold number (font-size: 28px, weight: 700)
- **Spacing from edge:** 16 px
- **Example values:** 1–20 (tournament difficulty)

#### Title Group (Center)
- **Primary title:** Large bold sans-serif (font-size: 48px, weight: 700, color: white)
- **Secondary title:** Medium sans-serif (font-size: 24px, weight: 600, color: gold #F2B705)
- **Layout:** Stacked, centered
- **Max width:** 250 px
- **Examples:**
  - LAGOS / NIGERIA
  - CAIRO / EGYPT
  - JOHANNESBURG / SOUTH AFRICA

#### Country Flag (Right)
- **Size:** 48 x 48 px circle
- **Border:** 2 px gold (#F2B705)
- **Content:** Country flag (circular crop)
- **Spacing from edge:** 16 px
- **Alternatives:** Flag SVG, regional emblem, or country crest

---

### 2. **Background Image Area (280px)**
Location: Center-top, full card width minus padding

#### Image Specs
- **Aspect Ratio:** 16:9 (approx 448 x 252 px with padding)
- **Content:** City skylines, landmarks, regional imagery
- **Overlay:** 30% dark gradient overlay (top-to-bottom) to ensure text readability
- **Border Radius:** 16 px
- **Examples:**
  - Lagos skyline (Lekki Ikoyi Bridge)
  - Cairo cityscape (Nile, pyramids)
  - Johannesburg (Skyline)
  - Accra (Independence Square)

#### Optional Badge Overlay
- Small "AFRICAN TOUR" or event name badge
- Placed center-top of image
- Style: Hexagonal or chevron-shaped border, gold text on dark background
- Font-size: 12 px, weight: 700

---

### 3. **Game Badge Section (60px)**
Location: Below image, centered

#### Main Game Badge
- **Shape:** Rounded rectangle with side wings/chevrons (hexagon-like)
- **Size:** 320 x 56 px
- **Border:** 2 px gold (#F2B705)
- **Background:** Dark (transparent or very dark navy)
- **Glow:** Soft outer glow (gold, 8px blur)

#### Badge Content (Centered)
- **Left Icon:** Game symbol (e.g., 8-ball icon, billiard symbol) – 32 x 32 px
- **Text:** Game type & mode name (e.g., "8 BALL CALL POCKET")
  - Font-size: 20 px, weight: 700, color: gold
  - Subtitle (optional): 12 px, weight: 600, color: white, below main text
- **Spacing:** 12 px between icon and text

#### Badge Variants (by game type)
- **8 Ball:** 8-ball icon, gold accents
- **9 Ball:** 9-ball icon, purple/blue accents
- **Snooker:** Snooker ball icon, red accents
- **Carom:** Carom ball icon, cyan accents

---

### 4. **Rewards Section (80px)**
Location: Below game badge, split 2-column layout

#### Column Layout
- **Width:** 210 px each (with 8 px divider in center)
- **Height:** 80 px
- **Background:** Transparent with subtle border accent
- **Border:** 1 px gold, bottom only (light separator)

#### Left Column — "WIN" Reward
- **Label:** "WIN" (font-size: 14 px, weight: 700, color: white, ALL CAPS)
- **Icon:** Coin stack (32 x 32 px, gold)
- **Amount:** Large bold number (font-size: 40 px, weight: 800, color: white)
- **Suffix:** Currency symbol or text (optional, 16 px)
- **Layout:** Icon left (12 px margin), amount right-aligned
- **Examples:** 3000, 5000, 10000

#### Right Column — "ENTRY" Cost
- **Label:** "ENTRY" (font-size: 14 px, weight: 700, color: white, ALL CAPS)
- **Icon:** Coin with dollar symbol (32 x 32 px, gold)
- **Amount:** Large bold number (font-size: 40 px, weight: 800, color: white)
- **Layout:** Icon left (12 px margin), amount right-aligned
- **Examples:** 500, 1500, 2500

#### Center Divider
- **Style:** Vertical line, 1 px, gold (#F2B705), height 50 px, centered
- **Optional glow:** Slight vertical glow effect

---

### 5. **Rating/Difficulty Indicator (40px)**
Location: Below rewards, centered

#### Rating Stars
- **Count:** 5 stars
- **Size:** 24 x 24 px each
- **Color:** Gold (#F2B705)
- **Spacing:** 4 px between stars
- **Style:** Solid filled, or gradient with inner glow
- **Alternative:** Half-stars (0.5 increments) for partial ratings
- **Placement:** Horizontally centered

#### Star Rating Meaning
- 1–2 stars: Beginner / Rookie level
- 3 stars: Intermediate / Competitor level
- 4 stars: Advanced / Master level
- 5 stars: Expert / Grand Master level

---

### 6. **Difficulty Badge Section (40px)**
Location: Below rating, centered

#### Badge Container
- **Shape:** Rounded rectangle with side chevrons (similar to game badge)
- **Size:** 280 x 40 px
- **Border:** 1.5 px colored (by difficulty tier)
- **Background:** Very dark or transparent
- **Padding:** 8 px

#### Difficulty Levels & Colors
| Level | Color | Border Color | Text Color |
|-------|-------|--------------|-----------|
| Rookie | Green | #00AA44 | White |
| Competitor | Blue | #0066FF | White |
| Master | Orange/Gold | #FFB800 | White |
| Grand Master | Red | #FF3333 | White |
| Legend | Purple | #AA00FF | White |

#### Badge Text
- **Font-size:** 16 px, weight: 700, ALL CAPS
- **Example:** "MASTER LEVEL", "VETERAN", "PRO"
- **Optional subtitle:** Rank or tier name (12 px, weight: 600, below main text)

---

### 7. **Footer Section (32px)**
Location: Bottom of card

#### Player Count
- **Icon:** Group/people silhouette icon (20 x 20 px)
- **Text:** Number of players (font-size: 18 px, weight: 700, color: white)
- **Suffix:** "Playing" or "Joined" (font-size: 12 px, weight: 600, color: gold)
- **Layout:** Icon left (12 px margin), text right
- **Examples:** "186 Playing", "1250 Joined"
- **Alignment:** Left-aligned, 16 px from edge

---

## Color Palette (Standard)

### Primary Colors
- **Primary Gold:** #F2B705
- **Background Dark:** #0a0e27
- **Border Dark:** #1a1f3a

### Tier/Difficulty Colors
- **Rookie Green:** #00AA44
- **Competitor Blue:** #0066FF
- **Master Gold:** #FFB800
- **Grand Master Red:** #FF3333
- **Legend Purple:** #AA00FF

### Utility Colors
- **White (Text):** #FFFFFF
- **Dark Gray (Secondary):** #999999
- **Glow Shadow:** rgba(242, 183, 5, 0.3)

---

## Typography

### Font Stack (Recommended)
- **Primary Font:** Montserrat, Roboto, or similar sans-serif (bold, geometric)
- **Secondary Font:** Inter or Open Sans (clean, readable)
- **Fallback:** System font (Helvetica Neue, Arial)

### Font Weights Used
- **700 (Bold):** Headers, numbers, badges
- **600 (Semi-Bold):** Sub-labels, subtitles
- **400 (Regular):** Body text (if any)

### Font Sizes (px)
| Element | Size | Weight |
|---------|------|--------|
| Level number | 28 | 700 |
| Primary title | 48 | 700 |
| Secondary title | 24 | 600 |
| Game badge text | 20 | 700 |
| Reward label | 14 | 700 |
| Reward amount | 40 | 800 |
| Difficulty badge | 16 | 700 |
| Footer text | 18 | 700 |

---

## Effects & Styling

### Borders & Glows
- **Main card border:** 3 px gold, outer glow (8px blur, 40% opacity)
- **Badge borders:** 2 px gold, softer glow (4px blur, 30% opacity)
- **Divider lines:** 1 px gold with slight vertical glow effect

### Shadows & Depth
- **Card shadow:** Drop shadow (offset 0, blur 16px, y-offset 8px, black 20% opacity)
- **Image shadow:** Subtle inner shadow (top-to-bottom dark gradient, 30% opacity)

### Gradients
- **Card background:** Subtle gradient (dark blue to darker blue, top to bottom)
- **Image overlay:** Dark gradient (transparent to black, 0–100%, top to bottom)
- **Star icons:** Optional subtle gradient (white to gold, creates 3D effect)

### Interactive States
- **Hover:** Card brightens slightly (5% opacity increase), scale up 2%
- **Pressed:** Card dims (10% opacity decrease), scale down 1%
- **Disabled:** 50% opacity, desaturate colors

---

## Customization Guide for Designers

### How to Adapt This Template

#### Change Tournament Theme
1. Replace background image (maintains 16:9 aspect ratio)
2. Update primary title (city/region name)
3. Update secondary title (country name)
4. Replace flag with country flag SVG
5. Update level indicator number if needed

#### Change Game Type
1. Replace game badge icon (8-ball → 9-ball, etc.)
2. Update game badge text
3. Consider secondary color scheme if desired
4. Adjust difficulty colors if tier changes

#### Change Rewards
1. Update "WIN" amount number
2. Update "ENTRY" cost number
3. Adjust coin icon style if needed (gold to silver, etc.)

#### Change Difficulty/Rating
1. Update star count (0–5)
2. Update difficulty badge color and text
3. Update difficulty level label

#### Change Player Count
1. Update player count number
2. Adjust footer text ("Playing", "Joined", "Registered", etc.)

---

## Export & Asset Checklist (Designer to Developer)

### Required Assets
- [ ] Card main background image (1x, 2x, 3x densities)
- [ ] Level indicator frame (SVG/PNG)
- [ ] Country flag (SVG or PNG circle crop)
- [ ] Game badge background (9-slice or vector)
- [ ] Game icon (8-ball, 9-ball, etc.) – SVG preferred
- [ ] Coin/reward icon (SVG)
- [ ] Currency icon ($ or ₦) – SVG
- [ ] Star icons (filled, half, empty) – SVG
- [ ] Difficulty badge background (9-slice or vector)
- [ ] Player group icon – SVG
- [ ] All divider lines/separators (SVG)

### File Naming Convention
```
tournament_card_[element]_[state]@[density].png
Examples:
- tournament_card_bg_lagos@2x.png
- tournament_card_game_badge_8ball@2x.png
- tournament_card_stars_5@1x.png
- tournament_card_difficulty_master@2x.png
```

### Figma Component Structure
```
Tournament Card (Main Component)
├── Header
│   ├── Level Indicator
│   ├── Title (Primary)
│   ├── Title (Secondary)
│   └── Country Flag
├── Background Image
│   └── Overlay Gradient
├── Game Badge
│   ├── Icon
│   └── Text
├── Rewards Section
│   ├── Win Column
│   └── Entry Column
├── Stars
├── Difficulty Badge
└── Footer
    └── Player Count
```

### Variants to Create (in Figma)
- **By difficulty:** Rookie / Competitor / Master / Grand Master / Legend
- **By game type:** 8 Ball / 9 Ball / Snooker / Carom
- **By region:** Lagos / Cairo / Johannesburg / Accra / etc.
- **By state:** Default / Hover / Pressed / Disabled
- **By rating:** 1–5 stars

---

## Implementation Notes for Unity Developers

### Canvas/Panel Setup
- Use Canvas with Graphic Raycaster for interactions
- Card as Image component with custom Material (for glow effect)
- Content nested with Layout Group (Vertical Layout Group)

### Sprite Settings
- Texture Type: Sprite (2D and UI)
- Mesh Type: Full Rect
- Pivot: Center
- Compression: None (crisp borders and text)

### 9-Slice Setup (for scalable elements)
- Game badge background: Slice insets [16, 8, 16, 8] px
- Difficulty badge background: Slice insets [12, 6, 12, 6] px
- Divider lines: Use simple line Sprites with Stretch layout

### Button Interaction
- Attach Button component to card
- Transition: Color Tint or Animation
- On Click: Open tournament details or join flow

### Dynamic Text Updates
- Title: TextMeshProUGUI with auto-sizing
- Amounts: Format as currency (e.g., 1500 → "1,500" or "₦1.5K")
- Star count: Instantiate 0–5 star Sprites based on rating

---

## Design Best Practices

1. **Consistency:** Always maintain the 24px corner radius and 3px border.
2. **Legibility:** Ensure text contrast is minimum 4.5:1 over any background.
3. **Icon Simplicity:** Keep icons flat and bold; avoid overly complex details.
4. **Spacing:** Use multiples of 8px for all padding and margins.
5. **Color Meaning:** Use consistent difficulty colors across all screens.
6. **Accessibility:** Provide alt text for flag icons and meaningful labels for icons.
7. **Testing:** Preview on 1x, 2x, 3x densities before handoff.

---

## Version & Updates

- **Version:** 1.0
- **Last Updated:** 2026-07-24
- **Maintained by:** Design System Team

---

## Questions & Support

For questions on customization, reach out to the design lead or refer to the main **README.md** for Figma file location and contact details.
