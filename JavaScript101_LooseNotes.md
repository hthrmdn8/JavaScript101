# **<u>JavaScript 101</u>**

JavaScript is the world's most popular programming language!

JavaScript is the programming language of the Web.

## <u>Why Study JavaScript?</u>

JavaScript is one of the **3 languages** all web developers **must** learn:

1. JavaScript's Vital to the Internet -- Between pop-ups, entry forms, because its already embedded into most popular web browsers

2. Easy to Learn -- JavaScript is a highly abstracted language. This means it reads closer to English than it is to the machine language directly understood by computer processors. JavaScript is also strictly object-oriented. With object-oriented languages, distinct lines of code that can be reused emulate the actions of any sort of object

3. Community Support -- JavaScript is either one of the most popular programming languages around if not the most popular one. There’s a massive amount of help available online

A **computer program** is a list of "instructions" to be "executed" by a computer.

In a programming language, these programming instructions are called **statements**.

A JavaScript program is a list of programming statements.

JavaScript statements are composed of:

Values, Operators, Expressions, Keywords, and Comments.

Semicolons separate JavaScript statements.

Add a semicolon at the end of each executable statement

````javascript
let a = 0; 
````

When separated by semicolons, multiple statement on one line are allowed

````javascript
let b = 1; let c = 3;
````

JavaScript ignores 'white space', and you can add extra spaces in your code to make it more readable.

````javascript
let a = 0; 
let b = 1;
let c = 3;
````

It is a good practice to add spaces around operators; ( + = - * / )

<u>JavaScript Data Types</u>

In JavaScript there are 5 different data types that can contain values:

- `string`
- `number`
- `boolean`
- `object`
- `function`

There are 6 types of objects:

- `Object`
- `Date`
- `Array`
- `String`
- `Number`
- `Boolean`

And 2 data types that cannot contain values:

- `null`
- `undefined`

````javascript
typeof "John"                 // Returns "string"
typeof 3.14                   // Returns "number"
typeof NaN                    // Returns "number"
typeof false                  // Returns "boolean"
typeof [1,2,3,4]              // Returns "object"
typeof {name:'John', age:34}  // Returns "object"
typeof new Date()             // Returns "object"
typeof function () {}         // Returns "function"
typeof myCar                  // Returns "undefined" *
typeof null                   // Returns "object"
````

- The data type of NaN is number
- The data type of an array is object
- The data type of a date is object
- The data type of null is object
- The data type of an undefined variable is **undefined** *
- The data type of a variable that has not been assigned a value is also **undefined** *

You cannot use `typeof` to determine if a JavaScript object is an array (or a date).

## Primitive Data

A primitive data value is a single simple data value with no additional properties and methods.

The `typeof` operator can return one of these primitive types:

- `string`
- `number`
- `boolean`
- `undefined`

## Complex Data

The `typeof` operator can return one of two complex types:

- `function`
- `object`

The `typeof` operator returns "object" for objects, arrays, and null.

The `typeof` operator does not return "object" for functions.

The `typeof`operator is not a variable. It is an operator. Operators ( + - * / ) do not have any data type.

The `typeof` operator always **returns a string** (containing the type of the operand).

## Empty Values

An empty value has nothing to do with `undefined`.

An empty string has both a legal value and a type.

## Null

In JavaScript `null` is "nothing". It is supposed to be something that doesn't exist.

Unfortunately, in JavaScript, the data type of `null` is an object.

You can consider it a bug in JavaScript that `typeof null` is an object. It should be `null`.

## Difference Between Undefined and Null

`undefined` and `null` are equal in value but different in type

## <u>JavaScript Values</u>

The JavaScript syntax defines two types of values:

- Fixed values
- Variable values

Fixed values are called **Literals**.

Variable values are called **Variables**.

## JavaScript Literals

The two most important syntax rules for fixed values are:

1. **Numbers** are written with or without decimals:

````javascript
100324
10.65
-223
7

42,000//not valid because commas treat like a pair of values
````

2. **Strings** are text, written within double or single quotes.

   If you put a number in quotes, it will be treated as a text string.

````javascript
"Hello, World!"
"Pikachu was okay at best but really over hyped"
"There should have only been 3 starter pokemon"
"1002"
'Seriously it's a mouse with static problems 
"Why doesn't anyone take me seriously about this"
'Just a rat'
'Wow a little harsh on pikachu don"t you think??'
````

Console.log can print any values as long as they are separated by commas 

````javascript
console.log(12, 3, "Hello, World!", 4.01, "17"); 
````

Remember not to put commas or spaces in your integers, no matter how big they are. Formal languages are strict, the notation is concise, and even the smallest change might mean something quite different from what you intend

## JavaScript Type Conversions

Most of the time, operators and functions automatically convert the values given to them to the right type.

For example, `alert` automatically converts any value to a string to show it. Mathematical operations convert values to numbers.

There are also cases when we need to explicitly convert a value to the expected type.

````javascript
console.log(Number("2658")); //console: 2658
console.log(typeof Number("2685")); //console: number
console.log(Number(34)); //console: 34
console.log(Number("There is a reason Ash didn't even want pikachu")); //console: NaN --not a number 

console.log(String(2658)); //console: 2658
console.log(typeof String("2685")); //console: string
console.log(String(34)); //console: 34
console.log(String("There is a reason Ash didn't even want pikachu")); //console: There is a reason Ash didn't even want pikachu
````



Methods to Convert Dates to Strings

| Method            | Description                                       |
| :---------------- | :------------------------------------------------ |
| getDate()         | Get the day as a number (1-31)                    |
| getDay()          | Get the weekday a number (0-6)                    |
| getFullYear()     | Get the four digit year (yyyy)                    |
| getHours()        | Get the hour (0-23)                               |
| getMilliseconds() | Get the milliseconds (0-999)                      |
| getMinutes()      | Get the minutes (0-59)                            |
| getMonth()        | Get the month (0-11)                              |
| getSeconds()      | Get the seconds (0-59)                            |
| getTime()         | Get the time (milliseconds since January 1, 1970) |

Conversion table

| Original Value   | Converted to Number | Converted to String | Converted to Boolean |
| ---------------- | ------------------- | ------------------- | -------------------- |
| FALSE            | 0                   | "false"             | FALSE                |
| TRUE             | 1                   | "true"              | TRUE                 |
| 0                | 0                   | "0"                 | FALSE                |
| 1                | 1                   | "1"                 | TRUE                 |
| "0"              | 0                   | "0"                 | TRUE                 |
| "000"            | 0                   | "000"               | TRUE                 |
| "1"              | 1                   | "1"                 | TRUE                 |
| NaN              | NaN                 | "NaN"               | FALSE                |
| Infinity         | Infinity            | "Infinity"          | TRUE                 |
| -Infinity        | -Infinity           | "-Infinity"         | TRUE                 |
| ""               | 0                   | ""                  | FALSE                |
| "20"             | 20                  | "20"                | TRUE                 |
| "twenty"         | NaN                 | "twenty"            | TRUE                 |
| [ ]              | 0                   | ""                  | TRUE                 |
| [20]             | 20                  | "20"                | TRUE                 |
| [10,20]          | NaN                 | "10,20"             | TRUE                 |
| ["twenty"]       | NaN                 | "twenty"            | TRUE                 |
| ["ten","twenty"] | NaN                 | "ten,twenty"        | TRUE                 |
| function(){}     | NaN                 | "function(){}"      | TRUE                 |
| { }              | NaN                 | "[object Object]"   | TRUE                 |
| null             | 0                   | "null"              | FALSE                |
| undefined        | NaN                 | "undefined"         | FALSE                |



## JavaScript Variables

In a programming language, **variables** are used to **store** data values.

JavaScript uses the keywords `var`, `let` and `const` to **declare** variables.

All JavaScript **variables** must be **identified** with **unique names**.

These unique names are called **identifiers**.

Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

The general rules for constructing names for variables (unique identifiers) are:

- Names can contain letters, digits, underscores, and dollar signs.

- Names must begin with a letter (special cases use _ , $)

  ​			Using the dollar sign is not very common in JavaScript, but professional programmers often use it as an alias for the main function in a JavaScript 				library.

  ​			Using the underscore is not very common in JavaScript, but a convention among professional programmers is to use it as an alias for "private 			(hidden)" variables.

- Names are case sensitive (y and Y are different variables)

- Reserved words (like JavaScript keywords) cannot be used as names

An **equal sign** is used to **assign values** to variables.

````javascript
let a = "pikachu is overhyped";
let obviouslyTheBestPokemon = "Cydiquill";
````

Avoid saying "A IS EQUAL TO 'pikachu is overhyped'" Instead say "A is **<u>assigned</u>** to the value of 'pikachu is overhyped'"

The `let` keyword tells the code editor to create variables (prefered)

The `const` keyword tells the code editor to create variables. Must be assigned a value when they are declared (Preferred when checks are met)

The `var` keyword also tells the code editor to create variables (not preferred)



## JavaScript Keywords

JavaScript **keywords** are used to identify actions to be performed.

Common JavaScript Keywords:

| Keyword  | Description                                                  |
| :------- | :----------------------------------------------------------- |
| var      | Declares a variable                                          |
| let      | Declares a block variable                                    |
| const    | Declares a block constant                                    |
| if       | Marks a block of statements to be executed on a condition    |
| switch   | Marks a block of statements to be executed in different cases |
| for      | Marks a block of statements to be executed in a loop         |
| function | Declares a function                                          |
| return   | Exits a function                                             |
| try      | Implements error handling to a block of statements           |

Reserved Words (you cannot use these words to name variables, labels, functions etc.)

| abstract | arguments  | await*       | Boolean   |
| -------- | ---------- | ------------ | --------- |
| break    | byte       | case         | catch     |
| char     | class*     | const        | continue  |
| debugger | default    | delete       | do        |
| double   | else       | enum*        | eval      |
| export*  | extends*   | false        | final     |
| finally  | float      | for          | function  |
| goto     | if         | implements   | import*   |
| in       | instanceof | int          | interface |
| let*     | long       | native       | new       |
| null     | package    | private      | protected |
| public   | return     | short        | static    |
| super*   | switch     | synchronized | this      |
| throw    | throws     | transient    | true      |
| try      | typeof     | var          | void      |
| volatile | while      | with         | yield     |

Words marked with* are new in ECMAScript 5 and 6.

## JavaScript  Declaring  Variables

Creating a variable in JavaScript is called "declaring" a variable.

````javascript
let a;
````

After the declaration, the variable has no value (technically it has the value of `undefined`).

To **assign** a value to the variable, use the equal sign:

You can also assign a value to the variable when you declare it:

````javascript
let a;
a = 10;

let b = 10;
````

In computer programs, variables are often declared without a value. The value can be something that has to be calculated, or something that will be provided later, like user input.

A variable declared without a value will have the value `undefined`.

It's a good programming practice to declare all variables at the beginning of a script.

Let

Variables defined with `let` cannot be Redeclared.

Variables defined with `let` must be Declared before use.

Variables defined with `let` have Block Scope.

You cannot accidentally redeclare a variable defined with let

````javascript
let a = 10;
let a = 11; //console: Syntax Error: 'a' has already been declared
````

###### 

Var

Variables defined with `var` can be Redeclared.

Variables declared with the `var` keyword can NOT have block scope.

Redeclaring a variable using the `var` keyword can impose problems.

Redeclaring a variable inside a block will also redeclare the variable outside the block when using var which can have unintended consequences 

Const

Variables defined with `const` cannot be Redeclared.

Variables defined with `const` cannot be Reassigned.

Variables defined with `const` have Block Scope.

````javascript
const a = 10;
const a = 11; //error
const c = c + 10 //error
const b; //error
b = 5;  //error
````

JavaScript `const` variables must be assigned a value when they are declared

As a general rule, always declare a variable with `const` unless you know that the value will change

The keyword `const` is a little misleading.

It does not define a constant value. It defines a constant reference to a value.

Because of this you can NOT:

- Reassign a constant value
- Reassign a constant array
- Reassign a constant object

- But you CAN:

- Change the elements of constant array
- Change the properties of constant object

Block Scope 

In this context block scope means variables declared inside a { } block cannot be accessed from outside the block

````javascript
const x = 10;
// Here x is 10

{
const x = 2;
// Here x is 2
}

// Here x is 10
````



## JavaScript Statement Identifiers

JavaScript statements often start with a **statement identifier** to identify the JavaScript action to be performed.

Statement identifiers are reserved words and cannot be used as variable names (or any other things).

The following table lists all JavaScript statement identifiers:

| Statement                                                    | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [break](https://www.w3schools.com/jsref/jsref_break.asp)     | Exits a switch or a loop                                     |
| const                                                        | Declares a variable with a constant value                    |
| [class](https://www.w3schools.com/jsref/jsref_class.asp)     | Declares a class                                             |
| [continue](https://www.w3schools.com/jsref/jsref_continue.asp) | Breaks one iteration (in the loop) if a specified condition occurs, and continues with the next iteration in the loop |
| [debugger](https://www.w3schools.com/jsref/jsref_debugger.asp) | Stops the execution of JavaScript, and calls (if available) the debugging function |
| [do ... while](https://www.w3schools.com/jsref/jsref_dowhile.asp) | Executes a block of statements and repeats the block while a condition is true |
| [for](https://www.w3schools.com/jsref/jsref_for.asp)         | Loops through a block of code a number of times              |
| [for ... in](https://www.w3schools.com/jsref/jsref_forin.asp) | Loops through the properties of an object                    |
| [for ... of](https://www.w3schools.com/jsref/jsref_forof.asp) | Loops through the values of an iterable object               |
| [function](https://www.w3schools.com/jsref/jsref_function.asp) | Declares a function                                          |
| [if ... else ... else if](https://www.w3schools.com/jsref/jsref_if.asp) | Marks a block of statements to be executed depending on a condition |
| let                                                          | Declares a variable inside brackets {} scope                 |
| [return](https://www.w3schools.com/jsref/jsref_return.asp)   | Stops the execution of a function and returns a value from that function |
| [switch](https://www.w3schools.com/jsref/jsref_switch.asp)   | Marks a block of statements to be executed depending on different cases |
| [throw](https://www.w3schools.com/jsref/jsref_throw.asp)     | Throws (generates) an error                                  |
| [try ... catch ... finally](https://www.w3schools.com/jsref/jsref_try_catch.asp) | Marks the block of statements to be executed when an error occurs in a try block, and implements error handling |
| [var](https://www.w3schools.com/jsref/jsref_var.asp)         | Declares a variable                                          |
| [while](https://www.w3schools.com/jsref/jsref_while.asp)     | Marks a block of statements to be executed while a condition is true |

## JavaScript is Case Sensitive

All JavaScript identifiers are **case sensitive**. 

The variables `animalCrossing` and `animalcrossing`, are two different variables

````javascript
let animalCrossing, animalcrossing;
animalCrossing = "Isabell isn't helpful";
animalcrossing = "Neither is the Nook family";
````

Variable names need to be written in camelCase as a standard

Hyphens are not allowed in JavaScript. They are reserved for subtractions.

## JavaScript Operators

JavaScript uses **arithmetic operators** ( `+` `-` `*` `/` ) to **compute** values

 An expression is a combination of values, variables, and operators, which computes to a value.

The computation is called an evaluation.

| Operator | Description                  |
| :------- | :--------------------------- |
| +        | Addition                     |
| -        | Subtraction                  |
| *        | Multiplication               |
| **       | Exponentiation               |
| /        | Division                     |
| %        | Modulus (Division Remainder) |
| ++       | Increment                    |
| --       | Decrement                    |

Order of operations matters in coding mathematics 

````javascript
let a = 1 + 3;
let b = (5 + 7) * 10;
let c = 2 * (10 + 5) - 13;
````

JavaScript uses an **assignment operator** ( `=` ) to **assign** values to variables:

````javascript
let a = 72;
````

Expressions can also contain variable values

````javascript
let x = 5;
console.log(x * 10);  //ouput: 50
````

The values can be of various types, such as numbers and strings.

````javascript
console.log("I'll admit pikachu is at least top" + " " + 25); //console: I'll admit pikachu is at least top 25
````

## JavaScript Assignment Operators

Assignment operators assign values to JavaScript variables.

| Operator | Example | Same As    |
| :------- | :------ | :--------- |
| =        | x = y   | x = y      |
| +=       | x += y  | x = x + y  |
| -=       | x -= y  | x = x - y  |
| *=       | x *= y  | x = x * y  |
| /=       | x /= y  | x = x / y  |
| %=       | x %= y  | x = x % y  |
| **=      | x **= y | x = x ** y |

````javascript
let x = 10;
x += 5; //console: 15

let z = 10;
z -= 5; //console: 5

let y = 10;
y *= 5; //console: 50
````

## JavaScript String Operators

The `+` operator can also be used to add (concatenate) strings.

````javascript
let text1 = "Pikachu";
let text2 = "is overhyped";
let text3 = text1 + " " + text2; //console: Pikachu is overhyped
````

The `+=` assignment operator can also be used to add (concatenate) strings:

````javascript
let text1 = "How dare ";
text1 += "you say that about pikachu";
````

Adding two numbers, will return the sum, but adding a number and a string will return a string:

````javascript
let x = 15 + 5; //console: 20
let y = "15" + 5; //console: 155
let z = "Hello" + 5; //console: Hello5
````

## JavaScript Comments

Not all JavaScript statements are "executed".

Code after double slashes `//` or between `/*` and `*/` is treated as a **comment**.

Comments are ignored, and will not be executed

Single line comments start with `//`.

Any text between `//` and the end of the line will be ignored by JavaScript (will not be executed).

Multi-line comments start with `/*` and end with `*/`.

Any text between `/*` and `*/` will be ignored by JavaScript.

Using comments to prevent execution of code is suitable for code testing.

Adding `//` in front of a code line changes the code lines from an executable line to a comment.

````javascript
//I will be ignored

/*Same
*/

/*
me too
*/ I wont

me neither 

//the code below assigns a the value of 2 + 3
let a = 2 + 3;
````

JavaScript comments can be used to explain JavaScript code, and to make it more readable.

JavaScript comments can also be used to prevent execution, when testing alternative code.

## JavaScript Character Set

JavaScript uses the **Unicode** character set.

Unicode covers (almost) all the characters, punctuations, and symbols in the world. 

The **Unicode Standard** provides a unique number for every character, no matter the platform, device, application, or language. **UTF-8** is a popular Unicode encoding which has 88-bit code units.

## JavaScript Unicode

There are several ways that Unicode may be needed in JavaScript. These include:

- Unicode in JavaScript source code.

- Unicode in JavaScript strings.

- Unicode in JavaScript source code

  In JavaScript, the identifiers and string literals can be expressed in Unicode via a Unicode escape sequence. The general syntax is `\uXXXX`, where X denotes four hexadecimal digits. For example, the letter `o` is denoted as ‘\u006F’ in Unicode. Hence, to write the letter “foo” in Unicode, we can use the following code.

````javascript
let f\u006F\u006F = 'abc';
console.log(foo)
````

## JavaScript String Methods/Properties

A **JavaScript property** is a characteristic of an object, often describing attributes associated with a data structure

Strings are objects, but that is covered in greater detail in later chapters. No need to worry about that now.

Dot notation is one way to access a property of an object. To use dot notation, **write the name of the object, followed by a dot (.), followed by the name of the property**.

There are 3 methods for extracting a part of a string:

- `slice(*start*, *end*)`

- `substring(*start*, *end*)`

- `substr(*start*, *length*)`

  `slice()` extracts a part of a string and returns the extracted part in a new string.

  The method takes 2 parameters: the start position, and the end position (end not included).

  ````javascript
  let str = "Heather, Keifer, Xena";
  let part = str.slice(9, 15); //output : Heather, Xena
  ````

  JavaScript counts positions from zero. First position is 0.

  If a parameter is negative, the position is counted from the end of the string.

  ````java
  let str = "Heather, Keifer, Xena";
  let part = str.slice(-12, -6); //output : Heather, Xena
  ````

  If you omit the second parameter, the method will slice out the rest of the string:

  ````javascript
  let str = "Heather, Keifer, Xena";
  let part = str.slice(7); //output : Heather
  ````

  or, counting from the end:

  ````javascript
  let str = "Heather, Keifer, Xena";
  let part = str.slice(-12); //output : Heather
  ````

  `substring()` is similar to `slice()`.

  The difference is that `substring()` cannot accept negative indexes.

  ````javascript
  let str = "Heather, Keifer, Xena";
  let part = substring(7, 13); //output : Heather, Xena
  ````

  If you omit the second parameter, `substring()` will slice out the rest of the string.

  ````javascript
  let str = "Heather, Keifer, Xena";
  let part = str.substr(7); //output : Heather
  ````

  If the first parameter is negative, the position counts from the end of the string.

  ````javascript
  let str = "Heather, Keifer, Xena";
  let part = str.substr(-4); //output : Xena
  ````

  The `replace()` method replaces a specified value with another value in a string:

  ````javascript
  let text = "Pickachu is the best!";
  let newText = text.replace("Pikachu", "Cydiquill"); //output: Cydiquill is the best!
  ````

  The `replace()` method does not change the string it is called on. It returns a new string.

  By default, the `replace()` method replaces **only the first** match

  

  ````javascript
  let text = "Pikachu is the best! Pikachu is okay at best!";
  let newText = text.replace("Pikachu", "Cydiquill"); //output: Cydiquill is the best! Pikachu is okay at best!
  ````

  By default, the `replace()` method is case sensitive

  To replace case insensitive, use a **regular expression** with an `/i` flag (insensitive)

  

  ````javascript
  let text = "PIkAchU is the best! Pikachu is okay at best!";
  let newText = text.replace(/PIKACHU/i, "Cydiquill"); //output: Cydiquill is the best Pikachu is okay at best!!
  ````

  To replace all matches, use a **regular expression** with a `/g` flag (global match):

  

  ````javascript
  let text = "Pikachu is the best! Yeah Pikachu is the best!";
  let newText = text.replace(/Pikachu/g, "Cydiquill"); //output: Cydiquill is the best! Cydiquill is okay at best!
  ````

  A string is converted to upper case with `toUpperCase()`

  A string is converted to lower case with `toLowerCase()`

  ````javascript
  let text1 = "Hello World!";
  let text2 = text1.toUpperCase();
  let text3 = "Hello World!";
  let text4 = text3.toUpperCase();
  ````

  `concat()` joins two or more strings

  ````javascript
  let text1 = "Hello";
  let text2 = "World";
  let text3 = text1.concat(" ", text2);
  ````

  The `concat()` method can be used instead of the plus operator.

  ````javascript
  let text = "Hello" + " " + "World!";
  let text = "Hello".concat(" ", "World!");
  ````

  The `trim()` method removes whitespace from both sides of a string

  ````javascript
  let text = "      Hello World!      ";
  let text.trim()
  ````

  ECMAScript 2017 added two String methods: `padStart` and `padEnd` to support padding at the beginning and at the end of a string.

  ````javascript
  let text1 = "7";
  let padded1 = text.padStart(4,0);
  let text2 = "5";
  let padded2 = text.padEnd(4,0);
  ````

  The `charAt()` method returns the character at a specified index (position) in a string

  ````javascript
  let text = "HELLO WORLD";
  let char = text.charAt(0);
  ````

  ECMAScript 5 (2009) allows property access [ ] on strings

  ````javascript
  let text = "HELLO WORLD";
  let char = text[0];
  ````

  Property access might be a little **unpredictable:**

  - It makes strings look like arrays (but they are not)
  - If no character is found, [ ] returns undefined, while charAt() returns an empty string.
  - It is read only. str[0] = "A" gives no error (but does not work!)

  ````javascript
  let text = "HELLO WORLD";
  text[0] = "A";    //console: Gives no error, but does not work
  ````

  A string can be converted to an array with the `split()` method:

  ````javascript
  let text = "Stardew|Valley, Where all your dreams come true"
  text.split(",")    // Split on commas
  text.split(" ")    // Split on spaces
  text.split("|")    // Split on pipe
  ````

  If the separator is omitted, the returned array will contain the whole string in index [0].

  If the separator is "", the returned array will be an array of single characters:

  ````javascript
  let text = "Stardew|Valley, Where all your dreams come true"
  text.split("") 
  ````

  

| Method                                                       | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [charAt()](https://www.w3schools.com/jsref/jsref_charat.asp) | Returns the character at the specified index (position)      |
| [charCodeAt()](https://www.w3schools.com/jsref/jsref_charcodeat.asp) | Returns the Unicode of the character at the specified index  |
| [concat()](https://www.w3schools.com/jsref/jsref_concat_string.asp) | Joins two or more strings, and returns a new joined strings  |
| [endsWith()](https://www.w3schools.com/jsref/jsref_endswith.asp) | Checks whether a string ends with specified string/characters |
| [fromCharCode()](https://www.w3schools.com/jsref/jsref_fromcharcode.asp) | Converts Unicode values to characters                        |
| [includes()](https://www.w3schools.com/jsref/jsref_includes.asp) | Checks whether a string contains the specified string/characters |
| [indexOf()](https://www.w3schools.com/jsref/jsref_indexof.asp) | Returns the position of the first found occurrence of a specified value in a string |
| [lastIndexOf()](https://www.w3schools.com/jsref/jsref_lastindexof.asp) | Returns the position of the last found occurrence of a specified value in a string |
| [localeCompare()](https://www.w3schools.com/jsref/jsref_localecompare.asp) | Compares two strings in the current locale                   |
| [match()](https://www.w3schools.com/jsref/jsref_match.asp)   | Searches a string for a match against a regular expression, and returns the matches |
| [repeat()](https://www.w3schools.com/jsref/jsref_repeat.asp) | Returns a new string with a specified number of copies of an existing string |
| [replace()](https://www.w3schools.com/jsref/jsref_replace.asp) | Searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced |
| [search()](https://www.w3schools.com/jsref/jsref_search.asp) | Searches a string for a specified value, or regular expression, and returns the position of the match |
| [slice()](https://www.w3schools.com/jsref/jsref_slice_string.asp) | Extracts a part of a string and returns a new string         |
| [split()](https://www.w3schools.com/jsref/jsref_split.asp)   | Splits a string into an array of substrings                  |
| [startsWith()](https://www.w3schools.com/jsref/jsref_startswith.asp) | Checks whether a string begins with specified characters     |
| [substr()](https://www.w3schools.com/jsref/jsref_substr.asp) | Extracts the characters from a string, beginning at a specified start position, and through the specified number of character |
| [substring()](https://www.w3schools.com/jsref/jsref_substring.asp) | Extracts the characters from a string, between two specified indices |
| [toLocaleLowerCase()](https://www.w3schools.com/jsref/jsref_tolocalelowercase.asp) | Converts a string to lowercase letters, according to the host's locale |
| [toLocaleUpperCase()](https://www.w3schools.com/jsref/jsref_tolocaleuppercase.asp) | Converts a string to uppercase letters, according to the host's locale |
| [toLowerCase()](https://www.w3schools.com/jsref/jsref_tolowercase.asp) | Converts a string to lowercase letters                       |
| [toString()](https://www.w3schools.com/jsref/jsref_tostring_string.asp) | Returns the value of a String object                         |
| [toUpperCase()](https://www.w3schools.com/jsref/jsref_touppercase.asp) | Converts a string to uppercase letters                       |
| [trim()](https://www.w3schools.com/jsref/jsref_trim_string.asp) | Removes whitespace from both ends of a string                |
| [valueOf()](https://www.w3schools.com/jsref/jsref_valueof_string.asp) | Returns the primitive value of a String object               |

## JavaScript Number Methods

| Method                                                       | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [isFinite()](https://www.w3schools.com/jsref/jsref_isfinite_number.asp) | Checks whether a value is a finite number                    |
| [isInteger()](https://www.w3schools.com/jsref/jsref_isinteger.asp) | Checks whether a value is an integer                         |
| [isNaN()](https://www.w3schools.com/jsref/jsref_isnan_number.asp) | Checks whether a value is Number.NaN                         |
| [isSafeInteger()](https://www.w3schools.com/jsref/jsref_issafeinteger.asp) | Checks whether a value is a safe integer                     |
| [toExponential(x)](https://www.w3schools.com/jsref/jsref_toexponential.asp) | Converts a number into an exponential notation               |
| [toFixed(x)](https://www.w3schools.com/jsref/jsref_tofixed.asp) | Formats a number with x numbers of digits after the decimal point |
| [toLocaleString()](https://www.w3schools.com/jsref/jsref_tolocalestring_number.asp) | Converts a number into a string, based on the locale settings |
| [toPrecision(x)](https://www.w3schools.com/jsref/jsref_toprecision.asp) | Formats a number to x length                                 |
| [toString()](https://www.w3schools.com/jsref/jsref_tostring_number.asp) | Converts a number to a string                                |
| [valueOf()](https://www.w3schools.com/jsref/jsref_valueof_number.asp) | Returns the primitive value of a number                      |

## JavaScript Boolean

In programing we have a datatype that only has two values, `Boolean`. 

`Boolean` data types can only have the values true or false.

`Boolean` data types are very important will ask a question, and will normally start with 'is'.

`Boolean` statements are very specific about what question is being asked. 

You can use the `Boolean()` function to find out if an expression (or a variable) is true

````javascript
console.log(Boolean("true")); //console: true
console.log(Boolean("TRUE")); //console: true
console.log(Boolean(0)); //console: false
console.log(Boolean(1)); //console: true
console.log(Boolean('')); //console: false
console.log(Boolean('LaunchCode')); //console: true
console.log(Boolean(-1)); //console: true
````

Conversion table

| Original Value   | Converted to Number | Converted to String | Converted to Boolean |
| ---------------- | ------------------- | ------------------- | -------------------- |
| FALSE            | 0                   | "false"             | FALSE                |
| TRUE             | 1                   | "true"              | TRUE                 |
| 0                | 0                   | "0"                 | FALSE                |
| 1                | 1                   | "1"                 | TRUE                 |
| "0"              | 0                   | "0"                 | TRUE                 |
| "000"            | 0                   | "000"               | TRUE                 |
| "1"              | 1                   | "1"                 | TRUE                 |
| NaN              | NaN                 | "NaN"               | FALSE                |
| Infinity         | Infinity            | "Infinity"          | TRUE                 |
| -Infinity        | -Infinity           | "-Infinity"         | TRUE                 |
| ""               | 0                   | ""                  | FALSE                |
| "20"             | 20                  | "20"                | TRUE                 |
| "twenty"         | NaN                 | "twenty"            | TRUE                 |
| [ ]              | 0                   | ""                  | TRUE                 |
| [20]             | 20                  | "20"                | TRUE                 |
| [10,20]          | NaN                 | "10,20"             | TRUE                 |
| ["twenty"]       | NaN                 | "twenty"            | TRUE                 |
| ["ten","twenty"] | NaN                 | "ten,twenty"        | TRUE                 |
| function(){}     | NaN                 | "function(){}"      | TRUE                 |
| { }              | NaN                 | "[object Object]"   | TRUE                 |
| null             | 0                   | "null"              | FALSE                |
| undefined        | NaN                 | "undefined"         | FALSE                |

`Boolean` data types are useful for comparing two values

````javascript
Boolean(6 == 7); //output: false
Boolean(10 < 33); //output: true
Boolean(26 > (5 + 3) * 4) //output: false
Boolean("Pikachu" == "Best Pokemon Ever")  //output: false
Boolean("5" == 5)  //output: true
Boolean("five" == 5)  //output: false
Boolean(false == 0)  //output: true
Boolean(true == 1)  //output: true
Boolean(true == -1)  //output: false
````

For the example above if we run all of the statements at once it will only give us the answer to the last comparison. This is a caveat of Repl.it. Even though we are not telling the console to print, or log anything it still gives us the answer to the last equation. 

## JavaScript Comparison Operators

| Operator | Description                       |
| :------- | :-------------------------------- |
| ==       | equal to                          |
| ===      | equal value and equal type        |
| !=       | not equal                         |
| !==      | not equal value or not equal type |
| >        | greater than                      |
| <        | less than                         |
| >=       | greater than or equal to          |
| <=       | less than or equal to             |
| ?        | ternary operator                  |

In order to make a comparison in JavaScript it is important that we are comparing the same data types. JavaScript can compare values that are not the same data type, but this can have unintended consequences. 

When doing a comparison from string to another datatype JavaScript always converts the other data type to a string. 

We use `==` if the two are different data types, but with conversion there is almost no real life context where you will ever need to use `==`

 The `===` operator behaves identically to the abstract equality operator `==` except no type conversion is done, and the types must be the same to be considered equal 

To quote Douglas Crockford's  [JavaScript: The Good Parts](https://rads.stackoverflow.com/amzn/click/com/0596517742),

> JavaScript has two sets of equality operators: `===` and `!==`, and their evil twins `==` and `!=`. The good ones work the way you would expect. If the two operands are of the same type and have the same value, then `===` produces `true` and `!==` produces `false`. The evil twins do the right thing when the operands are of the same type, but if they are of different types, they attempt to coerce the values. The rules by which they do that are complicated and unmemorable. These are some of the interesting cases:

````javascript
'' == '0'           //console: false
0 == ''             //console: true
0 == '0'            //console: true

false == 'false'    //console: false
false == '0'        //console: true

false == undefined  //console: false
false == null       //console: false
null == undefined   //console: true

' \t\r\n ' == 0     //console: true
````

![image-20211208144849088](C:\Users\Heather\AppData\Roaming\Typora\typora-user-images\image-20211208144849088.png)

For objects, `==` and `===` act consistently with one another (except in a special case).

```js
let a = [1,2,3];
let b = [1,2,3];

let c = { x: 1, y: 2 };
let d = { x: 1, y: 2 };

let e = "text";
let f = "te" + "xt";

a == b            // false
a === b           // false

c == d            // false
c === d           // false

e == f            // true
e === f           // true
```

The special case is when you compare a primitive with an object that evaluates to the same primitive, due to its `toString` or `valueOf` method. For example, consider the comparison of a string primitive with a string object created using the `String` constructor.

```js
"abc" == new String("abc")    // true
"abc" === new String("abc")   // false
```

Here the `==` operator is checking the values of the two objects and returning `true`, but the `===` is seeing that they're not the same type and returning `false`. Which one is correct? That really depends on what you're trying to compare. My advice is to bypass the question entirely and just don't use the `String` constructor to create string objects from string literals.

`var1 === var2`

When using `===` for JavaScript equality testing, everything is as is.
Nothing gets converted before being evaluated.

https://dorey.github.io/JavaScript-Equality-Table/

![Equality evaluation of === in JS](https://i.stack.imgur.com/62vxI.png)

`var1 == var2`

When using `==` for JavaScript equality testing, some ***funky conversions*** take place.

![Equality evaluation of == in JS](https://i.stack.imgur.com/35MpY.png)

Summary of equality in JavaScript

![Equality in Javascript](https://i.stack.imgur.com/FX7z1.png)

## JavaScript Logical Operators

| Operator | Description |
| :------- | :---------- |
| &&       | logical and |
| \|\|     | logical or  |
| !        | logical not |

A **compound boolean expression** is a boolean expression built out of smaller boolean expressions. JavaScript allows us to create a compound boolean expression using these three logical operators.

&& (and) takes two operands, and only results in true if both operands are true. If one, or both are false the overall expression is false

|| (or) takes two operands, and results in true if either operands are true. Only if both operands are false will the overall expression be false

! (bang/not) takes only one operand, and reverses its boolean value. 

Operator precedence is the set of rules that dictate in which order the operators are applied.

JavaScript will always apply the logical NOT operator, `!`, first. Next, it applies the arithmetic operators, followed by the comparison operators. The logical AND and OR are applied last

| Precedence |          Category           |        Operators         |
| :--------: | :-------------------------: | :----------------------: |
| (highest)  |         Logical NOT         |           `!`            |
|            |       Exponentiation        |           `**`           |
|            | Multiplication and division |      `*`, `/`, `%`       |
|            |  Addition and subtraction   |         `+`, `-`         |
|            |         Comparison          |   `<=`, `>=`, `>`, `<`   |
|            |          Equality           | `===`, `!==`, `==`, `!=` |
|            |         Logical AND         |           `&&`           |
|  (lowest)  |         Logical OR          |           `||`           |

## JavaScript Truth Tables

The truth tables tell us what the truthiness of an *expression* is based on the truthiness of its *parts*.

For instance, the first row in the Negation truth table (below) should be read like this: “if statement A is True, then the expression !A is False.”

![img](https://miro.medium.com/max/1270/1*SX5-E0EOlfb-HfuttEblHw.png)

The **Negation** table is very straightforward. Negation is the only unary logical operator, meaning it acts on a single input. This means that `!A || B` should not be considered the same as `!(A || B)`. Parentheses act like grouping notation similar to what you’d find in mathematics.

There are two big caveats to treating JavaScript code like propositional logic: **short circuiting** and **order of operations**.

Short circuiting is something that JavaScript engines do to save time by not evaluating something that will not change the output of the whole expression. The function `doSomething()` in the following examples is never called because no matter what it returned, the outcome of the logical expression wouldn’t change:

````javascript
// doSomething() is never called
false && doSomething();
true || doSomething();
````

## JavaScript Conditionals

## Conditional Statements

Very often when you write code, you want to perform different actions for different decisions.

You can use conditional statements in your code to do this.

In JavaScript we have the following conditional statements:

- Use `if` to specify a block of code to be executed, if a specified condition is true
- Use `else` to specify a block of code to be executed, if the same condition is false
- Use `else if` to specify a new condition to test, if the first condition is false
- Use `switch` to specify many alternative blocks of code to be executed

Use the `if` statement to specify a block of JavaScript code to be executed if a condition is true.

````javascript
if (hour < 18) {
  greeting = "Good Morning Ducklings!";
}
````

Use the `else` statement to specify a block of code to be executed if the condition is false.

````javascript
if (hour < 18) {
  greeting = "Good Morning Ducklings!";
} else {
  greeting = "Good evening";
}
````

Use the `else if` statement to specify a new condition if the first condition is false.

````javascript
if (time < 10) {
  greeting = "Good Morning Ducklings!";
} else if (time < 20) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
````

Use the `switch` statement to select one of many code blocks to be executed.

This is how it works:

- The switch expression is evaluated once.
- The value of the expression is compared with the values of each case.
- If there is a match, the associated block of code is executed.
- If there is no match, the default code block is executed.

````javascript
switch (new Date().getDay()) {
  case 0:
    day = "Sunday";
    break;
  case 1:
    day = "Monday";
    break;
  case 2:
     day = "Tuesday";
    break;
  case 3:
    day = "Wednesday";
    break;
  case 4:
    day = "Thursday";
    break;
  case 5:
    day = "Friday";
    break;
  case 6:
    day = "Saturday";
}
````

## JavaScript Nested Conditionals 

Embedding conditional statement inside another conditional statement is called a Nested conditional statement.

````javascript
if ( test condition 1)
{
 
   //If the test condition 1 is TRUE then these it will check for test condition 2
   if ( test condition 2)
   {
    //If the test condition 2 is TRUE then these statements will be executed
    Test condition 2 True statements;
   }

   else
   {
    //If the c test condition 2 is FALSE then these statements will be executed
    Test condition 2 False statements;
   }

else
{
 //If the test condition 1 is FALSE then these statements will be executed
 Test condition 1 False statements;
}
````

![FLOW CHART For Nested If in C Programming](https://www.tutorialgateway.org/wp-content/uploads/NESTED-IF-FLOW-CHART.jpg?ezimgfmt=rs:521x338/rscb179/ng:webp/ngcb179)

If the Test Condition1 is FALSE, then STATEMENT3 will execute. If Test Condition1 is TRUE, then it will check for the Test Condition2, and if it is TRUE, STATEMENT1 will execute else STATEMENT2.

## JavaScript More In Depth Into Strings

A JavaScript string is zero or more characters written inside quotes.

The string data type is a collection type. Data types that are comprised of smaller pieces are called **collection data types**, or simply **collection types**.

A **character** is a string that contains exactly one element, such as `'a'`, `"?"`, or even `" "` (a single space character).

Strings are built out of characters, and because of this we can break down a string into its individual characters. Each of these characters have a length of one

To add punctuation to a string

| Code | Result | Description  |
| :--- | :----- | :----------- |
| \'   | '      | Single quote |
| \"   | "      | Double quote |
| \\   | \      | Backslash    |

To add white space into a string

| Code | Result               |
| :--- | :------------------- |
| \b   | Backspace            |
| \f   | Form Feed            |
| \n   | New Line             |
| \r   | Carriage Return      |
| \t   | Horizontal Tabulator |
| \v   | Vertical Tabulator   |

Primitive values, like the string "John Doe", cannot have properties or methods (because they are not objects).

But with JavaScript, methods and properties are also available to primitive values, because JavaScript treats primitive values as objects when executing methods and properties.

The `length` property returns the length of a string

````javascript
let txt = "Stardew Valley";
let length = txt.length;
````

The `indexOf()` method returns the index of (the position of) the `first` occurrence of a specified text in a string

````javascript
let str = "Please locate where 'locate' occurs!";
str.indexOf("locate");
````

The `lastIndexOf()` method returns the index of the **last** occurrence of a specified text in a string

````javascript
let str = "Please locate where 'locate' occurs!";
str.lastIndexOf("locate");
````

Both `indexOf()`, and `lastIndexOf()` return -1 if the text is not found:

````javascript
let str = "Please locate where 'locate' occurs!";
str.lastIndexOf("John");
````

Both methods accept a second parameter as the starting position for the search

````javascript
let str = "Please locate where 'locate' occurs!";
str.indexOf("locate", 15);
````

The `lastIndexOf()` methods searches backwards (from the end to the beginning), meaning: if the second parameter is `15`, the search starts at position 15, and searches to the beginning of the string

````javascript
let str = "Please locate where 'locate' occurs!";
str.lastIndexOf("locate", 15);
````

The `search()` method searches a string for a specified value and returns the position of the match

````javascript
let str = "Please locate where 'locate' occurs!";
str.search("locate");
````

The two methods, `indexOf()` and `search()`, are **equal?**

They accept the same arguments (parameters), and return the same value?

The two methods are **NOT** equal. These are the differences:

- The `search()` method cannot take a second start position argument.
- The `indexOf()` method cannot take powerful search values (regular expressions).

## JavaScript Ordered Collections

We defined strings as *sequential* collections of characters. This means that the individual characters that make up the string are assumed to be in a particular order from left to right.

Collection types that allow their elements to be ordered are known as **ordered collections**

**Bracket notation** is the special syntax that allows us to access the individual characters that make up a string. 

**Index** is the location of an item in a string, array etc.

An expression of the form `someString[i]` gives the character at index `i`.

````javascript
let jsCreator = "Brendan Eich";
let firstInitial = jsCreator[0];
let lastInitial = jsCreator[8];

let outputStr = "JavaScript was created by somebody with initials " +
   firstInitial + "." +
   lastInitial + ".";

console.log(outputStr); //output: JavaScript was created by somebody with initials B.E.
````

````javascript
let jsCreator = "Brendan Eich";

console.log(jsCreator[-1]); //output: undefined
console.log(jsCreator[42]); //output: undefined
````

## JavaScript Strings as Objects

Normally, JavaScript strings are primitive values, created from literals

But strings can also be defined as objects with the keyword `new`:

An **object** is a collection of related data and operations. An operation that can be carried out on an object is known as a **method**. A piece of data associated with an object is known as a **property**.

````javascript
let y = new String("John");
````

Do not create Strings objects.

The `new` keyword complicates the code and slows down execution speed.

String objects can produce unexpected results:

````javascript
let x = "John";
let y = new String("John");
console.log(x == y); //console: true
console.log(x === y); //console: false
````

Comparing two JavaScript objects **always** returns **false**.

Javascript String is immutable, which means once a String object is assigned to String reference the object value cannot be changed. However, we can still assign a new object to a String reference

````javascript
let myVar = "Hello World";
myVar.toUpperCase();
````

One may think after the first line the *myVar* will become “HELLO WORLD”, but it still equals to “Hello World”. The method will return a new String object it will not change the existing String reference. So we have to assign it to a new variable to get the desired value.

````javascript
let myVarUpperCase = myVar.toUpperCase();
````

It may seem that once a String reference is assigned to a String object it cannot be reused as we can't change the value but we can assign existing String reference a new String object altogether.

````javascript
let str = "Hello World";
str = "Hello World!!!!"; //new String reference assigned
//this will assign return new String reference to myVar object.
str = str.toUpperCase();
````

*Note*: We also cannot assign a new character to an index in String by square bracket notation. As Strings are immutable, by doing that we will be updating the content of String reference which cannot be possible in case of immutability.

````javascript
var myVar = "Hello";
myVar[0] = "i";//still myVar remains same
````

String object has many methods which deal with string characters and all of them returns a new String object instead of modifying the String object on which they are called.

## JavaScript Array Methods

| Method                                                       | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [concat()](https://www.w3schools.com/jsref/jsref_concat_array.asp) | Joins two or more arrays, and returns a copy of the joined arrays |
| [copyWithin()](https://www.w3schools.com/jsref/jsref_copywithin.asp) | Copies array elements within the array, to and from specified positions |
| [entries()](https://www.w3schools.com/jsref/jsref_entries.asp) | Returns a key/value pair Array Iteration Object              |
| [every()](https://www.w3schools.com/jsref/jsref_every.asp)   | Checks if every element in an array pass a test              |
| [fill()](https://www.w3schools.com/jsref/jsref_fill.asp)     | Fill the elements in an array with a static value            |
| [filter()](https://www.w3schools.com/jsref/jsref_filter.asp) | Creates a new array with every element in an array that pass a test |
| [find()](https://www.w3schools.com/jsref/jsref_find.asp)     | Returns the value of the first element in an array that pass a test |
| [findIndex()](https://www.w3schools.com/jsref/jsref_findindex.asp) | Returns the index of the first element in an array that pass a test |
| [forEach()](https://www.w3schools.com/jsref/jsref_foreach.asp) | Calls a function for each array element                      |
| [from()](https://www.w3schools.com/jsref/jsref_from.asp)     | Creates an array from an object                              |
| [includes()](https://www.w3schools.com/jsref/jsref_includes_array.asp) | Check if an array contains the specified element             |
| [indexOf()](https://www.w3schools.com/jsref/jsref_indexof_array.asp) | Search the array for an element and returns its position     |
| [isArray()](https://www.w3schools.com/jsref/jsref_isarray.asp) | Checks whether an object is an array                         |
| [join()](https://www.w3schools.com/jsref/jsref_join.asp)     | Joins all elements of an array into a string                 |
| [keys()](https://www.w3schools.com/jsref/jsref_keys.asp)     | Returns a Array Iteration Object, containing the keys of the original array |
| [lastIndexOf()](https://www.w3schools.com/jsref/jsref_lastindexof_array.asp) | Search the array for an element, starting at the end, and returns its position |
| [map()](https://www.w3schools.com/jsref/jsref_map.asp)       | Creates a new array with the result of calling a function for each array element |
| [pop()](https://www.w3schools.com/jsref/jsref_pop.asp)       | Removes the last element of an array, and returns that element |
| [push()](https://www.w3schools.com/jsref/jsref_push.asp)     | Adds new elements to the end of an array, and returns the new length |
| [reduce()](https://www.w3schools.com/jsref/jsref_reduce.asp) | Reduce the values of an array to a single value (going left-to-right) |
| [reduceRight()](https://www.w3schools.com/jsref/jsref_reduceright.asp) | Reduce the values of an array to a single value (going right-to-left) |
| [reverse()](https://www.w3schools.com/jsref/jsref_reverse.asp) | Reverses the order of the elements in an array               |
| [shift()](https://www.w3schools.com/jsref/jsref_shift.asp)   | Removes the first element of an array, and returns that element |
| [slice()](https://www.w3schools.com/jsref/jsref_slice_array.asp) | Selects a part of an array, and returns the new array        |
| [some()](https://www.w3schools.com/jsref/jsref_some.asp)     | Checks if any of the elements in an array pass a test        |
| [sort()](https://www.w3schools.com/jsref/jsref_sort.asp)     | Sorts the elements of an array                               |
| [splice()](https://www.w3schools.com/jsref/jsref_splice.asp) | Adds/Removes elements from an array                          |
| [toString()](https://www.w3schools.com/jsref/jsref_tostring_array.asp) | Converts an array to a string, and returns the result        |
| [unshift()](https://www.w3schools.com/jsref/jsref_unshift.asp) | Adds new elements to the beginning of an array, and returns the new length |
| [valueOf()](https://www.w3schools.com/jsref/jsref_valueof_array.asp) | Returns the primitive value of an array                      |

## JavaScript Array Properties

| Property                                                     | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [constructor](https://www.w3schools.com/jsref/jsref_constructor_array.asp) | Returns the function that created the Array object's prototype |
| [length](https://www.w3schools.com/jsref/jsref_length_array.asp) | Sets or returns the number of elements in an array           |
| [prototype](https://www.w3schools.com/jsref/jsref_prototype_array.asp) | Allows you to add properties and methods to an Array object  |