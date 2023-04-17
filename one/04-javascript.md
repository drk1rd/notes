# javascript

## implementing in html
* within: `<script>..code..</script>`  
* outside: `<script src="javascript.js"></script>`  

## general
* `console.log()` to output to console
* use `alert(variable)` to show content
* use `prompt()` for input
* use `${variable}` to use a variable in another whatever

## variables
* use `var`, `let`, `const`; latter two being relatively new  
* `use strict` is a thing  
* for constant values use `const`

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