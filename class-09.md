# FORMS and _______ (JS Events)

## Forms(p.144-175)

- Why use forms
  - Allows for information to be generated from users

- Forms generate key value pairs that are sent to a server and then the server seens a message backe

- Various forms come pre-built by HTML tag

## Forms cont.(p.330-357)

- Lists have some style choices:
  - settting the dot inside or outside the text
  - changing the dot indication
  - changing it to an icon

- Tables
  - Using a `<thead>` tag makes it easier to target the top row
  - Using a `<tfoot>` tag makes it easier to target the bottom row
  - A few ways to make the data easier to read:
    - `padding`
    - `boarder-spacing` which puts space each cell
    - `font-size` can make the data larger in size

- Once you have chosen the form that best suits your purposes
  - There is many ways to style them
  - Styled forms have the benefit of feeling better to fill out

## Events (like a party?) (p.243-292)

- Events
  - Interactions from the user start events
    - `click`
    - `load`
    - `keypress`
  - These interactions then 'trigger' events
    - different actions can start because of this
  - Code becomes interactive
    - events can be used to modify the DOM so the page can be responsive to the user

- Events Handling
  - Identify the element Node you want to respond to
  - Indicate what will trigger the event eg `click, mouseclick`
    - also called binding
  - state the code you would like to run

- Binding event to Element
  - HTML event handlers
    - not reccomended for new code
    - used in the past
    - `<onclick>`
  - Traditional DOM Handlers
    - allow to separate HTML from JS unlike HTML event handlers
    - can only attach a single funtion to an event
    - `element.onevent = functionName;`
      1. Funtion that will be targeted
      2. Locate node
      3. ` elementNode.onblur = Function` and no parentheses on the function  
    - Event Listeners
        - SYntax is quite different
        - allows for several functions to be binned to single event
        - Takes three parts
        - `element.addEventListener('event',functionName,boolean)`
    
[Knowledge Base](README.md)