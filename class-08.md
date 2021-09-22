# Layout Flayout
## Learn all the BASICS!

### [previous reading](class-04.md)

### Controlling Position of Elements

- Normal Flow
  - Default Behavior
  - Each piece appears on the next line 
- Relative Positioning
  - Moves targeted elements relative to the page
  - Does not affect other elements
- Absolute Positioning
  - Positions the element in relation to its containing element.
  - once postioned this way, the elements will move as a user scrolls up and down
- Fixed positioning
  - It is like absolute positioning but doesm't move when user scrolls
- Floating Elements
  - Allows to move an item to the far left or right of the containing box

### Fixed vs Liquid

- Fixed - uses absolute measruements
  - Advantages
  - Increases Design Control
  - Always looks exactly as designed
  - Disadvantages
  - May not fit different screens
  - May have a lot of space not filled
- Liquid - uses relative measurements
  - Advantages
  - Windows will flex to space
  - Disadvantages
  - Without additional control elements can move to weird places

#### Additional Terms
- z-index - identfies which element should be "on top" of others
- float - moves items within their box
- clear - states should not touch any other elements inside the same containing element

### Layout Grids
- CSS Frameworks
  - 960.GS
  - Downloadable style shet
    - comes with predesigned bins
    - keeps you from writing code for the same tasks
  - Multiple Style Sheets
    - `@import url("tables.css")` - happens on the CSS page
    - `<link rel = "stylsheet" href = "stylesheet.css" type ="text/css">` - happens on the HTML page
