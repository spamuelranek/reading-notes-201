# What's an OBj**e**c*t*

## Domain Modeling
### Modeling
- This is the abstract construction of what the problem entails. This is a brief that helps multiple stakeholders communicate and express ideas about the problem

```js
var EpicFailVideo = function(epicRating, hadAnimals){
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

var parkourFail= new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4,true);

console.log(parkourFail); //==> epicRating: 7   hasAnimals:false
console.log(corgiFail); //==> epicRating: 4  hasAnimals:true
```

- `new` creates another object named EpicFailVideo
  - that object is stored in the variable `parkourFail`
  - `this.epicRating` sets the attribute to parameter



### Random Number Generation
``` js
var EpicFailVideo = function(epicRating, hasAnimals){
    this.epicRating = epicRating;
    this.hadAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max) {
    return Math.floor(Math.random()* (max - min + 1)) + min;
}

var parkourfail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1,5));
console.log(corgiFail.generateRandom(1,5));
```

- Parkourfail at `parkourFail.generateRandom()` searches through itself to find `generateRandom()`. When it does not find it it searches `prototype` and finds it there.???????

### Random Number manipulation and pairing with a boolean
``` js
var EpicFailVideo = function(epicRating,hasAnimals){
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min,max){
    return Math.floor(Math.random * (max-min+1))+min;
}

EpicFailVideo.prototype.dailylikes = function(){
    var views, percentage;
    views = this.generateRandom(10,30) * epicRating
    if (hasAnimals){
        percentage = .75;
    } else {
        percentage = .25;
    }

    return Math.round(views * percentage)
}

var parkourFail = new EpicFailVideo(7,false);
var corgiFail = new EpicFailVideo(4,true);

console.log(parkourFail.dailylikes());
console.log(corgiFail.dailylikes());
```

```js

var EpicFailVideo = function(epicRating,hasAnimals){
    this.epicRating = epicRating;
    this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min,max){
    return Math.floor(Math.random*(max-min+1)+min);
}

EpicFailVideo.prototype.dailyLikes = function(){
    var views, percentage;
    views = generateRandom(10,30) * this.epicRating;
    if (this.hasAnimals){
        percentage=.75;
    } else{
        percentage =.25;
    }
    return Math.round(views * percentage);
}

EpicFailVideo.prototype.weeklyLikes = function(){
    for (days = 0; days<7 ; days++){
        total += this.dailyLikes(); 
    }
    return total;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4,true);

console.log(parkourFail.weeklyLikes());
console.log(corgiFail.weeklyLikes());

```

## Tabled for now
- Basic Four Things:
1. `<table>` creates the table
2. `<tr>` defines teh start of each row
3. `<td>` defines each cell
4. `<th>` defines a heading

```html
<table>
    <tr>
        <th></th>
        <th scope = 'col'>fights started</th>
        <th scope = 'col'>fights won</th>
    </tr>
    <tr>
        <th scope = 'row'>Sam</th>
        <td>65</td>
        <td>2</td>
    </tr>
    <tr>
        <th scope = 'row'>Nathan</th>
        <td>1</td>
        <td>71</td>
    <tr>
```
- extra vocab:
  - `<thead>`
  - `<tbody>`
  - `<tfoot>`

## Functions, Methods, and Objects
- Constructor Notation

``` js

var sam = new Object();
    sam.age = 78;
    sam.precievedAge = 25;
    sam.postition = 'god';
    sam.posion = 'strong winds'
    sam.differenceAge = function(){
        return this.age - this.precievedAge
    }
```
- creates a new object with stated atributes

- Multiple Constructor Notation
```js

function person(name,age,position){
    this.name=name;
    this.age=age;
    this.position=positoin;
}

```

- would allow for several objects created with 

```js
var firstPerson = person('sam',556,'cryptid')
```

- Three Groups of Built-in Objects pg.122 JS
  - Browser Object Model
    - creates a model of the brower tab or window
  - Document Object Model
    - creates a model of the current web page
  - Global JavaScript Objects
    - Group of individual objects that relate to different parts of JS

[Knowledge Base](README.md)

        