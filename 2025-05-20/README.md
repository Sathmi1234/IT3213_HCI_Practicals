## Project Overview
- Top bar with image display
- Quick action buttons (Share, Heart/Like, Info, Delete)
- Interactive panels with slide animations
- Toggle functionality for the heart/like button
- Image position adjustment based on info panel visibility 

## Output
https://github.com/user-attachments/assets/df80db19-ca6e-47bd-ad51-5e92f230e02c

## Instructions Given

### Basic Structure
1. Create the top bar
2. Add Dynamic Panel with an image container
3. Add image to the container
4. Create a rectangle at the bottom for quick action buttons
5. Add icons (Share, Heart, Info, Delete) to the rectangle

### Share Panel
1. Create a rectangle for the share panel
2. Adjust border color and visibility
3. Add ellipse elements for share menu options
4. Create as a dynamic panel with horizontal scroll
5. Add "Share" title (heading 3)
6. Group rectangle, title, and share buttons as a dynamic panel named "share"
7. Pin to horizontal center and vertical bottom of browser
8. Set to hidden initially

### Heart/Like Button
1. Select the heart icon
2. Add a selected style effect
3. Change the fill color to red when selected

### Info Panel
1. Create a rectangle for the info panel
2. Add "Info" heading and set border properties
3. Create as a dynamic panel
4. Inside the dynamic panel, add a rectangle with info content text
5. Pin to horizontal center and vertical bottom of browser
6. Set to hidden initially

### Delete Panel
1. Create a dynamic panel for delete confirmation
2. Add two buttons:
   - Delete button (red color)
   - Cancel button
3. Set background color to transparent black
4. Pin to horizontal center and vertical bottom of browser
5. Set to hidden initially
6. Position horizontally as needed

## Interactions

### Share Button
- Click/Tap: Show share panel with slide up animation (200ms)
- Set as lightbox with semi-transparent black background
- Share panel has a close button to hide the panel

### Heart/Like Button
- Click/Tap: Toggle selected/checked state

### Info Button
- Click/Tap:
  - Show info panel with slide up animation (200ms)
  - Move image panel up by -100px with linear animation (200ms)
  - Set image panel selected state to true
- Additional interactions:
  - On swipe down (when info panel is visible):
    - Move image panel down by 100px with linear animation (200ms)
    - Hide info panel with slide down animation (200ms)
    - Set image panel selected state to false
  - Info panel has swipe down interaction that triggers the image panel swipe down event

### Delete Button
- Click/Tap: Show delete confirmation panel with slide up animation (200ms)
- Set as lightbox
- Delete confirmation panel has:
  - "Delete Photo" button: Hides the delete panel when clicked
  - "Cancel" button: Hides the delete panel

## Notes
- All animations are set to 200ms duration
- The info panel affects the position of the image panel
- Conditional logic is used to determine image panel position based on selection state
- Swipe gestures provide enhanced mobile interaction

## Files Included
- Axure source file: Day7.rp