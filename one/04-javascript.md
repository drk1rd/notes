# javascript

## implementing in html
* within: `<script>..code..</script>`  
* outside: `<script src="javascript.js"></script>`  

## miscellaneous
* `console.log()` to output to console
* use `alert(variable)` to show content
* use `prompt()` for input
* use `${variable}` to use a variable in another whatever
* to get a random value from an array `let randomItem = myArray[Math.floor(Math.random()*myArray.length)];`

## variables
* use `var`, `let`, `const`; latter two being relatively new  
* `use strict` is a thing  
* for constant values use `const`
* to use them in strings; put the string within backtick and put the variable like `${variable}`

## math
* normal arithmetic applies
* `Math.pow(x,2)` is used for power, just like `**`
* precedence applies
* all numbers are 64 bit floating
* they are accurate upto 15 digits
* floating calc is not always accurate so you may first remove their decimal, calculate, and then again bring back decimals
* it will convert string inputed numbers to numbers
* `Nan` is reserved to show that a number is not a legal number, can use `isNan()` to check
* increment decrement occurs as always
* bitwise operators exists ;-;

## strings
* use `' '` or `" "`
* can use escape characters like `\` if a quote is being used in the string; example, `'I\'ve'`
* can concatenate them
* can write in multiline simply by using enter key if single quote, but in double quote use `\n`
* `.length`
* `.slice(start, end)`  
 `.substring(start, end)`  
  `.substr(start, length)`
* `.replace(toberep, new)`; for case sensitive `/word/i`; to replace all `/word/g`
* `.replaceAll(toberep, new)` exists
* `.toUpperCase()`  
 `.toLowerCase()`
* `.concat()`
* `.trim()` removes whitespaces from both ends  
 `.trimStart()`  
 `.trimEnd()`
* `.padStart()`  
 `.padEnd()`
 pad a string until it reaches a specific length; `pad(length, whattobepaddedwith)`
* `.charAt(position)`  
 `.charCodeAt()` returns unicode  
  or just the square brackets
* `.split()` split a string on something to convert it into arrays

## comparision
* `<`,`>`
* `=`, `!=`
* `==`
* `a >= b`, `a <= b`

## conditional
* `if`
* `else`
* `else if`
* `switch`

## logical operators
* `||` or; evaluates left to right; finds first truthy value to return if none found gives last operand
* `&&` and; finds falsy value if none found and everything was truthy gives the last operand; higher precedence than `||`
* `!` not; `!!` sometimes used to convert value to boolean type

## functions
* `function func(parameters) {}`
* scopes do exist
* use `return` to return values for further use
* default parameters are the ones that are assigned with something in the brackets itself
* arrow functions; `let func = (arg1, arg2, ..., argN) => expression;` returns whatever the expression evaluates
* multiline arrow uses curly braces
* the call stack works based on the LIFO principle i.e., last-in-first-out
* if the number of execution contexts exceeds the size of the stack, a stack overflow error will occur

## errors
* `ReferenceError` thrown when one refers to a variable that is not declared and/or initialized within the current scope
* `SyntaxError`
* `TypeError`

## objects
* ` const object = {firstkey:"one", secondkey:"two", thirdkey:3}; `
* this can be accessed by `object.firstkey`, and so on
* named index

## arrays
* numbered index
* `const cars = ["one", "two", "three"];`  
 also can just create `= []` and then give in values  
 can be accessed by using indexes  
 item can be changed
* array item can be accessed in html by `document.getElementById("id").innerHTML = arrayname;`
* `.length`
* `.sort()`
* `.forEach(a function for each value)`
* `.push()` adds a new item
* `.pop()`
* `.toString()` puts the value to string with comma separation
* `.join(specify the separator)`
* `.shift()` removes first element
* `.unshift()` adds to first index
* `delete arr[index]` deletes an item but leaves holes in place
* `.concat(other array)` joins the array, can put multiple array by commas
* `.flat()` creates a new array with sub-array elements concatenated to a specified depth
* `.splice(wherenewelementsshouldbeadded, howmanyelementsshouldberemoved, items)`
* `.slice(start, end)` creates a new array from the index forward, excluding end index; end index not necessary
* `.reverse()`

## dom
* tree-like representation of the contents of a webpage - a tree of “nodes” with different relationships depending on how they’re arranged in the HTML document.
* selectors:  
 `div.display`  
 `.display`  
 `#container > .display`  
 `div#container > div.display`  
 `firstElementChild`  
 `lastElementChild`
* query selectors:  
 `element.querySelector(selector)` returns a reference to the first match of selector  
 `element.querySelectorAll(selectors)` returns a “nodelist” containing references to all of the matches of the selectors; the return value is not an array. it looks like an array, and it somewhat acts like an array, but it’s really a “nodelist”. to convert the nodelist into an array. You can do this with Array.from()
* element creation, appening, removing:  
 `document.createElement(tagName, [options])` creates a new element of tag type tagName. creates it in memory.  
 `parentNode.appendChild(childNode)` appends childNode as the last child of parentNode  
 `parentNode.insertBefore(newNode, referenceNode)` inserts newNode into parentNode before referenceNode
 `parentNode.removeChild(child)` removes child from parentNode on the DOM and returns a reference to child
* altering:  
 `const div = document.createElement('div');`  // creates a new div referenced in the variable 'div'
 `div.style.color = 'blue';`   
 `div.style.cssText = 'color: blue; background: white;';` 
 `div.setAttribute('style', 'color: blue; background: white;');`  
 `div.setAttribute('id', 'theDiv');`  
 `div.getAttribute('id');` //returns value
 `div.removeAttribute('id');`  
 `div.classList.add('new');`  // adds class "new" to your new div  
 `div.classList.remove('new');` 
`div.classList.toggle('active');` //if has then remove, if don't then add  
`div.textContent = 'Hello World!'`  //creates a text node containing "Hello World!"  
`div.innerHTML = '<span>Hello World!</span>';`