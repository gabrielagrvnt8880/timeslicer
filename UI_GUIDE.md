# Time Slicer - Modern UI Guide

## Layout Overview

```
┌─────────────────────────────────────────────────────────────────┐
│                    Time Slicer - Image Slicing Tool              │
├────────────┬──────────────────────────┬──────────────────────────┤
│  FILES     │                          │  SETTINGS                │
│ ─────────  │                          │ ──────────               │
│ List View  │                          │ ┌─ Transition ─┐        │
│ (Images)   │    PREVIEW AREA          │ │ ┌─────────┐  │        │
│            │   (Graphics View)        │ │ │ Type    │  │        │
│            │                          │ │ ├─────────┤  │        │
│ + Add File │                          │ │ │ Linear  │  │        │
│ + Add Fold │                          │ │ │ Radial  │  │        │
│ [Load][Sav]│                          │ │ │ Grid    │  │        │
│            │    [   Preview   ]       │ │ └─────────┘  │        │
│            │                          │ │             │        │
│            │                          │ ├─────────────┤        │
│            │                          │ │ Angle: [__] │        │
│            │                          │ │ Origin X...│        │
│            │                          │ └─────────────┘        │
│            │                          │ ┌─ Mask ──────┐        │
│            │                          │ │ Blend: [__] │        │
│            │                          │ │ Shadow: ...│        │
│            │                          │ └─────────────┘        │
│            │                          │ ┌─ Baking ────┐        │
│            │                          │ │ Output...   │        │
│            │                          │ │ Quality: 90%│        │
│            │                          │ │             │        │
│            │                          │ │ [SLICE IT!] │        │
│            │                          │ │ Ready!      │        │
│            │                          │ │ Progress: █│        │
│            │                          │ └─────────────┘        │
└────────────┴──────────────────────────┴──────────────────────────┘
│ TimeSlice 0.1                                                    │
└────────────────────────────────────────────────────────────────────┘
```

## Panel Descriptions

### Left Panel: Image Management
- **Header**: "Image Files" (blue background)
- **Content**: Scrollable list of loaded images
- **Controls**:
  - "+ Add Files" - Opens file dialog to select individual images
  - "+ Add Folder" - Opens folder dialog to bulk import images
  - "Load" / "Save" - Project management buttons

### Center Panel: Preview
- **Header**: "Preview" (blue background)
- **Content**: Large graphics view for image preview
- **Control**: "Preview" button to refresh preview based on current settings

### Right Panel: Settings (Tabbed Interface)

#### Tab 1: Transition
Configure how images transition between each other:
- **Type Selection**: Linear, Radial, or Grid
- **Linear Settings**: Angle adjustment (0-90°)
- **Radial Settings**: Origin point (X, Y), Sweep angle, Start angle
- **Grid Settings**: Number of rows
- **Options**: Reverse order checkbox

#### Tab 2: Mask
Configure masking and blending:
- **Blending Factor**: 0 (soft edges) to 1 (hard edges)
- **Drop Shadow**: None, Forward, or Backward with alpha control
- **Scaling**: X and Y scale factors
- **Preview Button**: Update preview with current mask settings

#### Tab 3: Baking
Configure output and render:
- **Output Folder**: Destination for sliced images
- **Output Type**: JPEG or TIFF format
- **Quality**: Compression quality (0-100%)
- **Options**: Output intermediate masked slices
- **Main Button**: Large green "Slice It!" button to start processing
- **Status**: Real-time info and progress bar

## Color Scheme

| Element | Color | Use |
|---------|-------|-----|
| Headers | #007acc (Blue) | Section titles, branding |
| Action Button | #007acc (Blue) | Secondary actions |
| Success Button | #28a745 (Green) | Main action "Slice It!" |
| Background | #f5f5f5 (Light Gray) | Window background |
| Panels | White | Content areas |
| Borders | #ddd (Light Gray) | Subtle divisions |
| Text | #333 (Dark Gray) | Body text |

## Workflow

### Basic Usage
1. **Load Images**
   - Click "+ Add Files" or "+ Add Folder"
   - Select images to process

2. **Configure Transition**
   - Choose transition type (Linear/Radial/Grid)
   - Adjust relevant parameters
   - Click "Preview" to see effect

3. **Configure Mask** (Optional)
   - Adjust blending and shadow settings
   - Preview changes

4. **Configure Output**
   - Set output folder
   - Choose format and quality
   - Select output options

5. **Process**
   - Click "Slice It!"
   - Monitor progress bar
   - Check status messages

### Advanced Features

**Project Management:**
- Save current setup with "Save" button
- Load previous projects with "Load" button

**Live Preview:**
- Toggle between different transition types
- Immediately see preview updates
- Fine-tune parameters before processing

**Batch Processing:**
- Add multiple images
- Configure once
- Process all at once with a single click

## Responsive Design

The layout adapts to different window sizes:
- **Minimum width**: 1400px for optimal viewing
- **Minimum height**: 900px
- Left/right panels have fixed min/max widths
- Center panel expands/contracts with window
- All panels are scrollable if needed

## Keyboard Shortcuts (Future Enhancement)
Could be added:
- Ctrl+O: Open files
- Ctrl+S: Save project
- Ctrl+L: Load project
- Ctrl+E: Execute slice
- Space: Preview
