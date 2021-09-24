# STOP BUGGING ME!
## I *mean* it.
### seriously, like stop it
### ...please?

## Debugging (p.449)
- The Console + Dev Tools
- Common Problems
- Handling Errors

###
- Identification
  - Order of execution
    - Processes one line of code at a time
    - what is the series of steps taken to process the code?
      - it may not be just top down.
  - Execution Content
    - global
      - code not in a function
    - function
  - Variable scope
    - global scope
      - defined outside a function
    - function level
  - Hoisting
    - it hoists all the variables and functions to the top of the excution context
- Errors
  - They are your friends
  - Types:
    - Error
    - SyntaxError
    - ReferenceError
      - tried to reference a variable not declared or not within scope
    - TypeError
      - based on type of data
    - RangeError
      - Numbers not in correct range
    - URIError
      - ?
    - EvalError
- Debugging
  - Where is the Problem
    - read error message
    - console logging is your friend
    - separation of code gives meaningful points of break points
    - having a positive attitude does wonders for debugging
  - Breakpoints ?
    - ability to step through code one line at a time
- Try, Catch, and Finally
  - `try {` tries the possible problematic code
  - `} catch(exception) {` runs a possiblly different code
  - `finally{` runs with whether try or catch run

  [Knowledge Base](README.md)