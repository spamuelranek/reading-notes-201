# Problems, Objects vs Primitives, The DOM 
- maybe the SUB?

## Problem Domain. Are *You* the problem? Maybe.

### Problem Domain
- Problem Domain refers to the total piece (be it a patch, new feature, some project)
  - Working with in a familiar problem domain makes it easier to learn newer tech
  - Two Ways to make it easier :
    - Break it down - Find individiual parts of the overall problem domain to solidfiy understanding and move from there
    - Take the time to learn what the Problem Domain is and what it is scoped for. Talking to the client can be an easy way to trully know what you are working toward

### Datatypes in JavaScript: Primitve and Object References
- 8? Data Types
1. Booleans
2. Null
3. Undefined
4. Number
5. BigInt?
6. String
7. Symbol

- Difference between a value and a reference
  - value is a directly associate value
  - reference is actuall a reference to an address that holds the values

- Difference between immutable and mutable data
    - Immutable is a value that can not be partly changed eg ` let word = snow `
    - Mutable is a value that can be changed `let word = [s,n,o,w]`

``` js
let lead = {
    name: 'John Lennon',
    group: 'The Beatles'
}
let coLead = Object.assign({}, lead, {
    name: 'Paul McCartney'
})
console.log(lead,colead)
// {name: "John Lennon", group: "The Beatles"}
// {name: "Paul McCartney", group: "The Beatles}
```
[reference](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)

- The above example is showing how Object.assign functions if you are not trying to make the same object. 
  - Object.assign first argument says what it is targeting. 
    - In this case `{}` is a new object
    - ` lead, {name: "Paul McCartney"}` These are the additional arguments of the new object
      - It is coping the object of `lead` and changing the property of `name: ` to Paul McCartney

- Objects that have the same contents will not be equal unless it is a duplication
  - The information will need to be normalized for equality operators to give meaningful answers

### Objects : The now being told story
- Objects are defined as follows:
```js

var object = {
    keyOne: value,
    keyTwo: value,
    key: function(){
        action;
    }
}

```
- `var object =` is used to name the object
- `{}` defines the object
- `key: value` is the properties of the object. Keys are the names: and values are the values
- `key: funtion ()` a function inside an object is called a method and associated with the object
- to call a calue or method `var two = hotel.keyTwo;`

### The non-SUB or DOCUMENT OBJECT MODEL (DOM)
- The DOM specifies ho browsers should creat a model of an HTML page and how JavaScript can accesss and update teh contests of the a web page while it is in the browser window ~ *Duckett-JAVASCRIPT and JQUERY pg.184*
  - DOM specifies how the model of the page should be structured
  - DOM defines methods and properties about access and updates.
    - additonal vocab
      - Application Programming Interface (API)
        - A way for programs to talk to one another
#### DOM TREE
  - A tree that has nodes representing every element in the HTLM
  - Different Nodes
    - Element Nodes
      - Represents HTML Elements eg `<p>`
    - Attribute Nodes
      - Represents Opening tags attributes eg ` id = cool`
      - these are part of the associated element not a child
    - Text Nodes
      - This is a node exists within other nodes
      - no other nodes exists with in text nodes

#### Working the DOM
- Access The Elements
  - Indvidual Nodes
    - `getElementById()`
    - `querySelector()`
      - CSS selector and returns first matching element
  - Multiiple Nodes
    - `getElmentByClassName()`
    - `getElementsByTagName()`
    - `querySelectorAll()`
      - CSS selector chooses all matching elements
  - Traversing
    - `parentNode`
    - `previousSibling/nextSibiling`
    - `firstChild/ lastChild`
- Working the Elements
  - Access/ Update Text Nodes
    - Identify the specific node
    - `nodeValue`
     - Allows access to content and ability to update
  - Work with HTML Content
    - `innerHTML`
      - Access to child elements and text content
      - Get Content `var content =document.getElementById("cool").innerHTML;`
      - Set Content `document.getElementById("cool").innerHTML = elContent;`
    - `textContent`
      - Access to text content
      - Get Content ``var content =document.getElementById("cool").textContent:`
      - Set Content `document.getElementById("cool").textContent = elContent;`
- DOM Queries > than one element
  - It can return more than one
    - It comes in an indexed list starting at 0 called a Nodelist
    - Selecting from within a Nodelist
      - `item()` method
      - `array[]` method
        - ``` js
        var elements = document.getElementByClassName('multiple tags');
        if (elements.length >= 1){
            var firstItem = elements[0];
        }
        ```

[Knowledge Base](README.md)
