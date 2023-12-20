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
  :memo: **Note:** The addition operator can also be used to concatenate strings.

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
  :memo: **Note:** The division operator returns the quotient of the division of the first number by the second number.
+ **Modulus (`%`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var mod = num % num2;
  console.log(mod); // 10
  ```
  :memo: **Note:** The modulus operator returns the remainder of the division of the first number by the second number.

## Relational Operators
Relational operators are used to compare two values. The result of the comparison is either `true` or `false`.
+ **Less Than (`<`):**
  ```javascript
  console.log(10 < 20) // true
  console.log(10 < 10) // false
  console.log(10 < 0) // false
  ```
+ **Greater Than (`>`):**
  ```javascript
  console.log(10 > 20) // false
  console.log(10 > 10) // false
  console.log(10 > 0) // true
  ```
+ **Less Than or Equal To (`<=`):**
  ```javascript
  console.log(10 <= 20) // true
  console.log(10 <= 10) // true
  console.log(10 <= 0) // false
  ```
+ **Greater Than or Equal To (`>=`):**
  ```javascript
  console.log(10 >= 20) // false
  console.log(10 >= 10) // true
  console.log(10 >= 0) // true
  ```
+ **Equal To (`==`):**
  ```javascript
  console.log(10 == 20) // false
  console.log(10 == 10) // true
  console.log(10 == 0) // false
  ```
  :memo: **Note:** The equality operator only check the values not the type. Comparing different type with same valye is considered equal.
  Example:
  ```javascript
  console.log(10 == "10") // true
  ```
+ **Not Equal To (`!=`):**
  ```javascript
  console.log(10 != 20) // true
  console.log(10 != 10) // false
  console.log(10 != 0) // true
  ```
+ **Strict Equal To (`===`):**
  ```javascript
  console.log(10 === 20) // false
  console.log(10 === 10) // true
  console.log(10 === 0) // false
  ```
  :memo: **Note:** The strict equality operator checks the type and value of the operands. Comparing different type with same value is considered not equal.
  Example:
  ```javascript
  console.log(10 === "10") // false
  ```
+ **Strict Not Equal To (`!==`):**
  ```javascript
  console.log(10 !== 20) // true
  console.log(10 !== 10) // false
  console.log(10 !== 0) // true
  console.log(10 !== "10") // true
  ```

## Logical Operators
Logical operators are used to combine the results of two or more expressions which are either `true` or `false`.
+ **Logical AND (`&&`):**
  ```javascript
  console.log(true && false) // false
  ```
  :memo: **Note:** The logical AND operator returns the first expression which evaluates to `false`. If all the expressions evaluate to `true`, the logical AND operator returns the last expression.
+ **Logical OR (`||`):**
  ```javascript
  console.log(true || false) // true
  ```
  :memo: **Note:** The logical OR operator returns the first expression which evaluates to `true`. If all the expressions evaluate to `false`, the logical OR operator returns the last expression.
+ **Logical NOT (`!`):**
  ```javascript
  console.log(!true) // false
  ```
  :memo: **Note:** The logical NOT operator is used to negate the result of the expression.

The below table gives the truth table for the logical operators. using this table you can easily understand the logical operators.

| Expression 1  | Expression 2 | AND   |  OR  |  NOT  |
|:--------------:|:--------------:|:------------:|:-----------:|:------------:|
|`expr1`|`expr2`|`expr1 && expr2`|`expr1 \|\| expr2`|`!expr1`|
| true         | true         | true       | true      | false      |
| true         | false        | false      | true      | false      |
| false        | true         | false      | true      | true       |
| false        | false        | false      | false     | true       |



## Assignment Operators
Assignment operators are used to assign values to variables.
+ **Assignment (`=`):**
  ```javascript
  var num = 10;
  ```
+ **Addition Assignment (`+=`):**
  ```javascript
  var num = 10;
  num += 20; // num = num + 20;
  console.log(num); // 30
  ```
  :memo: **Note:** The addition assignment operator is used to add the value of the right operand to the left operand and assign the result to the left operand.
+ **Subtraction Assignment (`-=`):**
  ```javascript
  var num = 10;
  num -= 20; // num = num - 20;
  console.log(num); // -10
  ```
+ **Multiplication Assignment (`*=`):**
  ```javascript
  var num = 10;
  num *= 20; // num = num * 20;
  console.log(num); // 200


  ```

## Conditional Operator
Conditional operator is used to execute a statement if a specified condition is true, otherwise another statement.
+ **Ternary Operator (`? :`):**
  ```javascript
  var num = 10;
  var num2 = 20;
  var result = (num > num2)? "num is greater than num2" : "num is less than num2";
  console.log(result); // num is greater than num2
  ```

## Bitwise Operators
Bitwise operators are used to perform bitwise operations on integers.
+ **Bitwise AND (`&`):**
+ **Bitwise OR (`|`):**
+ **Bitwise NOT (`~`):**
+ **Bitwise XOR (`^`):**
+ **Left Shift (`<<`):**
+ **Right Shift (`>>`):**
+ **Zero Fill Right Shift (`>>>`):**
+ **Unsigned Right Shift (`>>>`):**


# Looping Statements
Looping statements are used to execute a block of code repeatedly. There are three types of looping statements in JavaScript:
## **While loop:**
   The while loop is a fundamental control flow statement in JavaScript. It repeatedly executes a block of code as long as a specified condition is true. The condition is checked before executing the block of code.
   ### Syntax
   ```javascript
   while (condition) {
      // code block to be executed
   }
   ```
   ### Example
   ```javascript
   let count = 0;

   while(count < 5) {
      console.log("Count: " + count);
      count++;
   } while (count < 5);

   console.log("Loop Finished");
   ```
   ### Output
   ```vbnet
   Count: 0
   Count: 1
   Count: 2
   Count: 3
   Count: 4
   Loop Finished
   ```
   ### Explanation:
   + The `while` keyword is followed by a condition in parentheses.
   + If the condition is true, the code block inside the curly braces `{}` is executed.
   + After the block execution, the condition is checked again, and if it's still true, the loop continues.
   + This process repeats until the condition becomes `false`.

   :memo: **Note:** The while loop checks the condition before the block execution. If the condition is initially false, the block of code may not run at all.

## **For loop:**
   The for loop is used to execute a block of code a specified number of times. The condition is checked after executing the block of code.

   ### Syntax
   ```javascript
   for (initialization; condition; increment) {
      // code block to be executed
   }
   ```
   ### Example
   ```javascript
   for (var i = 1; i <= 5; i++) {
      console.log(i); // 1, 2, 3, 4, 5
   }
   console.log("Done");
   ```
   ### Output
   ```vbnet
   1
   2
   3
   4
   5
   Done
   ```
   ### Explanation:
   + The `for` keyword is followed by three expressions in parentheses, separated by semicolons.
     + The first expression is executed only once, when the loop starts. This expression is used to initialize the loop variable.
     + The second expression is evaluated before every iteration of the loop. If the expression evaluates to `true`, the loop body is executed. If the expression evaluates to `false`, the loop terminates.
     + The third expression is executed at the end of every iteration of the loop. This expression is used to increment or decrement the loop variable, thereby controlling the loop flow.
   + The loop terminates when the condition becomes `false`.


   :memo: **Note:** The for loop can also be used to iterate over an array.
   ```javascript
   var fruits = ["Banana", "Orange", "Apple", "Mango"];
   for (var i = 0; i < fruits.length; i++) {
      console.log(fruits[i]); // Banana, Orange, Apple, Mango
   }
   console.log("Done");
   ```
## do...while loop
   The do...while loop is used to execute a block of code at least once. The condition is checked before executing the block of code.
   ### Syntax
   ```javascript
   do {
      // code block to be executed
      } while (condition);
   ```
   ### Example
   ```javascript
   let count = 0;
   do {
      console.log("Count: " + count);
      count++;
   } while (count < 5);
   console.log("Loop Finished");
   ```
   ### Output
   ```vbnet
   Count: 0
   Count: 1
   Count: 2
   Count: 3
   Count: 4
   Loop Finished
   ```
   ### Explanation:
   + The `do` keyword is followed by a block of code.
   + The block of code is executed at least once.
   + The `while` keyword is followed by a condition in parentheses.
   + If the condition is true, the code block inside the curly braces `{}` is executed.
   + After the block execution, the condition is checked again, and if it's still true, the loop continues.
   + This process repeats until the condition becomes `false`.
   + The loop terminates when the condition becomes `false`.
   + The do...while loop is similar to the while loop but the condition is checked after executing the block of code.
   + The do...while loop is useful when you want to execute a block of code at least once.
