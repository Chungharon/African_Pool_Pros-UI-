# Figma Setup Guide: Tournament Card Template
## Step-by-Step Instructions for Importing SVG Assets

---

## Quick Start

1. **Download all SVG files** from the `assets/svg/` folder
2. **Open your Figma file** (https://www.figma.com/design/AQBdEFtEKx1MTWdluw5PT7/)
3. **Follow the import & organization steps below**

---

## File Structure

You have the following SVG files ready to import:

```
assets/svg/
├── tournament-card-template.svg     (Complete card with all sections)
├── header-component.svg              (Level + Titles + Flag)
├── game-badge.svg                    (Game type badge)
├── difficulty-badge-rookie.svg       (Difficulty badge - Green)
├── difficulty-badge-master.svg       (Difficulty badge - Gold)
├── stars-5.svg                       (5-star rating)
├── rewards-section.svg               (Win/Entry columns)
└── FIGMA_SETUP_GUIDE.md             (This file)
```

---

## Import Steps in Figma

### Step 1: Create a New File or Use Existing
1. Open your Figma workspace
2. Create a new file called **"Tournament Card Library"** or open your existing file
3. Create a new page called **"Components"** (for reusable components)
4. Create a new page called **"Screens"** (for full card examples)

### Step 2: Import SVG Assets

#### Method A: Drag & Drop (Easiest)
1. In Figma, click on the **Screens** page
2. Open your file explorer and locate the `assets/svg/` folder
3. **Drag & drop** `tournament-card-template.svg` into your Figma canvas
4. It will import as a group/frame
5. Repeat for each SVG file (place them on separate artboards)

#### Method B: File → Import
1. In Figma, go to **File → Import**
2. Select one or all SVG files from `assets/svg/`
3. Click **Open** to import

### Step 3: Organize the Main Template

After importing **tournament-card-template.svg**:

1. **Rename it** to "Tournament Card - Main (480×640)"
2. **Lock it** (right-click → Lock) so you don't accidentally move it
3. This will be your reference frame

---

## Creating Reusable Components in Figma

### Step 4: Convert SVG Groups to Components

#### For the Header Section:
1. Import or draw the header in Figma (Level circle + Titles + Flag)
2. **Select all header elements** (level circle, both text layers, flag)
3. Right-click → **Create Component**
4. Rename to: `Header / Default`
5. In the component properties panel (right), set:
   - **Width:** 480
   - **Height:** 56

#### For the Game Badge:
1. Select the game badge group from your import
2. Right-click → **Create Component**
3. Rename to: `Game Badge / 8 Ball`
4. Set properties:
   - **Width:** 320
   - **Height:** 56

#### For Difficulty Badge (Create 5 variants):
1. **Select** the difficulty badge
2. Right-click → **Create Component**
3. Rename to: `Difficulty Badge / Rookie`
4. **Duplicate this component** 4 times:
   - `Difficulty Badge / Competitor` (change border to blue #0066FF)
   - `Difficulty Badge / Master` (change border to gold #FFB800)
   - `Difficulty Badge / Grand Master` (change border to red #FF3333)
   - `Difficulty Badge / Legend` (change border to purple #AA00FF)

#### For Star Ratings:
1. Create components for each rating:
   - `Stars / 1 Star`
   - `Stars / 2 Stars`
   - `Stars / 3 Stars`
   - `Stars / 4 Stars`
   - `Stars / 5 Stars` ← Use the imported one

#### For Rewards Section:
1. Select the rewards section group
2. Right-click → **Create Component**
3. Rename to: `Rewards / Default`
4. Set properties:
   - **Width:** 448
   - **Height:** 80

#### For Footer:
1. Create a new component (level indicator + "186 Playing" text)
2. Name it: `Footer / Player Count`
3. Set properties:
   - **Width:** 448
   - **Height:** 32

---

## Step 5: Set Up Component Variants

### Using Figma's Variant System (Recommended for Figma Professional+)

1. **Select all badge difficulty components** (Rookie, Competitor, Master, Grand Master, Legend)
2. Right-click → **Combine as variants**
3. This creates a single **Difficulty Badge** component with variants you can toggle:
   - **Level:** Rookie / Competitor / Master / Grand Master / Legend

### Repeat for:
- **Stars:** Level = 1 / 2 / 3 / 4 / 5
- **Game Badge:** Game Type = 8 Ball / 9 Ball / Snooker / Carom
- **Header:** Region = Lagos / Cairo / Johannesburg / Accra / etc.

---

## Step 6: Create the Full Card Component

### Assemble the Main Card:
1. Create a new frame (480 × 640)
2. Rename it: `Tournament Card / Master`
3. **Add these elements in order (from top to bottom):**
   - **Background:** Rectangle (480×640, rounded 24px, border 3px gold, gradient fill)
   - **Header Component:** Drag in the Header component
   - **Background Image:** Rectangle placeholder (448×252, rounded 16px)
   - **Game Badge Component:** Insert the Game Badge component
   - **Rewards Section Component:** Insert the Rewards component
   - **Stars Component:** Insert Stars component
   - **Difficulty Badge Component:** Insert Difficulty Badge component (set to "Master")
   - **Footer Component:** Insert Footer component

### Make it a Component:
1. **Right-click** on the assembled frame → **Create Component**
2. Name it: `Card / Tournament / Master`
3. This is now your main reusable component!

---

## Step 7: Create Variants of the Main Card

### Using Component Variants:
1. **Duplicate** the `Card / Tournament / Master` component 4 times
2. Rename them:
   - `Card / Tournament / Rookie`
   - `Card / Tournament / Competitor`
   - `Card / Tournament / Master`
   - `Card / Tournament / Grand Master`
   - `Card / Tournament / Legend`

3. In each one, **change only the Difficulty Badge component** to match the level

4. **Select all 5 card variants** and **Combine as variants**
5. Create a **Difficulty** property with options: Rookie / Competitor / Master / Grand Master / Legend

### Optional: Add More Variants
- **Region:** Lagos / Cairo / Johannesburg / Accra
- **Game:** 8 Ball / 9 Ball / Snooker / Carom
- **Stars:** 1 / 2 / 3 / 4 / 5

---

## Step 8: Create a Design System Page

### Create a "Design System" page with:

#### Colors Section
Create color swatches for:
- Primary Gold: #F2B705
- Background Dark: #0a0e27
- Rookie Green: #00AA44
- Competitor Blue: #0066FF
- Master Gold: #FFB800
- Grand Master Red: #FF3333
- Legend Purple: #AA00FF
- White: #FFFFFF

#### Typography Section
Document your type scale:
- **Display:** Montserrat 48px / 700 (primary titles)
- **Heading 1:** Montserrat 28px / 700 (level number)
- **Heading 2:** Montserrat 20px / 600 (secondary titles)
- **Body Large:** Montserrat 18px / 700 (amounts)
- **Body:** Montserrat 14px / 700 (labels)
- **Caption:** Montserrat 12px / 600 (small text)

#### Component Library Section
Screenshot each main component variant for quick reference

---

## Step 9: Create Example Screens

### Create screens showing real-world usage:

1. **Clubs Screen**
   - Use the Tournament Card component (Master difficulty)
   - Place 3-4 cards in a grid
   - Add header, back button, filters above

2. **Leaderboard Screen**
   - Use Tournament Card component variants
   - Show cards at different difficulties
   - Add sorting/filtering UI

3. **Tournament Details**
   - Full card (Master variant)
   - Add join button, description, rules below
   - Show related tournaments

---

## Step 10: Share & Export

### For Team Collaboration:
1. Go to **Share** (top right)
2. Set permission to **Edit** for your design team
3. Copy the link and share in Slack/Discord

### For Developer Handoff:
1. Select all components
2. Go to **Assets panel** (right sidebar)
3. Click **Publish to library** (library icon)
4. Name it: "African Pool Pros - Tournament Cards"
5. **Copy the link** and share with developers

### Export for Mobile:
1. Select components you want to export
2. Right-click → **Export** (or use the export panel)
3. Format: **PNG (for Sprite) + SVG (for vector)**
4. Densities: 1x, 2x, 3x

---

## File Organization Best Practices

### Figma File Structure (Recommended):

```
Tournament Card Library
│
├── 📄 Design System
│   ├── Colors
│   ├── Typography
│   ├── Icons & Assets
│   └── Effects (Shadows, Glows, Gradients)
│
├── 📄 Components
│   ├── Header
│   ├── Game Badge
│   ├── Difficulty Badge (Variants: 5 levels)
│   ├── Stars (Variants: 1-5)
│   ├── Rewards Section
│   ├── Footer
│   └── Card / Tournament (Master component with variants)
│
├── 📄 Screens
│   ├── Clubs Screen
│   ├── Leaderboard Screen
│   ├── Tournament Details
│   └── Home Screen
│
├── 📄 Icons & Assets
│   ├── 8 Ball Icon
│   ├── Coin Icon
│   ├── Flag Icons (Nigeria, Egypt, South Africa, Ghana, etc.)
│   └── Level Badge Icons
│
└── 📄 Archive (Deprecated, Drafts)
    └── Old versions
```

---

## Naming Convention for Components

Use this format for consistency:

```
[Category] / [Component Name] / [Variant]

Examples:
- Header / Level Indicator / Gold
- Badge / Game / 8 Ball
- Badge / Difficulty / Master
- Badge / Difficulty / Rookie
- Stars / Rating / 5 Stars
- Card / Tournament / Master
- Card / Tournament / Rookie
- Section / Rewards / Default
- Footer / Player Count / Default
```

---

## Customization Checklist

Before handing off to developers, ensure:

- [ ] All components are organized in folders
- [ ] Component naming follows convention
- [ ] Variants are created for all interactive states
- [ ] Color palette is documented and linked to components
- [ ] Typography is applied consistently (use text styles)
- [ ] All icons are at the right size (128×128, 48×48, etc.)
- [ ] Spacing follows 8px grid
- [ ] Corner radii are consistent (24px cards, 12px badges, etc.)
- [ ] Shadows and glows are applied
- [ ] Exported assets (PNG/SVG) match Figma components
- [ ] Component library is published
- [ ] Developer link/access is shared

---

## Quick Customization Examples

### To Create "Cairo" Tournament Card:
1. Duplicate the **Card / Tournament / Master** component
2. In the **Header component**, change:
   - Primary title: CAIRO
   - Secondary title: EGYPT
   - Flag: Egyptian flag (SVG)
3. Change background image (Cairo skyline)
4. Done! ✓

### To Add a New Game Type (9 Ball):
1. Duplicate **Game Badge / 8 Ball** component
2. Change icon from 8 to 9
3. Change text to: "9 BALL ROTATION"
4. Rename to: **Game Badge / 9 Ball**
5. Update card variants to include this option

### To Change Difficulty Colors:
1. Select **Difficulty Badge / Master** component
2. Change **border color** from gold (#FFB800) to your chosen color
3. Update all variants the same way
4. Export new PNG assets

---

## Next Steps

1. ✅ Import all SVG files into Figma
2. ✅ Convert groups to components
3. ✅ Create component variants
4. ✅ Organize into pages and folders
5. ✅ Test each variant by clicking through
6. ✅ Publish to team library
7. ✅ Share link with developers
8. ✅ Export final assets (PNG 1x/2x/3x + SVG)
9. ✅ Create Figma handoff document
10. ✅ Meet with development team to confirm Unity import settings

---

## Support & Questions

- **Component not showing?** Check that layers are properly named and grouped
- **Variant not working?** Ensure you're using Figma Professional+ (required for variants)
- **Text not rendering?** Ensure Montserrat font is installed or use Figma's fallback
- **Export quality?** Set PNG to "4x" for maximum clarity, then rename to @2x, @3x

---

**Happy designing! 🎨**
