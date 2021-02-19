# javascript

### variables

```js
let n = 10 // number
let b = true // boolean (true/false)
let s = "hello world" // string

// ARRAYS
let array = [1, 2, 3, "hi"] // square brackets = "array"
// access the items with square brackets
array[0] // 1
array[3] // "hi"

// arrays have some special functions:
// .map iterates through the array
array.map((item,index)=> console.log(item,index))
// .filter returns a NEW array filtered by the condition
const newArray = array.filter((item,index)=> item>2) // [3]
// .sort 
array.sort((a,b)=> a-b)
// push a new item into the array:
array.push(4) // [1, 2, 3, "hi", 4]

// OBJECTS
var o = {
    hi: 'hello',
    number: 22,
}
// access the items with dot notation
o.hi // hello
o.number // 22
```

### functions

Using function, you can create re-usable blocks of code that can greatly simplify you javascript.

```js
// declaring the function
function myFunction(argument1, argument2){
    // body
    return argument1 + argument2
}
// using the function
myFunction(1, 2) // 3
```

### conditional statements

```js
if(condition===true) {
    // run this code
}

if(3>5) {
    // will this code run? NO!
}

// && means "and" 
if(true && "true" && 5) {
    // will this code run? YES!!!
}

// || means "or"
if(true || false) {
    // will this code run? YES!!!
}

// == compares the value
if(5=="5") {
    // will this code run? YES!!!
}

// === compares the value AND the data type
if(5==="5") {
    // will this code run? NO!!!
}
```