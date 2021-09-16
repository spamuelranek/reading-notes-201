# LINK listen, FUNKtions, CSS payout in the Layout

## Hey Listen!
- a link
  - it takes you somewhere else
- `<a href ="google.com">The Search Engine</a>`
  - `<a>` is the tag used
  - `href` defines the where you are goint
  - `="google.com"` tells the path to get there.
    - this can also be a file path
  - `The Search Engine` becomes the clickable link
- Linking to a specific part of the same page
    - you can target ids of tags elsewhere in the document
    -`<a href="#arc_shot"> and <h2 id="arc_shot">`

## The layout that gets the payout
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

## FunkTronics
- Functions are the doing
  - `function sayHello() { document.write("woooo")}`
  - `function` is the keyword or "declarer"
  - `sayHello` is the name
  - `()` states the function 
  - `{document.write("woooo")}`is what it actually is telling the computer what to do
    - To invoke or call `function()`
- Parameters
  - Information that needs to be given to the to the function
  ``` js
  function getArea(width,height) {
      return width * height;  
  }
  ```
- Multiple values from a function...it makes an array
  ```js
  function getsize(width, height, depht) {
      var area = width * depht;
      var volume = width * depht *height;
      var surfaceArea = (width * depht * 2) + (width * height * 2) + (depht * height *2);
      var total = [area, volume, surfaceArea];
      return total;
  }
  ```
- Anonymous and Declared
 - Declared is form of function above
 - Anonymous
    ``` js
    var area = function(w,h){
        return = w * h;
    }
    ```
    - This is know as a function expression

## Peer Programing
- Driver and Navigator
  - Driver
    - The one doing the typing
    - Brain off to the big things
  - Navigator
    - Doing the big pictiure thinking
    - Helping identify mistakes
- Benefits
  - Greater Efficiency
    - Not time faster first time through, but higher quality code
    - Engaged Collaboration
      - Easier time to be engaged for the time needed
    - Learning from fellow students
      - Help you see solutions in new ways
    - Social Skills
      - Being able to communicate in the vernacular clearly is a invaluable skill
    - Job readiness
      - Both in interview settings and work enviroment, employers will be looking to see how you manage this skill
[Knowledge Base](README.md)