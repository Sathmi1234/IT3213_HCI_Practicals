# Project Overview (2025-05-30) - Tab Bar Navigation System

- Three-tab navigation with icons and labels (Home, Message, Me)
- Selection styling with yellow highlight for active states
- Inline frame for dynamic page content loading
- Selection group functionality for mutual exclusivity
- Scroll optimization with bottom whitespace handling

## Output
https://github.com/user-attachments/assets/1962ad4e-7941-400b-89bb-65369fd53761

## Instructions Given

### Basic Structure
1. Add icons with labels for each tab (Home, Message, Me)
2. Cover each tab with hotspots for interaction
3. Add inline frame for content display
4. Right-click and select toggle border for visual debugging
5. Set toggle border width slightly larger for better visibility
6. Create three sub-pages linked to main page:
   - Home page
   - Message page  
   - Me page

### Page Content Setup
7. **Home Page**: Add heading "Home" with content box
8. **Message Page**: Add avatar and thin rectangles for message bars
9. **Me Page**: [Content as needed]

## Interactions

### Tab Selection Styling
1. **Home Icon**: Add selected style effect with yellow fill color
2. **All Icons**: Repeat yellow fill selection effect
3. **Home Label**: Add selected style effect with yellow fill color  
4. **All Labels**: Repeat yellow fill selection effect
5. **Hotspot Setup**: Duplicate hotspots twice and combine with respective icons and labels

### Selection Group Configuration
6. Set selection group named "Tab" for mutual exclusivity
7. **Home Tab Interaction**:
   - Click/Tap action
   - Set selected/checked state (target: this)
   - Add next action: Open link in inline frame
   - Target: Inline frame
   - Link to: Home page
8. **Repeat Interaction**: Apply same interaction pattern to Message and Me tabs

### Frame and Content Setup
9. **Inline Frame**: Double-click and link to Home page as default
10. **Scroll Optimization**: Add hotspots at bottom of each reference page to prevent content being covered during scrolling

## Technical Details

### Tab Styling
- **Selected State**: Yellow fill color for icons and labels
- **Selection Group**: "Tab" (ensures mutual exclusivity)
- **Default Selection**: Home tab active on load

### Navigation Configuration  
- **Three Tabs**: Home, Message, Me
- **Inline Frame**: Dynamic content loading without page refresh
- **Hotspot Coverage**: Full tab area (icon + label) for better UX

### Page Structure
- **Home Page**: Heading + content box layout
- **Message Page**: Avatar + message bar elements
- **Me Page**: [Customizable content area]

## Interactive Behavior

### Tab Selection
- Only one tab can be active at a time (selection group)
- Active tab displays yellow highlight on icon and label
- Content loads dynamically in inline frame

### Content Loading
- Click any tab loads corresponding page in inline frame
- No page refresh, seamless content switching
- Maintains navigation state across content changes

### Scroll Management
- Bottom hotspots prevent content overlap
- Proper whitespace handling for scroll end
- Content remains accessible without navigation interference

## Notes
- Selection group ensures single active tab state
- Inline frame provides smooth content transitions
- Hotspot positioning critical for proper scroll behavior
- Yellow highlight provides clear visual feedback for active state
- Border toggle helpful for development and debugging