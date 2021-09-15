# Lists, Flow, Box
## Lists, Flow, Box
### Lists, Flow, Box

## Lists(pp.62-73)
- Lists
  - Three Types:
    - Ordered Lists
      - `<ol>`
        - ordered list tag
      - `<li>`
        - line item
    - Unordered Lists
      - `<ul>`
        - unordered list tag
      - `<li>`
        - liste item
    - Definition Lists
      - `<dt>`
        - definition term
      - `<dd>`
        - definition
  - All need closing tags for every piece

## Boxes, Boxes, Boxes (pp.300-329)
- Boxes:
 - distinct properties
   - Border - all have one even if not visible
   - Margin - sits out side the border a distance away
   - padding - like margin for stuff inside the box
 - physical space
   - width
   - height
- Addtional features
  - Overflow - anytime the content is going to be too large of the box
    - `overflow : hidden;` hides extra infromation
    - `overflow : scroll;` makes the contect scrollable
  - Borders
    - width - `border-width`
    - style - `border-style`
    - color - `border-color`
    - radius - `border-radius`
  - Padding - `padding`
  - Margin - `margin`
  - Display
    - inline - `display: inline;`
      - makes block-level act like an inline
    - block - `display: block;`
      - makes inline level act like block-level
    - none - `display: none;`
      - makes it so it is not displayed on the page but is in source code

## Decisions and Loop to Loops
- Types of Data
  - `string` is text
  - `number` is a number
  - `boolean` is true/ flase
  - `null` is an empty value
  - `undefined` is undeclared
- Truthy and Falsy
## Falsy

| Value | Description |
| --- | --- |
|var highScore = flase;|The traditional Boolean False|
|var highScore = 0;|The number zero|
|var highScore = ' ';|Empty String|
|var highScore = 10/'score';|NaN|
|var highScore;| variable with no value assigned|
-*javascript and jquery By Ducket pp.167*

## Truthy

|Value| Description|
|---|---|
|var highScore = true;|Traditional Boolean True|
|var highScore = 1;| Numbers other than zero|
|var highScore = 'carrot';| Strings with Content|
|var highScore = 10/5;| Number Calculations|
|var highScore = 'true';| true written as a string|
|var highScore = 'false';| false written as a string|
|var highScore = '0';| zero written as a string|
-*javascript and jquery By Ducket pp.167*

- Now you are in for a Loop
  - Three types today:
    - For - run code for a specific number of times
      - `for (let i=0; i<=something; i++)` 
        - `i=0` is the index and initialization.
        - `i<=something` is the conditinal
        - `i++` is the incremntation
    - while - will continue to run until the conditional is false
      - `while (i<10{ i + "is how much people think you smell"; i++)`
        - `i<10` is the conditional and will break before the statement if it is no longer true
        - `i++` is the incrementation
    - do...while - the same as while but will run the statement once even if the conditional is evaluated as false
      - `do {i + "is how much people think you smell"; i++;} while (i<10); `