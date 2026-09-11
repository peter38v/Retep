---
id: kicad-design-blocks
aliases:
  - kicad-design-blocks
tags: []
---
# Kicad Design Blocks how to

## What is design block?
Design blocks are reusable schematic+pcb configuration.
Imagine reusing code, just for schematic design

## How to make?
1. Make Schematic (in new project)
2. Click View->Panels->Design Blocks (Opens side panel)
3. (FIRST TIMER) Right Click in the panel->Create New library
    3a. Choose Project vs Global
    3b. Give it a name -> Save it as a .kicad_blocks file
    3c. (OPTIONAL) Add description to library
4. Select Library in right-side panel by clicking on it
5. Select the schematic in Kicad (left mouse-click drag a rectangle around it)
6. Right click on Library in panel -> Save Selection as Design Block
7. In pop-up window (Design Block Properties) -> give it name, OPTIONAL: keywords,description
8. Press "Okay" -> you gucci

## How to group in PCB
1. Place all components in desired layout (including edge cuts)
2. Select Grouping -> Right click -> save link to design block
Tada
3. If it does not allow option, group everything -> go to the right side panel and right click there to update it
## How to load
1. Open design-blocks in side panel (PCB making)
2. Drag it in
Tada
