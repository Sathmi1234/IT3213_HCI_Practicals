# Project Overview (2025-06-07) - Floating Action Button (FAB) Navigation System

- Multi-functional FAB with expandable options (Text, Photo, Camera)
- Dynamic panel-based page container with smooth transitions
- Conditional animation system with expand/collapse states
- Inline frame navigation with state management
- Custom UI components with styled interactions

## Output
https://github.com/user-attachments/assets/4c88cadd-4b68-44ab-b1b1-ee1cec0b5d32

## Instructions Given

### FAB Creation
1. **Main FAB Button**: Add ellipse shape with orange fill and white plus icon
2. **Text Option**: Duplicate ellipse, add pencil icon, group as "text"
3. **Photo Option**: Duplicate ellipse, add album icon, group as "photo" 
4. **Camera Option**: Duplicate ellipse, add camera icon, group as "camera"
5. **Initial State**: Hide all three option buttons and position behind main FAB

### Page Container Setup
6. **Inline Frame**: Add and send to back, convert to dynamic panel
7. **Title Bar**: Create rectangle with back button (left angle icon)
8. **Panel Configuration**: Hide border, pin to browser (center horizontal, bottom vertical)
9. **Child Pages**: Create three separate pages:
   - **Text Page**: Text field and text area with styling
   - **Photo Page**: Photo selector grid with checkboxes
   - **Camera Page**: Black viewfinder rectangle with white ellipse

### Dynamic Panel States
10. **State Management**: Configure three panel states
    - **Text State**: Links to text page
    - **Photo State**: Links to photo page  
    - **Camera State**: Links to camera page

## Interactions

### FAB Expansion Logic
**Conditional Animation System**:
- **If FAB NOT Selected** (is selected = false):
  1. Set FAB as selected/checked
  2. Move text option: Y coordinate -100px (linear 200ms)
  3. Move photo option: X -60px, Y -60px (linear 200ms)
  4. Move camera option: X coordinate -100px (linear 200ms)
  5. Show all option icons

- **Else If FAB IS Selected**:
  1. Set FAB as unselected
  2. Move text option: Y coordinate +100px (linear 200ms)
  3. Move photo option: X +60px, Y +60px (linear 200ms)
  4. Move camera option: X coordinate +100px (linear 200ms)
  5. Hide all option icons

### Option Button Interactions
**Each Option Button** (Text, Photo, Camera):
1. **Click/Tap Action**: Show dynamic panel with slide left 200ms animation
2. **Set Panel State**: Switch to corresponding state (text/photo/camera)
3. **Fire Event**: Trigger FAB click event to collapse options

### Navigation Controls
**Back Button** (in each panel state):
1. **Click/Tap Action**: Hide dynamic panel with slide right animation
2. **Consistency**: Same interaction copied across all panel states

## Technical Details

### Animation Specifications
- **Expansion Duration**: 200ms linear transitions
- **Movement Patterns**: 
  - Text: Vertical movement (±100px)
  - Photo: Diagonal movement (±60px, ±60px)
  - Camera: Horizontal movement (±100px)
- **Panel Transitions**: Slide left/right 200ms

### State Management
- **Selection Logic**: Boolean-based conditional animations
- **Panel States**: Three distinct states with unique content
- **Event Propagation**: Fire events for seamless FAB interaction

### UI Components
- **FAB Design**: Orange ellipse with white plus icon
- **Option Icons**: Pencil, Album, Camera with consistent styling
- **Panel Layout**: Title bar with back navigation
- **Content Areas**: Specialized layouts for each function

## Interactive Behavior

### FAB Expansion
- Single tap expands options in animated pattern
- Options appear with staggered positioning
- Second tap collapses all options with reverse animation

### Page Navigation  
- Option selection opens corresponding page in panel
- Smooth slide transitions between states
- Back button returns to main interface

### State Persistence
- FAB maintains selection state during navigation
- Panel states preserve content and layout
- Seamless transitions without interface disruption

### Interaction Flow
1. **FAB Click** → Conditional expansion/collapse
2. **Option Click** → Panel show + state change + FAB collapse
3. **Back Click** → Panel hide + return to main interface