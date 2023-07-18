
### Js Data Type
1. string
2. number : js numbers are always double ( 64-bit floating point)
3. bigint : [ES2020] store larger values than number.
4. boolean
5. undefined
6. null
7. symbol
8. Object : object { name: value } , array [], date
9. typeof operator

- object properties can be accessed in 2 ways:
1. objectname.propertyname
2. objectname["propertyname"]

### Variable declaration
1. var -  declare a varible [ 1995 to 2015 ]
2. let - declare a block varible/ block scope [ 2015 ]
3. const - declare block constant [ 2015 ] , if value & type cannot be changed. Const defined a constant reference to a value.
4. automatically

- re-declaration is not possible declared with let or const.
- let & const does not bind to this  
- let & const are hoisted to the top but not initilized.
- variable declaration can span multiple lines
- js treats ``` $, _  ``` as letter, hence can be declared as vairble

<b>Hoisting</b>: js default behaviour of moving declaration to top. Varibale can be used before declaration.

### Js Values
1. Fixed values : Literal
2. Varibale values: Varibales

- <b>undefined</b>: when value if not specified during declration.

### Javascript display object
- innerHTML : writing into an html element
- document.write(): writing into html output
- window.alert(): alert box
- console.log(): writing into browser console

<i>using document.write() after html is loaded, will delete all existing html</i>

### Operators
- arithemtic
- assignment
```
??= ( Null coalescing assignment ): if first value is undefined or null, second value is addigned.

let x;
document.getElementById("demo").innerHTML = x ??= 5; 
```
- comparison
- string
- logical
- bitwise
- ternary
- type
```
== : compare values
=== : compare values and type
```

<i>when adding a number and string, number is treated as string. Depeding upon sequence</i>
```
let x = "apple" + 10 + 8;  //apple18
let a = 78 + "apple" + 8;  //78apple8
```

### fucntions
- accessing a function without () return the function , not the function result.

### this keyword
- refers to an object. which object dependes on how this is beign invoked.
- referes to the owner of the function.
- if an object mehtod : refers to the object
- alone : refers to global object
- function : refers to global object
- function in strict mode : this is undefiend
- event - refer to element that received the event.