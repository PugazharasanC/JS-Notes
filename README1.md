# [JavaScript Cheat Sheet](https://drive.google.com/file/d/14mSzInQ674Drdu_iKULASF1XsCDKjJcm/view?usp=sharing)

# Variable
A value box that can be updated at any time and accessed whenever needed.

## How to Declare a Variable
Use the syntax `<keyword> <variable_name> = <value>;`.

For example:
```javascript
var num = 10;
```

# Keywords in JavaScript

Keywords in JavaScript are compiler-known words that are already defined in the programming language itself.

## List of Keywords:

```javascript
var, let, const, function, if, else, for, while, break, continue, switch, case, default, do, return, try, catch, throw, typeof, instanceof, new, delete, in, this, super, class, extends, export, import, async, await, yield, debugger, null, undefined, true, false, NaN, Infinity
```

These keywords play essential roles in defining the structure and behavior of JavaScript code.


# Data Types in JavaScript

 **Data Type** refers to the type of data we store in programming.

## Number
- Examples: 1, 2, 3, -1, -5, -100, 10.5, 25.65

## String
- Examples: `" "` or `' '`


## Object
- A collection of key-value pairs.
- Structure: `{<key>: <value>, <key>: <value>,...}`
- ### Array
  - Structure: `[<any number of data>, <any type of data>]`
- ### Null
  - Represents the absence of any object value.

## Boolean
- Represents true or false values.

## Undefined
- Indicates a variable has been declared but not assigned a value.

## Symbol
- An immutable primitive value that is unique.

## BigInt
- A numeric data type that represents integers with arbitrary precision.

### Accessing Values from an Array
To access values from an array, use an index. The index starts from zero(0) and goes to length-1.

Example:
```javascript
const dataArray = ['apple', 'banana', 'cherry'];
const firstElement = dataArray[0]; // 'apple'
const secondElement = dataArray[1]; // 'banana'
```

# Coding Procedure

When starting a coding project, it's essential to follow a systematic procedure for better clarity and efficiency.

1. **Check User Input:**
   - Print user input to the console.
   - Ensure you understand the input provided by the user.

2. **Format Input:**
   - Regardless of the input format, transform it into a consistent format.
   - Make sure the input aligns with the requirements of your program.

3. **Implement Logic:**
   - Develop the main logic to achieve the desired outcome.
   - Break down the problem into smaller, manageable steps.
   - Ensure the logic aligns with the overall goal of the program.

By adhering to this procedure, you create a structured approach to coding, making it easier to understand, maintain, and debug your code.

# Typecasting in JavaScript

Typecasting involves converting data from one type to another, and it's a common operation in programming.

## String to Number

In JavaScript, when converting a string to a number, we have several methods to choose from:

1. **Using `parseInt`:**
    ```javascript
   var num = parseInt("1234");
   ```
2. **Using `parseFloat`:**
    ```javascript
    var num = parseFloat("1234.5");
    ```
3. **Using `Number`:**
   ```javascript
   var num = Number("1234.5");
   ```

4. **Using `+` Operator:**
   ```javascript
   var num = +"1234";
   ```

Choose the method that best suits your requirements. Each method has its own use case, so consider the specific needs of your code when performing typecasting.

```javascript
let num = Number("12js4.5"); // NaN
let num = parseInt("12js4.5"); // 12
```

## Array of Strings to Array of Numbers
### `.map(Number)`

   ```javascript
   var arr = ["10", "20", "30"];
   var numArr = arr.map(Number)
   console.log(numArr); // [10, 20, 30]
   ```
   Explanation:
   1. The `map` function is used to iterate over each element of the array.
   2.  The `Number` function is applied to each element during the mapping process, converting strings to numbers.
   1. The resulting array, `numberArray`, contains the converted numbers.
   2. Now you have successfully converted an array of strings to an array of numbers.

   ```
   +--------------------+                +-------------------+
   |   Array of         |                |   Array of        |
   |   Strings          |  .map(Number)  |   Numbers         |
   | ["10", "20", "30"] |  ------------> | [10, 20, 30]      |
   |                    |                |                   |
   +--------------------+                +-------------------+
   ```

## Number To String

1. **Using `toString`:**
   ```javascript
   var num = 1234;
   var str = num.toString();
   console.log(str); // "1234"
   ```
2. **Using `String`:**
   ```javascript
   var num = 1234;
   var str = String(num);
   console.log(str); // "1234"
   ```
3. **Using `+` Operator:**
   ```javascript
   var num = 1234;
   var str = ""+num;
   console.log(str); // "1234"
   ```

# JavaScript Operators
## Arithmetic Operators
Arithmatic operators are used to perform mathematical operations on numbers.
+ **Addition (`+`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var sum = num + num2;
  console.log(sum); // 30
  ```
  **Note:** :memo: The addition operator can also be used to concatenate strings.
+ **Subtraction (`-`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var diff = num - num2;
  console.log(diff); // -10
  ```
+ **Multiplication (`*`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var prod = num * num2;
  console.log(prod); // 200
  ```
+ **Division (`/`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var quot = num / num2;
  console.log(quot); // 0.5
  ```
+ **Modulus (`%`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var mod = num % num2;
  console.log(mod); // 10
  ```

## Relational Operators
+ **Less Than (`<`):**
+ **Greater Than (`>`):**
+ **Less Than or Equal To (`<=`):**
+ **Greater Than or Equal To (`>=`):**
+ **Equal To (`==`):**
+ **Not Equal To (`!=`):**
+ **Strict Equal To (`===`):**
+ **Strict Not Equal To (`!==`):**

## Logical Operators
+ **Logical AND (`&&`):**
+ **Logical OR (`||`):**
+ **Logical NOT (`!`):**

## Assignment Operators
+ **Assignment (`=`):**
+ **Addition Assignment (`+=`):**
+ **Subtraction Assignment (`-=`):**
+ **Multiplication Assignment (`*=`):**

## Conditional Operator
+ **Ternary Operator (`? :`):**
