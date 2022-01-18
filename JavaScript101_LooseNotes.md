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

`char1 === char2`

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

## JavaScript Arrays

An array is a special variable, which can hold more than one value:

````javascript
const starterPokemon = ["Charmander", "Bulbasaur", "Squirtle"];
````

If you have a list of items (a list of Pokémon names, for example), storing the Pokémon in single variables could look like this

````javascript
let starterPokemon1 = "Charmander";
let starterPokemon2 = "Bulbasaur";
let starterPokemon3 = "Squirtle";
````

However, what if you want to loop through the Pokémon and find a specific one? And what if you had not 3 Pokémon, but 150?

The solution is an array!

An array can hold many values under a single name, and you can access the values by referring to an index number.

Using an array literal is the easiest way to create a JavaScript Array.

Syntax:

````javascript
const array_name = [item1, item2, ...];    
````

It is a common practice to declare arrays with the const keyword.

Spaces and line breaks are not important. A declaration can span multiple lines:

````javascript
const starterPokemon = [
    "Charmander", 
    "Bulbasaur", 
    "Squirtle"
];
````

You can also create an array, and then provide the elements:

````javascript
const starterPokemon = [];
starterPokemon1 = "Charmander"; 
starterPokemon2 = "Bulbasaur"; 
starterPokemon3 = "Squirtle";
````

The following example also creates an Array, and assigns values to it:

````javascript
const starterPokemon = new Array("Charmander", "Bulbasaur", "Squirtle");
````

The two examples above do exactly the same.

There is no need to use `new Array()`.

For simplicity, readability and execution speed, use the array literal method.

You access an array element by referring to the **index number**:

````javascript
const starterPokemon = ["Charmander", "Bulbasaur", "Squirtle"];
let individualStarterPokemon = starterPokemon[0];
````

**Note:** Array indexes start with 0.

[0] is the first element. [1] is the second element.

This statement changes the value of the first element in `starterPokemon`:

````javascript
starterPokemon[0] = "Pikachu";
````

Arrays are a special type of objects. The `typeof` operator in JavaScript returns "object" for arrays.

But, JavaScript arrays are best described as arrays.

Arrays use **numbers** to access its "elements". In this example, `starterPokemon[0]` returns Charmander:

````javascript
const starterPokemon = ["Charmander", "Bulbasaur", "Squirtle"];
````

Warning !

Array elements can be deleted using the JavaScript operator `delete`.

Using `delete` leaves `undefined` holes in the array.

Use pop() or shift() instead.

By default, the `sort()` function sorts values as **strings**.

This works well for strings ("Apple" comes before "Banana").

However, if numbers are sorted as strings, "25" is bigger than "100", because "2" is bigger than "1".

Because of this, the `sort()` method will produce incorrect result when sorting numbers.



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

The Difference Between Arrays and Objects

In JavaScript, **arrays** use **numbered indexes**. 

In JavaScript, **objects** use **named indexes**.

Arrays are a special kind of objects, with numbered indexes.

When to Use Arrays. When to use Objects.

- JavaScript does not support associative arrays.
- You should use **objects** when you want the element names to be **strings (text)**.
- You should use **arrays** when you want the element names to be **numbers**.

Loops can execute a block of code a number of times.

## JavaScript Loops

Loops are handy, if you want to run the same code over and over again, each time with a different value.

````javascript
//instead of writing
text += starterPokemon[0] + "<br>";
text += starterPokemon[1] + "<br>";
text += starterPokemon[2] + "<br>";
text += starterPokemon[3] + "<br>";
text += starterPokemon[4] + "<br>";
text += starterPokemon[5] + "<br>";
//You can write:
for (let i = 0; i < starterPokemon.length; i++) {
  text += starterPokemon[i] + "<br>";
}
````

Different Kinds of Loops

JavaScript supports different kinds of loops:

- `for` - loops through a block of code a number of times
- `for/in` - loops through the properties of an object
- `for/of` - loops through the values of an iterable object
- `while` - loops through a block of code while a specified condition is true
- `do/while` - also loops through a block of code while a specified condition is true

The For Loop

The `for` loop has the following syntax:

````javascript
for (*statement 1*; *statement 2*; *statement 3*) {
 // *code block to be executed*
}
````

**Statement 1** is executed (one time) before the execution of the code block.

**Statement 2** defines the condition for executing the code block.

**Statement 3** is executed (every time) after the code block has been executed.

````javascript
for (let i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}
````

From the example above, you can read:

Statement 1 sets a variable before the loop starts (let i = 0).

Statement 2 defines the condition for the loop to run (i must be less than 5).

Statement 3 increases a value (i++) each time the code block in the loop has been executed.

**<u>Statement 1</u>**

Normally you will use statement 1 to initialize the variable used in the loop (let i = 0).

This is not always the case, JavaScript doesn't care. Statement 1 is optional.

You can initiate many values in statement 1 (separated by comma):

````javascript
for (let i = 0, len = starterPokemon.length, text = ""; i < len; i++) {
  text += starterPokemon[i] + "<br>";
}
````

And you can omit statement 1 (like when your values are set before the loop starts)

````javascript
let i = 2;
let len = starterPokemon.length;
let text = "";
for (; i < len; i++) {
  text += starterPokemon[i] + "<br>";
}
````

**<u>Statement 2</u>**

Often statement 2 is used to evaluate the condition of the initial variable.

This is not always the case, JavaScript doesn't care. Statement 2 is also optional.

If statement 2 returns true, the loop will start over again, if it returns false, the loop will end.

If you omit statement 2, you must provide a **break** inside the loop. Otherwise the loop will never end. This will crash your browser. Read about breaks in a later chapter of this tutorial.

**<u>Statement 3</u>**

Often statement 3 increments the value of the initial variable.

This is not always the case, JavaScript doesn't care, and statement 3 is optional.

Statement 3 can do anything like negative increment (i--), positive increment (i = i + 15), or anything else.

Statement 3 can also be omitted (like when you increment your values inside the loop):

````javascript
let i = 0;
let len = starterPokemon.length;
let text = "";
for (; i < len; ) {
  text += starterPokemon[i] + "<br>";
  i++;
}
````

Loop Scope

Using `var` in a loop:

````javascript
var i = 5;

for (var i = 0; i < 10; i++) {
  // some code
}

// Here i is 10
````

Using `let` in a loop:

````javascript
let i = 5;

for (let i = 0; i < 10; i++) {
  // some code
}

// Here i is 5
````

In the first example, using `var`, the variable declared in the loop redeclares the variable outside the loop.

In the second example, using `let`, the variable declared in the loop does not redeclare the variable outside the loop.

When `let` is used to declare the i variable in a loop, the i variable will only be visible within the loop.

The For In Loop

The JavaScript `for in` statement loops through the properties of an Object:

````javascript
for (key in object) {
  // code block to be executed
}
````

- The **for in** loop iterates over a **person** object
- Each iteration returns a **key** (x)
- The key is used to access the **value** of the key
- The value of the key is **person[x]**

````javascript
const person = {fname:"John", lname:"Doe", age:25};

let text = "";
for (let x in person) {
  text += person[x];
}
````

For In Over Arrays

The JavaScript `for in` statement can also loop over the properties of an Array:

````javascript
for (variable in array) {
  code
}
````

````javascript
const numbers = [45, 4, 9, 16, 25];

let txt = "";
for (let x in numbers) {
  txt += numbers[x];
}
````

Do not use **for in** over an Array if the index **order** is important.

The index order is implementation-dependent, and array values may not be accessed in the order you expect.

It is better to use a **for** loop, a **for of** loop, or **Array.forEach()** when the order is important.

The `forEach()` method calls a function (a callback function) once for each array element.

````javascript
const numbers = [45, 4, 9, 16, 25];

let txt = "";
numbers.forEach(myFunction);

function myFunction(value, index, array) {
  txt += value;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

The JavaScript `for of` statement loops through the values of an iterable object.

It lets you loop over iterable data structures such as Arrays, Strings, Maps, NodeLists, and more:

````javascript
for (variable of iterable) {
  // code block to be executed
}
````

**variable** - For every iteration the value of the next property is assigned to the variable. *Variable* can be declared with `const`, `let`, or `var`.

**iterable** - An object that has iterable properties.

**For/of** is not supported in Internet Explorer.

Looping over an Array:

````javascript
const cars = ["BMW", "Volvo", "Mini"];

let text = "";
for (let x of cars) {
  text += x;
}
````

Looping over a string

````javascript
let language = "JavaScript";

let text = "";
for (let x of language) {
text += x;
}
````

The `while` loop loops through a block of code as long as a specified condition is true.

We can use the `while` loop to create any type of iteration we wish, including anything that we have previously done with a `for` loop. 

````javascript
while (condition) {
  // code block to be executed
}
````

````javascript
//for loop
for (let i = 0; i < 51; i++) {
   console.log(i);
}
//while loop
let i = 0;

while (i < 51) {
   console.log(i);
   i++;
}
````

If you forget to increase the variable used in the condition, the loop will never end. This will crash your browser.

The `do while` loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

````javascript
do {
  // code block to be executed
}
while (condition);
````

The example below uses a `do while` loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested

````javascript
do {
  text += "The number is " + i;
  i++;
}
while (i < 10);
````

Do not forget to increase the variable used in the condition, otherwise the loop will never end!

## JavaScript Array Iteration

Array iteration methods operate on every array item.

The Array forEach() Method

The `forEach()` method calls a function (a callback function) once for each array element.

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

The example above uses only the value parameter. The example can be rewritten to:

````javascript
const numbers = [45, 4, 9, 16, 25];
let txt = "";
numbers.forEach(myFunction);

function myFunction(value) {
 txt += value + "<br>";
}
````

The Array map() Method

The `map()` method creates a new array by performing a function on each array element.

The `map()` method does not execute the function for array elements without values.

The `map()` method does not change the original array.

This example multiplies each array value by 2:

````javascript
const numbers1 = [45, 4, 9, 16, 25];
const numbers2 = numbers1.map(myFunction);

function myFunction(value, index, array) {
 return value * 2;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

When a callback function uses only the value parameter, the index and array parameters can be omitted:

````javascript
const numbers1 = [45, 4, 9, 16, 25];
const numbers2 = numbers1.map(myFunction);

function myFunction(value) {
 return value * 2;
}
````

The Array filter() Method

The `filter()` method creates a new array with array elements that passes a test.

This example creates a new array from elements with a value larger than 18:

````javascript
const numbers = [45, 4, 9, 16, 25];
const over18 = numbers.filter(myFunction);

function myFunction(value, index, array) {
 return value > 18;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

In the example above, the callback function does not use the index and array parameters, so they can be omitted:

````javascript
const numbers = [45, 4, 9, 16, 25];
const over18 = numbers.filter(myFunction);

function myFunction(value) {
 return value > 18;
}
````

The Array reduce() Method

The `reduce()` method runs a function on each array element to produce (reduce it to) a single value.

The `reduce()` method works from left-to-right in the array. See also `reduceRight()`.

The `reduce()` method does not reduce the original array.

This example finds the sum of all numbers in an array:

````javascript
const numbers = [45, 4, 9, 16, 25];
let sum = numbers.reduce(myFunction);

function myFunction(total, value, index, array) {
 return total + value;
}
````

Note that the function takes 4 arguments:

- The total (the initial value / previously returned value)
- The item value
- The item index
- The array itself

The example above does not use the index and array parameters. It can be rewritten to:

````javascript
const numbers = [45, 4, 9, 16, 25];
let sum = numbers.reduce(myFunction);

function myFunction(total, value) {
 return total + value;
}
````

The `reduce()` method can accept an initial value:

````javascript
const numbers = [45, 4, 9, 16, 25];
let sum = numbers.reduce(myFunction, 100);

function myFunction(total, value) {
 return total + value;
}
````

The Array reduceRight() Method

The `reduceRight()` method runs a function on each array element to produce (reduce it to) a single value.

The `reduceRight()` works from right-to-left in the array. See also `reduce()`.

The `reduceRight()` method does not reduce the original array.

This example finds the sum of all numbers in an array:

````javascript
const numbers = [45, 4, 9, 16, 25];
let sum = numbers1.reduceRight(myFunction);

function myFunction(total, value, index, array) {
 return total + value;
}
````

Note that the function takes 4 arguments:

- The total (the initial value / previously returned value)
- The item value
- The item index
- The array itself

The example above does not use the index and array parameters. It can be rewritten to:

````javascript
const numbers = [45, 4, 9, 16, 25];
let sum = numbers1.reduceRight(myFunction);

function myFunction(total, value) {
 return total + value;
}
````

The Array every() Method

The `every()` method check if all array values pass a test.

This example check if all array values are larger than 18:

````javascript
const numbers = [45, 4, 9, 16, 25];
let allOver18 = numbers.every(myFunction);

function myFunction(value, index, array) {
 return value > 18;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

When a callback function uses the first parameter only (value), the other parameters can be omitted:

````javascript
const numbers = [45, 4, 9, 16, 25];
let allOver18 = numbers.every(myFunction);

function myFunction(value) {
 return value > 18;
}
````

The Array some() Method

The `some()` method check if some array values pass a test.

This example check if some array values are larger than 18:

````javascript
const numbers = [45, 4, 9, 16, 25];
let someOver18 = numbers.some(myFunction);

function myFunction(value, index, array) {
 return value > 18;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

The Array indexOf() Method

The `indexOf()` method searches an array for an element value and returns its position.

**Note:** The first item has position 0, the second item has position 1, and so on.

Search an array for the item "Apple":

````javascript
const fruits = ["Apple", "Orange", "Apple", "Mango"];
let position = fruits.indexOf("Apple") + 1;
````

*array*.indexOf(*item*, *start*)

| *item*  | Required. The item to search for.                            |
| ------- | ------------------------------------------------------------ |
| *start* | Optional. Where to start the search. Negative values will start at the given position counting from the end, and search to the end. |

`Array.indexOf()` returns -1 if the item is not found.

If the item is present more than once, it returns the position of the first occurrence.

The Array lastIndexOf() Method

`Array.lastIndexOf()` is the same as `Array.indexOf()`, but returns the position of the last occurrence of the specified element.

Search an array for the item "Apple":

````javascript
const fruits = ["Apple", "Orange", "Apple", "Mango"];
let position = fruits.lastIndexOf("Apple") + 1;
````

*array*.lastIndexOf(*item*, *start*)

| *item*  | Required. The item to search for                             |
| ------- | ------------------------------------------------------------ |
| *start* | Optional. Where to start the search. Negative values will start at the given position counting from the end, and search to the beginning |

------

The Array includes() Method

ECMAScript 2016 introduced `Array.includes()` to arrays. This allows us to check if an element is present in an array (including NaN, unlike indexOf).

````javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];

fruits.includes("Mango"); // is true
````

*array*.includes(*search-item*)

Array.includes() allows to check for NaN values. Unlike Array.indexOf().

The first browser versions with full support are:

The Array find() Method

The `find()` method returns the value of the first array element that passes a test function.

This example finds (returns the value of) the first element that is larger than 18:

````javascript
const numbers = [4, 9, 16, 25, 29];
let first = numbers.find(myFunction);

function myFunction(value, index, array) {
 return value > 18;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

The Array findIndex() Method

The `findIndex()` method returns the index of the first array element that passes a test function.

This example finds the index of the first element that is larger than 18:

````javascript
const numbers = [4, 9, 16, 25, 29];
let first = numbers.findIndex(myFunction);

function myFunction(value, index, array) {
 return value > 18;
}
````

Note that the function takes 3 arguments:

- The item value
- The item index
- The array itself

The Array.from() Method

The `Array.from()` method returns an Array object from any object with a length property or any iterable object.

Create an Array from a String:

````javascript
Array.from("ABCDEFG")  // Returns [A,B,C,D,E,F,G]
````

The Array Keys() Method

The `Array.keys()` method returns an Array Iterator object with the keys of an array.

Create an Array Iterator object, containing the keys of the array:

````javascript
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const keys = fruits.keys();

for (let x of keys) {
 text += x + "<br>";
}
````

## JavaScript Objects

A Pokémon is an **object**.

A Pokémon has **properties** like name and type, and **methods** like usemoves and outofpokeball:

| Object                                                       | Properties                                                   | Methods                                                      |
| :----------------------------------------------------------- | ------------------------------------------------------------ | :----------------------------------------------------------- |
| ![image-20220104121535601](C:\Users\Heather\AppData\Roaming\Typora\typora-user-images\image-20220104121535601.png) | pokemon.name = Togepi  pokemon.type = Normal  pokemon.id = 175  pokemon.generation = II | pokemon.outofpokeball()  pokemon.caught()  pokemon.intopokeball()  pokemon.usemoves() |

All Pokémon have the same **properties**, but the property **values** differ from Pokémon to Pokémon.

All Pokémon have the same **methods**, but the methods are performed **at different times**.

JavaScript variables are containers for data values.

````javascript
let pokemon = "Togepi";
````

Objects are variables too. But objects can contain many values.

This code assigns **many values** (Togepi, Normal, 175) to a **variable** named pokemon:

````javascript
const pokemon = {pokemon.name: "Togepi",  pokemon.type: "Normal",  pokemon.id: 175  pokemon.generation: "II"};
````

The values are written as **name:value** pairs (name and value separated by a colon).

It is a common practice to declare objects with the const keyword.

You define (and create) a JavaScript object with an object literal:

````javascript
const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
````

Spaces and line breaks are not important. An object definition can span multiple lines:

````javascript
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
````

The **name:values** pairs in JavaScript objects are called **properties**:

| Property  | Property Value |
| :-------- | :------------- |
| firstName | John           |
| lastName  | Doe            |
| age       | 50             |
| eyeColor  | blue           |

You can access object properties in two ways:

````javascript
objectName.propertyName
//or
objectName["propertyName"]
````

JavaScript objects are containers for **named values** called properties.

Objects can also have **methods**.

Methods are **actions** that can be performed on objects.

Methods are stored in properties as **function definitions**.

| Property  | Property Value                                            |
| :-------- | :-------------------------------------------------------- |
| firstName | John                                                      |
| lastName  | Doe                                                       |
| age       | 50                                                        |
| eyeColor  | blue                                                      |
| fullName  | function() {return this.firstName + " " + this.lastName;} |

A method is a function stored as a property.

````javascript
const person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
````

In a function definition, `this` refers to the "owner" of the function.

In the example above, `this` is the **person object** that "owns" the `fullName` function.

In other words, `this.firstName` means the `firstName` property of **this object**.

You access an object method with the following syntax:

````javascript
//objectName.methodName()
//Example
const name = person.fullName(); 
````

If you access a method **without** the () parentheses, it will return the **function definition**:

````javascript
const name = person.fullName;
````

When a JavaScript variable is declared with the keyword "`new`", the variable is created as an object:

````javascript
x = new String();        // Declares x as a String object
y = new Number();        // Declares y as a Number object
z = new Boolean();       // Declares z as a Boolean object
````

Avoid `String`, `Number`, and `Boolean` objects. They complicate your code and slow down execution speed.

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
let myStr = "Hello World";
myVar.toUpperCase();
````

One may think after the first line the *myVar* will become “HELLO WORLD”, but it still equals to “Hello World”. The method will return a new String object it will not change the existing String reference. So we have to assign it to a new variable to get the desired value.

````javascript
let myStrUpperCase = myStr.toUpperCase();
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
let myStr = "Hello";
myVar[0] = "i";//still myVar remains same
````

String object has many methods which deal with string characters and all of them returns a new String object instead of modifying the String object on which they are called.

## JavaScript Math Object

The JavaScript Math object allows you to perform mathematical tasks on numbers.

Unlike other objects, the Math object has no constructor.

The Math object is static.

All methods and properties can be used without creating a Math object first.

The syntax for any Math property is : `Math.*property*`.

JavaScript provides 8 mathematical constants that can be accessed as Math properties:

````javascript
Math.E        // returns Euler's number
Math.PI       // returns PI
Math.SQRT2    // returns the square root of 2
Math.SQRT1_2  // returns the square root of 1/2
Math.LN2      // returns the natural logarithm of 2
Math.LN10     // returns the natural logarithm of 10
Math.LOG2E    // returns base 2 logarithm of E
Math.LOG10E   // returns base 10 logarithm of E
````

The syntax for Math any methods is : `Math.*method*(*number*)`

| Method                                                       | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [abs(x)](https://www.w3schools.com/jsref/jsref_abs.asp)      | Returns the absolute value of x                              |
| [acos(x)](https://www.w3schools.com/jsref/jsref_acos.asp)    | Returns the arccosine of x, in radians                       |
| [acosh(x)](https://www.w3schools.com/jsref/jsref_acosh.asp)  | Returns the hyperbolic arccosine of x                        |
| [asin(x)](https://www.w3schools.com/jsref/jsref_asin.asp)    | Returns the arcsine of x, in radians                         |
| [asinh(x)](https://www.w3schools.com/jsref/jsref_asinh.asp)  | Returns the hyperbolic arcsine of x                          |
| [atan(x)](https://www.w3schools.com/jsref/jsref_atan.asp)    | Returns the arctangent of x as a numeric value between -PI/2 and PI/2 radians |
| [atan2(y, x)](https://www.w3schools.com/jsref/jsref_atan2.asp) | Returns the arctangent of the quotient of its arguments      |
| [atanh(x)](https://www.w3schools.com/jsref/jsref_atanh.asp)  | Returns the hyperbolic arctangent of x                       |
| [cbrt(x)](https://www.w3schools.com/jsref/jsref_cbrt.asp)    | Returns the cubic root of x                                  |
| [ceil(x)](https://www.w3schools.com/jsref/jsref_ceil.asp)    | Returns x, rounded upwards to the nearest integer            |
| [cos(x)](https://www.w3schools.com/jsref/jsref_cos.asp)      | Returns the cosine of x (x is in radians)                    |
| [cosh(x)](https://www.w3schools.com/jsref/jsref_cosh.asp)    | Returns the hyperbolic cosine of x                           |
| [exp(x)](https://www.w3schools.com/jsref/jsref_exp.asp)      | Returns the value of Ex                                      |
| [floor(x)](https://www.w3schools.com/jsref/jsref_floor.asp)  | Returns x, rounded downwards to the nearest integer          |
| [log(x)](https://www.w3schools.com/jsref/jsref_log.asp)      | Returns the natural logarithm (base E) of x                  |
| [max(x, y, z, ..., n)](https://www.w3schools.com/jsref/jsref_max.asp) | Returns the number with the highest value                    |
| [min(x, y, z, ..., n)](https://www.w3schools.com/jsref/jsref_min.asp) | Returns the number with the lowest value                     |
| [pow(x, y)](https://www.w3schools.com/jsref/jsref_pow.asp)   | Returns the value of x to the power of y                     |
| [random()](https://www.w3schools.com/jsref/jsref_random.asp) | Returns a random number between 0 and 1                      |
| [round(x)](https://www.w3schools.com/jsref/jsref_round.asp)  | Rounds x to the nearest integer                              |
| [sign(x)](https://www.w3schools.com/jsref/jsref_sign.asp)    | Returns if x is negative, null or positive (-1, 0, 1)        |
| [sin(x)](https://www.w3schools.com/jsref/jsref_sin.asp)      | Returns the sine of x (x is in radians)                      |
| [sinh(x)](https://www.w3schools.com/jsref/jsref_sinh.asp)    | Returns the hyperbolic sine of x                             |
| [sqrt(x)](https://www.w3schools.com/jsref/jsref_sqrt.asp)    | Returns the square root of x                                 |
| [tan(x)](https://www.w3schools.com/jsref/jsref_tan.asp)      | Returns the tangent of an angle                              |
| [tanh(x)](https://www.w3schools.com/jsref/jsref_tanh.asp)    | Returns the hyperbolic tangent of a number                   |
| [trunc(x)](https://www.w3schools.com/jsref/jsref_trunc.asp)  | Returns the integer part of a number (x)                     |

## JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

````javascript
function myFunction(p1, p2) {
  return p1 * p2;   // The function returns the product of p1 and p2
}
````

A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
**(\*parameter1, parameter2, ...\*)**

The code to be executed, by the function, is placed inside curly brackets: **{}**

````javascript
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
````

Function **parameters** are listed inside the parentheses () in the function definition.

Function **arguments** are the **values** received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

The code inside the function will execute when "something" **invokes** (calls) the function:

- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

When JavaScript reaches a `return` statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a **return value**. The return value is "returned" back to the "caller"

````javascript
let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
} //value of x = 12
````

With functions you can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.

Accessing a function without () will return the function object instead of the function result.

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

````javascript
//Instead of using a variable to store the return value of a function:
let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";
//You can use the function directly, as a variable value:
let text = "The temperature is " + toCelsius(77) + " Celsius";
````

Variables declared within a JavaScript function, become **LOCAL** to the function.

Local variables can only be accessed from within the function.

````javascript
// code here can NOT use carName

function myFunction() {
  let carName = "Volvo";
  // code here CAN use carName
}

// code here can NOT use carName
````

Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.

Local variables are created when a function starts, and deleted when the function is completed.

While the function declaration above is syntactically a statement, functions can also be created by a function expression

Such a function can be **anonymous**; it does not have to have a name. For example, the function `square` could have been defined as:

Such a function can be **anonymous**; it does not have to have a name. For example, the function `square` could have been defined as:

````javascript
const square = function(number) { return number * number }
var x = square(4) // x gets the value 16
````

However, a name *can* be provided with a function expression. Providing a name allows the function to refer to itself, and also makes it easier to identify the function in a debugger's stack traces:

````javascript
const factorial = function fac(n) { return n < 2 ? 1 : n * fac(n - 1) }
console.log(factorial(3))
````

Function expressions are convenient when passing a function as an argument to another function. The following example shows a `map` function that should receive a function as first argument and an array as second argument:

````javascript
function map(f, a) {
  let result = []; // Create a new Array
  let i; // Declare variable
  for (i = 0; i != a.length; i++)
    result[i] = f(a[i]);
  return result;
}
````

In the following code, the function receives a function defined by a function expression and executes it for every element of the array received as a second argument:

````javascript
function map(f, a) {
  let result = []; // Create a new Array
  let i; // Declare variable
  for (i = 0; i != a.length; i++)
    result[i] = f(a[i]);
  return result;
}
const f = function(x) {
   return x * x * x;
}
let numbers = [0, 1, 2, 5, 10];
let cube = map(f,numbers);
console.log(cube); //Function returns: [0, 1, 8, 125, 1000].
````

In JavaScript, a function can be defined based on a condition. For example, the following function definition defines `myFunc` only if `num` equals `0`:

````javascript
var myFunc;
if (num === 0) {
  myFunc = function(theObject) {
    theObject.make = 'Toyota';
  }
}
````

In addition to defining functions as described here, you can also use the [`Function`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function) constructor to create functions from a string at runtime, much like [`eval()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/eval).

A **method** is a function that is a property of an object. 

*Defining* a function does not *execute* it. Defining it names the function and specifies what to do when the function is called.

**Calling** the function actually performs the specified actions with the indicated parameters. For example, if you define the function `square`, you could call it as follows:

````javascript
square(5); //The preceding statement calls the function with an argument of 5. The function executes its statements and returns the value 25
````

Functions must be *in scope* when they are called, but the function declaration can be hoisted (appear below the call in the code), as in this example:

````javascript
console.log(square(5));
/* ... */
function square(n) { return n * n }
````

The arguments of a function are not limited to strings and numbers. You can pass whole objects to a function.

There are other ways to call functions. There are often cases where a function needs to be called dynamically, or the number of arguments to a function vary, or in which the context of the function call needs to be set to a specific object determined at runtime.

It turns out that *functions are themselves objects*—and in turn, these objects have methods.

Every JavaScript function is actually a `Function` object. This can be seen with the code `(function(){}).constructor === Function`, which returns true.

Constructor

- [`Function()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/Function)

  Creates a new `Function` object. Calling the constructor directly can create functions dynamically but suffers from security and similar (but far less significant) performance issues to [`Global_Objects/eval`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/eval). However, unlike eval, the `Function` constructor creates functions that execute in the global scope only.

Instance properties

- [`Function.prototype.arguments`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/arguments)

  An array corresponding to the arguments passed to a function. This is deprecated as a property of [`Function`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function). Use the [`arguments`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments) object (available within the function) instead.

- [`Function.prototype.caller`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/caller)

  Specifies the function that invoked the currently executing function. This property is deprecated, and is only functional for some non-strict functions.

- [`Function.prototype.displayName`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/displayName)

  The display name of the function.

- [`Function.prototype.length`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/length)

  Specifies the number of arguments expected by the function.

- [`Function.prototype.name`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/name)

  The name of the function.

Instance methods

- `Function.prototype.apply(thisArg [, argsArray\])`

  Calls a function and sets its `this` to the provided `thisArg`. Arguments can be passed as an [`Array`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) object.

- `Function.prototype.bind(thisArg[, arg1[, arg2[, ...argN\]]])`

  Creates a new function which, when called, has its `this` set to the provided `thisArg`. Optionally, a given sequence of arguments will be prepended to arguments provided the newly-bound function is called.

- `Function.prototype.call(thisArg[, arg1, arg2, ...argN\])`

  Calls a function and sets its `this` to the provided value. Arguments can be passed as they are.

- `Function.prototype.toString()`

  Returns a string representing the source code of the function. Overrides the [`Object.prototype.toString`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/toString) method.

Difference between Function constructor and function declaration

Functions created with the `Function` constructor do not create closures to their creation contexts; they always are created in the global scope. When running them, they will only be able to access their own local variables and global ones, not the ones from the scope in which the `Function` constructor was created. This is different from using [`Global_Objects/eval`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/eval) with code for a function expression.

```javascript
let x = 10;

function createFunction1() {
    let x = 20;
    return new Function('return x;'); // this |x| refers global |x|
}

function createFunction2() {
    let x = 20;
    function f() {
        return x; // this |x| refers local |x| above
    }
    return f;
}

let f1 = createFunction1();
console.log(f1());          // 10
let f2 = createFunction2();
console.log(f2());          // 20
```

While this code works in web browsers, `f1()` will produce a `ReferenceError` in Node.js, as `x` will not be found. This is because the top-level scope in Node is not the global scope, and `x` will be local to the module.

## JavaScript Scope

Scope is the accessibility of variables, functions, and objects in some particular part of your code during runtime. In other words, scope determines the visibility of variables and other resources in areas of your code.

Understanding `scope` will make your code stand out, reduce errors and help you make powerful design patterns with it.

In the JavaScript language there are two types of scopes:

- Global Scope
- Local Scope

Variables defined **inside a function** are in local scope while variables defined outside of a function are in the global scope. Each function when invoked creates a new scope.

When you start writing JavaScript in a document, you are already in the Global scope. There is only one Global scope throughout a JavaScript document. A variable is in the Global scope if it’s defined outside of a function.

````javascript
// the scope is by default global
let name = 'Link';
````

Variables inside the Global scope can be accessed and altered in any other scope.

````javascript
let name = 'Link';

console.log(name); // logs 'Link'

function logName() {
    console.log(name); // 'name' is accessible here and everywhere else
}

logName(); // logs 'Link'
````

Variables defined inside a function are in the local scope. And they have a different scope for every call of that function. This means that variables having the same name can be used in different functions. This is because those variables are bound to their respective functions, each having different scopes, and are not accessible in other functions.

````javascript
// Global Scope
function someFunction() {
    // Local Scope #1
    function someOtherFunction() {
        // Local Scope #2
    }
}

// Global Scope
function anotherFunction() {
    // Local Scope #3
}
// Global Scope
````

Block statements like `if` and `switch` conditions or `for` and `while` loops, unlike functions, don’t create a new scope. Variables defined inside of a block statement will remain in the scope they were already in.

```javascript
if (true) {
    // this 'if' conditional block doesn't create a new scope
    let name = 'Link'; // name is still in the global scope
}

console.log(name); // logs 'Link'
```

Global scope lives as long as your application lives. Local Scope lives as long as your functions are called and executed.

Lexical Scope means that in a nested group of functions, the inner functions have access to the variables and other resources of their parent scope. This means that the child functions are lexically bound to the execution context of their parents. Lexical scope is sometimes also referred to as Static Scope.

````javascript
function grandfather() {
    var name = 'Link';
    // likes is not accessible here
    function parent() {
        // name is accessible here
        // likes is not accessible here
        function child() {
            // Innermost level of the scope chain
            // name is also accessible here
            var likes = 'Rupees';
        }
    }
}
````

The thing you will notice about lexical scope is that it works forward, meaning `name` can be accessed by its children’s execution contexts. But it doesn’t work backward to its parents, meaning that the variable `likes` cannot be accessed by its parents. This also tells us that variables having the same name in different execution contexts gain precedence from top to bottom of the execution stack. A variable, having a name similar to another variable, in the innermost function (topmost context of the execution stack) will have higher precedence.

The concept of closures is closely related to Lexical Scope, which we studied above. A Closure is created when an inner function tries to access the scope chain of its outer function meaning the variables outside of the immediate lexical scope. Closures contain their own scope chain, the scope chain of their parents, and the global scope.

A closure can not only access the variables defined in its outer function but also the arguments of the outer function.

A closure can also access the variables of its outer function even after the function has returned. This allows the returned function to maintain access to all the resources of the outer function.

When you return an inner function from a function, that returned function will not be called when you try to call the outer function. You must first save the invocation of the outer function in a separate variable and then call the variable as a function. Consider this example:

````javascript
function sayHi() {
    name = 'Link';
    return function () {
        console.log('Hi ' + name);
    }
}

sayHi(); // nothing happens, no errors

// the returned function from sayHi() gets saved in greetPerson
greetPerson = sayHi();

 // calling greetPerson calls the returned function from the sayHi() function
greetPerson(); // logs 'Hi Link'
````

The key thing to note here is the `greetPerson` function can access the name variable of the `greet` function even after it has been returned. One way to call the returned function from the `sayHi` function without variable assignment is by using parentheses `()` two times `()()` like this:

````javascript
function sayHi() {
    name = 'Link';
    return function () {
        console.log('Hi ' + name);
    }
}

sayHi()(); // logs 'Hi Link'
````

## The JavaScript *this* Keyword

````javascript
const person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
````

The JavaScript `this` keyword refers to the object it belongs to.

It has different values depending on where it is used:

- In a method, `this` refers to the **owner object**.
- Alone, `this` refers to the **global object**.
- In a function, `this` refers to the **global object**.
- In a function, in strict mode, `this` is `undefined`.
- In an event, `this` refers to the **element** that received the event.
- Methods like `call()`, and `apply()` can refer `this` to **any object**.

In an object method, `this` refers to the "**owner**" of the method.

In the example on the top of this page, `this` refers to the **person** object.

The **person** object is the **owner** of the **fullName** method.

````javascript
fullName : function() {
  return this.firstName + " " + this.lastName;
}
````

When used alone, the **owner** is the Global object, so `this` refers to the Global object.

In a browser window the Global object is `[object Window]`:

````javascript
let x = this;
````

In **strict mode**, when used alone, `this` also refers to the Global object `[object Window]`:

````javascript
"use strict";
let x = this;
````

In a JavaScript function, the owner of the function is the **default** binding for `this`.

So, in a function, `this` refers to the Global object `[object Window]`.

````javascript
function myFunction() {
  return this;
}
````

JavaScript **strict mode** does not allow default binding.

So, when used in a function, in strict mode, `this` is `undefined`.

````javascript
"use strict";
function myFunction() {
  return this;
}
````

In these examples, `this` is the **person** object (The person object is the "owner" of the function):

````javascript
const person = {
  firstName  : "John",
  lastName   : "Doe",
  id         : 5566,
  myFunction : function() {
    return this;
  }
};
````

In other words: **this.firstName** means the **firstName** property of **this** (person) object.

## Explicit Function Binding

The `call()` and `apply()` methods are predefined JavaScript methods.

They can both be used to call an object method with another object as argument.

You can read more about `call()` and `apply()` later in this tutorial.

In the example below, when calling person1.fullName with person2 as argument, `this` will refer to person2, even if it is a method of person1:

````javascript
const person1 = {
 fullName: function() {
  return this.firstName + " " + this.lastName;
 }
}
const person2 = {
 firstName:"John",
 lastName: "Doe",
}
person1.fullName.call(person2); // Will return "John Doe"
````

## JavaScript Arrow Function

Arrow functions allow us to write shorter function syntax:

````javascript
//javascript function
hello = function() {
  return "Stardew Valley";
}
//javascript arrow function
hello = () => {
  return "Stardew Valley";
}
````

If the function has only one statement, and the statement returns a value, you can remove the brackets *and* the `return` keyword:

````javascript
hello = () => "Stardew Valley";
//Note: This works only if the function has only one statement.
````

If you have parameters, you pass them inside the parentheses:

````javascript
hello = val => "Hello " + val;
````

An **arrow function expression** is a compact alternative to a traditional [function expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function), but is limited and can't be used in all situations. Arrow function expressions are best suited for non-method functions. 

**Differences & Limitations:**

- Does not have its own bindings to [`this`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this) or [`super`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super), and should not be used as [`methods`](https://developer.mozilla.org/en-US/docs/Glossary/Method).
- Does not have [`new.target`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new.target) keyword.
- Not suitable for [`call`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/call), [`apply`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply) and [`bind`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind) methods, which generally rely on establishing a [scope](https://developer.mozilla.org/en-US/docs/Glossary/Scope).
- Can not be used as [constructors](https://developer.mozilla.org/en-US/docs/Glossary/Constructor).
- Can not use [`yield`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/yield), within its body.

Let's see what happens when we try to use them as methods:

````javascript
'use strict';

var obj = { // does not create a new scope
  i: 10,
  b: () => console.log(this.i, this),
  c: function() {
    console.log(this.i, this);
  }
}

obj.b(); // prints undefined, Window {...} (or the global object)
obj.c(); // prints 10, Object {...}
````



The handling of `this` is different in arrow functions compared to regular functions.

In short, with arrow functions there are no binding of `this`.

In regular functions the `this` keyword represented the object that called the function, which could be the window, the document, a button or whatever.

With arrow functions the `this` keyword *always* represents the object that defined the arrow function.

Perhaps the greatest benefit of using Arrow functions is with DOM-level methods (setTimeout, setInterval, addEventListener) that usually required some kind of closure, call, apply or bind to ensure the function executed in the proper scope.

Arrow functions can have either a "concise body" or the usual "block body".

In a concise body, only an expression is specified, which becomes the implicit return value. In a block body, you must use an explicit `return` statement.

````javascript
var func = x => x * x;
// concise body syntax, implied "return"

var func = (x, y) => { return x + y; };
// with block body, explicit "return" needed
````

## JavaScript Recursive Functions

A recursive function is a [function](https://www.javascripttutorial.net/javascript-function/) that calls itself until it doesn’t. And this technique is called recursion.

Suppose that you have a function called `recurse()`. The `recurse()` is a recursive function if it calls itself inside its body, like this:

```javascript
function recurse() {
    // ...
    recurse();
    // ...
}
```

A recursive function always has a condition to stop calling itself. Otherwise, it will call itself indefinitely. So a recursive function typically looks like the following:

```javascript
function recurse() {
    if(condition) {
        // stop calling itself
        //...
    } else {
        recurse();
    }
}
```

Generally, you use recursive functions to break down a big problem into smaller ones. Typically, you will find the recursive functions in data structures like binary trees and graphs and algorithms such as binary search and quicksort.

The following shows the `countDown()` function:

```javascript
function countDown(fromNumber) {
    console.log(fromNumber);
}
countDown(3);
```

This `countDown(3)` shows only the number 3.

To count down from the number 3 to 1, you can:

1. show the number 3.
2. and call the `countDown(2)` that shows the number 2.
3. and call the `countDown(1)` that shows the number 1.

The following changes the `countDown()` to a recursive function:

```javascript
function countDown(fromNumber) {
    console.log(fromNumber);
    countDown(fromNumber-1);
}
countDown(3);
```

This `countDown(3)` will run until the call stack size is exceeded, like this:

```javascript
Uncaught RangeError: Maximum call stack size exceeded.
```

… because it doesn’t have the condition to stop calling itself.

The count down will stop when the next number is zero. Therefore, we add an [if condition](https://www.javascripttutorial.net/javascript-if-else/) as follows:

```javascript
function countDown(fromNumber) {
    console.log(fromNumber);

    let nextNumber = fromNumber - 1;

    if (nextNumber > 0) {
        countDown(nextNumber);
    }
}
countDown(3);Code language: JavaScript (javascript)
/*
3
2
1
*/
```

The `countDown()` seems to work as expected.

However the function’s name is a reference to the actual function object.

If the function name is set to null somewhere in the code, the recursive function will stop working.

For example, the following code will result in an error:

```javascript
let newYearCountDown = countDown;
// somewhere in the code
countDown = null;
// the following function call will cause an error
newYearCountDown(10);
//error: Uncaught TypeError: countDown is not a function
```

How the script works:

- First, assign the `countDown` function name to the variable `newYearCountDown`.
- Second, set the `countDown` function reference to `null`.
- Third, call the `newYearCountDown` function.

The code causes an error because the body of the `countDown()` function references the `countDown` function name, which was set to `null` at the time of calling the function.

To fix it, you can use a named function expression as follows:

```javascript
let countDown = function f(fromNumber) {
    console.log(fromNumber);

    let nextNumber = fromNumber - 1;

    if (nextNumber > 0) {
        f(nextNumber);
    }
}

let newYearCountDown = countDown;
countDown = null;
newYearCountDown(10);
```

Given a number e.g., 324, calculate the sum of digits 3 + 2 + 4 = 9.

To apply the recursive technique, you can use the following steps:

```javascript
f(324) = 4 + f(32)
f(32)  = 2 + f(3)
f(3)   = 3  + 0 (stop here)
```

So

```javascript
f(324) = 4 + f(32) 
f(324) = 4 + 2 + f(3) 
f(324) = 4 + 2 + 3 
```

The following illustrates the `sumOfDigits()` recursive function:

```javascript
function sumOfDigits(num) {
    if (num == 0) {
        return 0;
    }
    return num % 10 + sumOfDigits(Math.floor(num / 10));
}Code language: JavaScript (javascript)
```

How it works:

- The `num%10` returns the remainder of the number after divided by 10, e.g., `324 % 10 = 4`
- The `Math.floor(num / 10)` returns the whole part of the `num / 10` e.g., `Math.floor(324 / 10) = 32`
- The `if(num == 0)` is a condition that stops calling the function.

Why Do I Need To Know Recursion? --- I like to watch people suffer lol jk.

## JavaScript Modules

As our application grows bigger, we want to split it into multiple files, so called “modules”. A module may contain a class or a library of functions for a specific purpose.

For a long time, JavaScript existed without a language-level module syntax. That wasn’t a problem, because initially scripts were small and simple, so there was no need.

But eventually scripts became more and more complex, so the community invented a variety of ways to organize code into modules, special libraries to load modules on demand.

The language-level module system appeared in the standard in 2015, gradually evolved since then, and is now supported by all major browsers and in Node.js. So we’ll study the modern JavaScript modules from now on.

A module is just a file. One script is one module. As simple as that.

Modules can load each other and use special directives `export` and `import` to interchange functionality, call functions of one module from another one:

- `export` keyword labels variables and functions that should be accessible from outside the current module.
- `import` allows the import of functionality from other modules.

For instance, if we have a file `sayHi.js` exporting a function:

```javascript
// 📁 sayHi.js
export function sayHi(user) {
  alert(`Hello, ${user}!`);
}
```

…Then another file may import and use it:

```javascript
// 📁 main.js
import {sayHi} from './sayHi.js';

alert(sayHi); // function...
sayHi('Link'); // Hello, Link!
```

The `import` directive loads the module by path `./sayHi.js` relative to the current file, and assigns exported function `sayHi` to the corresponding variable.

As modules support special keywords and features, we must tell the browser that a script should be treated as a module, by using the attribute `<script type="module">`.

```html
<!doctype html>
<script type="module">
  import {sayHi} from './say.js';

  document.body.innerHTML = sayHi('Link');
</script>
```

The browser automatically fetches and evaluates the imported module (and its imports if needed), and then runs the script.

**Modules work only via HTTP(s), not locally**

If you try to open a web-page locally, via `file://` protocol, you’ll find that `import/export` directives don’t work. Use a local web-server, such as [static-server](https://www.npmjs.com/package/static-server#getting-started) or use the “live server” capability of your editor, such as VS Code [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) to test modules.

Core module features

What’s different in modules, compared to “regular” scripts?

There are core features, valid both for browser and server-side JavaScript.

Always “use strict”

Modules always work in strict mode. E.g. assigning to an undeclared variable will give an error.

```html
<script type="module">
  a = 5; // error
</script>
```

Module-level scope

Each module has its own top-level scope. In other words, top-level variables and functions from a module are not seen in other scripts.

In the example below, two scripts are imported, and `hello.js` tries to use `user` variable declared in `user.js`. It fails, because it’s a separate module (you’ll see the error in the console):

```html
<!doctype html>
<script type="module" src="user.js"></script>
<script type="module" src="hello.js"></script>
```

Modules should `export` what they want to be accessible from outside and `import` what they need.

- `user.js` should export the `user` variable.
- `hello.js` should import it from `user.js` module.

In other words, with modules we use import/export instead of relying on global variables.

This is the correct variant:

```javascript
import {user} from './user.js';

document.body.innerHTML = user; // Link
```

In the browser, if we talk about HTML pages, independent top-level scope also exists for each `<script type="module">`.

Here are two scripts on the same page, both `type="module"`. They don’t see each other’s top-level variables:

```html
<script type="module">
  // The variable is only visible in this module script
  let user = "Link";
</script>

<script type="module">
  alert(user); // Error: user is not defined
</script>
```

**Please note:**

In the browser, we can make a variable window-level global by explicitly assigning it to a `window` property, e.g. `window.user = "Link"`.

Then all scripts will see it, both with `type="module"` and without it.

That said, making such global variables is frowned upon. Please try to avoid them.

A module code is evaluated only the first time when imported

If the same module is imported into multiple other modules, its code is executed only once, upon the first import. Then its exports are given to all further importers.

The one-time evaluation has important consequences, that we should be aware of.

First, if executing a module code brings side-effects, like showing a message, then importing it multiple times will trigger it only once – the first time:

```javascript
// 📁 alert.js
alert("Module is evaluated!");
// Import the same module from different files

// 📁 1.js
import `./alert.js`; // Module is evaluated!

// 📁 2.js
import `./alert.js`; // (shows nothing)
```

The second import shows nothing, because the module has already been evaluated.

There’s a rule: top-level module code should be, and used for initialization, creation of module-specific internal data structures. If we need to make something callable multiple times – we should export it as a function, like we did with `sayHi` above.

## JavaScript Classes

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.

Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.

One way to define a class is using a **class declaration**. To declare a class, you use the `class` keyword with the name of the class ("Rectangle" here).

```
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}
```

An important difference between function declarations and class declarations is that while functions can be called in code that appears before they are defined, classes must be defined before they can be constructed. Code like the following will throw a ReferenceError:

````javascript
const p = new Rectangle(); // ReferenceError

class Rectangle {}
````

This occurs because while the class is hoisted its values are not initialized.

A class expression is another way to define a class. Class expressions can be named or unnamed. The name given to a named class expression is local to the class's body. However, it can be accessed via the name property.

````javascript
// unnamed
let Rectangle = class {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};
console.log(Rectangle.name);
// output: "Rectangle"

// named
let Rectangle = class Rectangle2 {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};
console.log(Rectangle.name);
// output: "Rectangle2"
````

**Note:** Class **expressions** must be declared before they can be used (they are subject to the same hoisting restrictions as described in the [class declarations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes#class_declarations) section).

A JavaScript class is **not** an object.

It is a **template** for JavaScript objects.

When you have a class, you can use the class to create objects:

````javascript
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}

let myCar1 = new Car("Ford", 2014);
let myCar2 = new Car("Audi", 2019);
````

The example above uses the **Car class** to create two **Car objects**.

The constructor method is called automatically when a new object is created.

The constructor method is a special method:

- It has to have the exact name "constructor"
- It is executed automatically when a new object is created
- It is used to initialize object properties

If you do not define a constructor method, JavaScript will add an empty constructor method.

Class methods are created with the same syntax as object methods.

Use the keyword `class` to create a class.

Always add a `constructor()` method.

Then add any number of methods.

```javascript
//Rough Synax
class ClassName {
  constructor() { ... }
  method_1() { ... }
  method_2() { ... }
  method_3() { ... }
}
```

````javascript
//Class method named "age", that returns the Car age
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
  age() {
    let date = new Date();
    return date.getFullYear() - this.year;
  }
}

let myCar = new Car("Ford", 2014);
document.getElementById("demo").innerHTML =
"My car is " + myCar.age() + " years old.";

//You can send parameters to Class methods
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
  age(x) {
    return x - this.year;
  }
}

let date = new Date();
let year = date.getFullYear();

let myCar = new Car("Ford", 2014);
document.getElementById("demo").innerHTML=
"My car is " + myCar.age(year) + " years old.";
````

































HTML

In HTML event handlers, `this` refers to the HTML element that received the event:

````javascript
<button onclick="this.style.display='none'">
  Click to Remove Me!
</button>
````











Sources: (possibly not complete)

https://javascript.info

https://www.w3schools.com/

https://developer.mozilla.org/

https://www.freecodecamp.org/

https://stackoverflow.com/

https://dorey.github.io/JavaScript-Equality-Table/

