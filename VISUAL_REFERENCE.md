# 🎨 Time Slicer - Modern UI Visual Reference

## Three-Panel Layout

```
┏━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┓
┃             ┃                                ┃                 ┃
┃  FILES      ┃      PREVIEW AREA              ┃    SETTINGS     ┃
┃             ┃                                ┃                 ┃
┃ ┌─────────┐ ┃                                ┃ [Transition]    ┃
┃ │ Files   │ ┃  ┌──────────────────────────┐  ┃ [Mask]          ┃
┃ │ List    │ ┃  │                          │  ┃ [Baking]        ┃
┃ │         │ ┃  │   Image Preview          │  ┃                 ┃
┃ │         │ ┃  │                          │  ┃ Type Selection  ┃
┃ │         │ ┃  │                          │  ┃ ○ Linear        ┃
┃ └─────────┘ ┃  │                          │  ┃ ○ Radial        ┃
┃             ┃  │                          │  ┃ ○ Grid          ┃
┃ [+ Add  ]   ┃  └──────────────────────────┘  ┃                 ┃
┃ [+ Folder]  ┃  [      Preview      ]         ┃ Angle: ___°     ┃
┃ [L][S]      ┃                                ┃ Origin X: ___   ┃
┃             ┃                                ┃ Origin Y: ___   ┃
┃ 280-350px   ┃      Flexible, Expands         ┃ 300-380px       ┃
┗━━━━━━━━━━━━━┻━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┻━━━━━━━━━━━━━━━━━┛
```

## Color Palette

### Primary Colors
```
┌─────────────────────────┐
│  #007ACC - PRIMARY BLUE │  ← Headers, buttons, focus
└─────────────────────────┘

┌─────────────────────────────┐
│  #28a745 - SUCCESS GREEN    │  ← Main action button (Slice It!)
└─────────────────────────────┘
```

### Neutral Colors
```
┌──────────────────────────┐
│  #FFFFFF - WHITE         │  ← Content panels
├──────────────────────────┤
│  #F5F5F5 - LIGHT GRAY    │  ← Background
├──────────────────────────┤
│  #DDDDDD - GRAY          │  ← Borders
├──────────────────────────┤
│  #666666 - MEDIUM GRAY   │  ← Secondary text
├──────────────────────────┤
│  #333333 - DARK GRAY     │  ← Primary text
└──────────────────────────┘
```

## Component Examples

### Button Styles

#### Primary Button
```
┌──────────────────────┐
│ + Add Files          │  Background: #007acc
│ (36px height)        │  Text: White, Bold
└──────────────────────┘
```

#### Action Button
```
┌──────────────────────┐
│ Slice It!            │  Background: #28a745
│ (40px height)        │  Text: White, Bold 700
└──────────────────────┘
```

### Tab Navigation

```
┌──────────────┬──────────┬──────────┐
│ Transition   │ Mask     │ Baking   │
└──────────────┴──────────┴──────────┘
  ↑
  Active tab (blue underline)
```

### Form Input

```
┌────────────────────────────┐
│ Linear Angle               │  Spinbox with value
│ [────────────────] 45.5°   │
└────────────────────────────┘

On Focus:
┌────────────────────────────┐
│ Linear Angle               │  Blue border
│ [════════════════] 45.5°   │
└────────────────────────────┘
```

## Typography

### Headers (14pt Bold)
```
╔═══════════════════════════════════╗
║  TRANSITION                       ║  Blue background (#007acc)
║  Configuration Controls           ║  White text
╚═══════════════════════════════════╝
```

### Labels (11pt Regular)
```
Linear Angle:     ________
Origin X:         ________  
Origin Y:         ________
```

### Buttons (11pt Bold)
```
[  Button Text  ]  32-44px height
```

## Layout Grid

```
Margin: 8px on all sides
Spacing: 8px between components

┌─────────────────────────────────┐
│ 8px                             │
│      ┌───────────────────┐      │
│      │ Content Area      │      │
│ 8px  │                   │  8px │
│      │                   │      │
│      └───────────────────┘      │
│ 8px                             │
└─────────────────────────────────┘
```

## Responsive Scaling

```
MIN WIDTH: 1400px

┌─────────┬────────────┬────────┐
│ 280px   │ ~840px     │ 300px  │
└─────────┴────────────┴────────┘

LARGER WINDOW: Center panel expands

┌─────────┬──────────────────┬────────┐
│ 280px   │ ~1000px          │ 300px  │
└─────────┴──────────────────┴────────┘

MAX WIDTHS:
├─ Left:   350px max
├─ Right:  380px max
└─ Center: Remaining space
```

## Interactive States

### Button States
```
DEFAULT
┌──────────────┐
│ Button Text  │  #007acc background
└──────────────┘

HOVER
┌──────────────┐
│ Button Text  │  #005a9e (darker)
└──────────────┘

PRESSED
┌──────────────┐
│ Button Text  │  #004578 (even darker)
└──────────────┘

DISABLED
┌──────────────┐
│ Button Text  │  Gray, semi-transparent
└──────────────┘
```

### Input Focus State
```
UNFOCUSED                  FOCUSED
┌────────────────┐        ┌════════════════┐
│ Value: 45.5    │        │ Value: 45.5    │
│ (1px gray)     │        │ (1px blue)     │
└────────────────┘        └════════════════┘
```

## Spacing Scale

```
4px   - Micro spacing (between elements)
6px   - Form field spacing
8px   - Standard spacing (panels, margins)
10px  - Section padding
12px  - Between major sections
20px+ - Large section gaps
```

## Typography Scale

```
14pt - Headers (Bold 700)
11pt - Labels, buttons, content (Regular/Bold 600)
9pt  - Helper text (optional future use)
```

## Panel Layouts

### Left Panel (Files)
```
┌────────────────────┐
│ Image Files        │  Header (14pt Bold Blue)
├────────────────────┤
│ ┌────────────────┐ │
│ │ file1.jpg      │ │  List View
│ │ file2.jpg      │ │
│ │ file3.png      │ │
│ └────────────────┘ │
│                    │
│ [+ Add Files]      │  Buttons
│ [+ Add Folder]     │
│ [Load]  [Save]     │
└────────────────────┘
```

### Center Panel (Preview)
```
┌────────────────────────────────┐
│ Preview                        │  Header
├────────────────────────────────┤
│ ┌──────────────────────────┐   │
│ │                          │   │
│ │   Image Preview Area     │   │  Graphics View
│ │   (QGraphicsView)        │   │
│ │                          │   │
│ │                          │   │
│ │                          │   │
│ └──────────────────────────┘   │
│ [       Preview Button     ]    │
└────────────────────────────────┘
```

### Right Panel (Settings with Tabs)
```
┌───────────────────────────────┐
│ [Transition] [Mask] [Baking]  │  Tab Headers
├───────────────────────────────┤
│ Type:                         │
│ ○ Linear                      │  Tab Content
│ ○ Radial                      │  (Transition shown)
│ ○ Grid                        │
│                               │
│ Angle: [──────────] 45°      │
│ Origin X: [────────] 50%     │
│ Origin Y: [────────] 50%     │
└───────────────────────────────┘
```

## Visual Hierarchy

```
HIGHEST PRIORITY
	↓
┌─────────────────────────────┐
│ [      Slice It!      ]     │  Green, 40px height
│ ╰─ Main action button       │
└─────────────────────────────┘
	↓
┌─────────────────────────────┐
│  SETTINGS SECTION           │  Blue header, clear label
│  Configuration controls     │
└─────────────────────────────┘
	↓
┌─────────────────────────────┐
│ Label: [─────────────] 45   │  Form controls
└─────────────────────────────┘
	↓
Status: Ready! (grey text)
	↓
LOWEST PRIORITY
```

## Animation & Transitions

```
Button Hover:     Color change 0.2s ease
Tab Switch:       Instant (no animation needed)
Input Focus:      Border color 0.1s ease
Progress Bar:     Smooth continuous animation
```

## Accessibility Features

```
✓ High contrast (AA compliant)
✓ Clear focus states (blue border)
✓ Logical tab order (left → center → right)
✓ Readable font sizes (11-14pt)
✓ Large touch targets (32-44px buttons)
✓ Clear labels for all inputs
```

## Design System Summary

| Element | Spec | Usage |
|---------|------|-------|
| Primary Color | #007acc | Headers, buttons |
| Action Color | #28a745 | Main action |
| Text | #333333 | Body |
| Background | #f5f5f5 | Window |
| Border | #ddd | Divisions |
| Font | 11-14pt | Standard |
| Spacing | 8px | Standard unit |
| Radius | 3-4px | Corners |
| Height | 32-44px | Buttons |

---

*Time Slicer UI - Modern, Professional, Ready to Use! 🎉*
