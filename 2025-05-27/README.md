# Project Overview (2025-05-27) - Button Selection System
- Two toggle buttons (Monthly/Yearly) with selection styling
- Dynamic panel with scrollable content states
- Selection group functionality for mutual exclusivity
- Vertical scrolling with proper whitespace handling

## Output
https://github.com/user-attachments/assets/7e6ca2f1-9e4c-4c54-93de-292279f3daae

## Instructions Given

### Basic Structure
1. Create two buttons using rectangles (Monthly, Yearly)
2. Add selected style effect for the monthly button (fill color - blue, font color - white) and change border width to 0
3. Copy and paste the style to the other button
4. Set the first button to default selected state
5. Set the selection group for both buttons as group 1
6. Add a dynamic panel
7. Inside the panel (in state one) create sections
8. Set the panel to scroll vertically
9. In state two create another section
10. Rename the states as:
    - Monthly
    - Yearly

## Interactions

### Monthly Button
- Click/Tap:
  - Set selected/checked state for the first button
  - Set panel state to "Monthly"

### Yearly Button  
- Click/Tap:
  - Set selected/checked state for the second button
  - Set panel state to "Yearly"

### Additional Elements
- Add hotspot at the bottom of the scrollable area to provide whitespace when scrolling content

## Technical Details

### Button Styling
- Selected state: Blue fill, white text, no border
- Selection group: Group 1 (ensures mutual exclusivity)
- Default selection: Monthly button

### Dynamic Panel Configuration
- Two states: "Monthly" and "Yearly"
- Vertical scrolling enabled
- Content sections within each state
- Bottom whitespace hotspot for scroll padding

## Notes
- Selection group ensures only one button can be active at a time
- Panel content changes dynamically based on button selection
- Vertical scrolling accommodates varying content lengths
- Hotspot provides proper scroll ending experience

## Files Included
- Axure source file with interactive button selection system