# Image Capture Guide for IR Robot README

This guide provides detailed instructions for capturing high-quality images from Altium Designer to enhance the README documentation. **Focus on schematics** for circuit understanding and **3D views** for PCB overview.

## Required Images (6 total - All Uploaded! ✅)

### 1. Main PCB 3D Render
**Filename**: `pcb_3d_render.png`
- **Source**: PCB Document (PCB1.PcbDoc)
- **View**: 3D View (press '3' key)
- **Settings**: 
  - High quality render
  - Show all components
  - Good lighting
  - Slight isometric angle to show depth
- **Resolution**: 1920x1080 or higher
- **Purpose**: Main hero image for README header

## Schematic Images (Focus Area)

### 2. STM32 Microcontroller Schematic
**Filename**: `stm32_schematic.png`
- **Source**: Main Schematic (main.SchDoc)
- **View**: Schematic Document
- **Focus**: STM32F446VET6 (U1) and surrounding support circuits
- **Include**: 
  - Crystal oscillator (8MHz)
  - Decoupling capacitors
  - Reset circuit
  - Programming header (SWD)
  - Power connections
- **Export Settings**: High resolution, show all component values

### 3. Power Management Schematic
**Filename**: `power_schematic.png`
- **Source**: Main Schematic (main.SchDoc)
- **Focus**: Complete power regulation circuit
- **Include**: 
  - LM2596S-3.3 (U4) switching regulator
  - Input protection diodes
  - Filtering capacitors (C22, C24)
  - Inductor (L1)
  - Feedback network
  - Input/output connectors
- **Purpose**: Show complete power management design

### 4. IR Communication Array Schematic
**Filename**: `ir_array_schematic.png`
- **Source**: IR Transmitter Schematic (ir_transmitter.SchDoc) + Main Schematic
- **Focus**: Complete IR communication system
- **Include**: 
  - 12x TSAL6400 IR LEDs (DS1-DS12)
  - 12x Photodiodes (D1-D12)
  - Current limiting resistors (R31-R48)
  - Driver circuits
  - Signal conditioning
- **Purpose**: Show omnidirectional IR communication design

### 5. Signal Processing Schematic
**Filename**: `amplifier_schematic.png`
- **Source**: Main Schematic (main.SchDoc)
- **Focus**: Complete signal conditioning circuits
- **Include**: 
  - LM324M op-amps (U7, U9, U10)
  - LM339 comparators (U5, U6, U8)
  - Feedback resistors and capacitors
  - Reference voltage circuits
  - Input/output connections
- **Purpose**: Show photodiode signal processing

### 6. Motor Driver Schematic
**Filename**: `motor_driver_schematic.png`
- **Source**: Main Schematic (main.SchDoc)
- **Focus**: Motor control circuits
- **Include**: 
  - TB6612FNG motor drivers (U2, U3)
  - Control signal connections from STM32
  - Power supply connections
  - Motor output connectors
  - Protection circuits
- **Purpose**: Show motor control interface design

## How to Capture Schematic Images from Altium Designer

### For Schematic Documents:
1. Open the appropriate schematic file (.SchDoc)
2. **View** → **Fit Document** to show complete schematic
3. **File** → **Export** → **Image**
4. Settings:
   - **Format**: PNG
   - **Resolution**: 300 DPI minimum
   - **Monochrome**: Unchecked (keep colors)
   - **Width**: 2400px minimum for clarity
5. Save with exact filename from list above

### For 3D PCB Views:
1. Open `PCB1.PcbDoc` in Altium Designer
2. Press **3** key or **View** → **3D Layout Mode**
3. Use mouse to adjust viewing angle:
   - **Isometric**: 45° angle for depth
   - **Top View**: Straight down for component layout
4. **File** → **Export** → **Image** from 3D view
5. Settings: PNG format, high resolution

### For Focused Schematic Sections:
1. Open main schematic (main.SchDoc)
2. Use **View** → **Zoom** → **Area** to select specific circuit section
3. **File** → **Export** → **Image**
4. Crop to show only relevant circuitry

## Image Quality Guidelines

- **Format**: PNG (lossless compression)
- **Resolution**: Minimum 2400px width for schematics
- **DPI**: 300 DPI for sharp text and component labels
- **Background**: White background for schematics
- **Text Visibility**: Ensure all component values and designators are readable

## File Naming Convention

Use exactly these filenames to match the README references:
- `pcb_3d_render.png` ✅
- `stm32_schematic.png` ✅
- `power_schematic.png` ✅
- `ir_array_schematic.png` ✅
- `amplifier_schematic.png` ✅
- `motor_driver_schematic.png` ✅

## Schematic Export Tips

1. **Component Values**: Ensure parameter text is visible
2. **Net Labels**: Include signal names for clarity
3. **Component Designators**: All U1, R1, C1, etc. should be readable
4. **Hierarchical Sheets**: Export each sheet separately if needed
5. **Color Coding**: Use colors to highlight different circuit sections

Once you've captured these images focusing on **schematics** rather than PCB sections, place them in the `images/` folder. 

## ✅ Status: All Required Images Uploaded!

Your README is now complete with all the necessary schematic diagrams! The documentation emphasizes circuit understanding through schematic diagrams while using a 3D view for PCB overview.
