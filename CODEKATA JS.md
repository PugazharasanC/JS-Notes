# CODEKATA JS

## Elevate Your Coding Skills with CodeKata

Embark on a journey of coding excellence with CodeKata, a curated series of challenges designed by industry veterans from companies like Microsoft, Walmart, Samsung, and more.

Practice on CodeKata to enhance your coding proficiency, level up your skills, and boost your chances of acing coding interviews.

## Diverse Challenges Await

Explore a range of coding challenges across categories like Absolute Beginner, Mathematics, Arrays, Strings, and more. CodeKata caters to all skill levels, making it ideal for both novice and experienced coders.

## Master JavaScript Problem Solving

Building on the basics covered in [our introductory guide](README.md), dive into real-world problem-solving with JavaScript on CodeKata. Hone your skills, tackle challenges across domains, and elevate your coding prowess through practical exercises.

Now, let's dive into problem-solving on CodeKata. To get started, visit [CodeKata on GUVI](https://www.guvi.in/code-kata) and explore a curated series of challenges across different categories. Whether you're an absolute beginner or an experienced coder, CodeKata provides a range of tiles to suit every skill level and interest.


# User Input in JavaScript

JavaScript is a language that is not inherently designed for obtaining basic user input. However, with the help of Node.js packages, we can facilitate the process of receiving user input.

## Default Input Code

To gather user input in JavaScript, you can use the following default code:

```javascript
// Getting input via STDIN
const readline = require("readline");

const inp = readline.createInterface({
  input: process.stdin
});

const userInput = [];

inp.on("line", (data) => {
  userInput.push(data);
});

inp.on("close", () => {
  // start-here
  // Your code goes here … replace the below line with your code logic

  console.log(userInput);

  // end-here
});
```

Replace the `console.log(userInput);` line with your actual code logic for processing the user input.

## Explanation

 :beginner: **Note for Beginners:**
   Understanding the intricacies of this basic snippet may not be crucial at the start. Instead, focus on utilizing the data in the `userInput` array to solve problems in your CodeKata challenges. As you progress, you'll become more familiar with handling user input and can delve deeper into the code details.

1. `const readline = require("readline");`
   - Import the `readline` module, a utility for reading data from a readable stream, using the `require` function.

2. `const inp = readline.createInterface({
      input: process.stdin
   });`
   - Create an interface (`inp`) for reading input. Specify that the input should come from the standard input (`stdin`) stream.

3. `const userInput = [];`
   - Initialize an empty array called `userInput` to store the user's input.

4. `inp.on("line", (data) => {
      userInput.push(data);
   });`
   - Set up an event listener on the `line` event of the `inp` interface. When a line of input is received, the provided callback function is executed, pushing the input data into the `userInput` array.

5. `inp.on("close", () => {
      console.log(userInput);
    });`
   - Set up another event listener on the `close` event of the `inp` interface. When the input stream is closed (no more data to read), the provided callback function is executed. This is where you can place your code logic. In the example, it prints the collected `userInput` array to the console.

# Let's Solve a Problem

## Odd or Even Checker

### Problem Description
You are tasked with creating a program that determines whether a given number is odd or even.
> This section provides an explanation of the problem you are required to solve. It outlines the task or challenge you need to address through your program.
### Input Format
There will be ony line of input, which contains a single integer.
> This section provides the format of the input data you are required to process. It also explains the data type of the input data.
### Output Format
Print "Even" if the number is even, and "Odd" if the number is odd.
> This section provides the format of the output data you are required to generate. It also explains the data type of the output data.
### Sample Input
```
4
```

### Sample Output
```
Even
```
## Let's understand the problem a bit better.

### What is an integer?
An integer is a number that can be represented as a whole number. In other words, it is a number without any fractional part. For example, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10

### What is an odd number?
An odd number is a number that is not divisible by 2. For example, 1, 3, 5, 7, 9, 11, 13, 15

### What is an even number?
An even number is a number that is divisible by 2. For example, 2, 4, 6, 8, 10

### How do we determine if a number is odd or even?
We can use the modulo operator (`%`) to determine if a number is odd or even. If the remainder of the number after division by 2 is 0, it is even. Otherwise, it is odd.

### How do we check if a number is odd or even?

```javascript
// Assuming the first element in userInput is the number to check
const numberToCheck = parseInt(userInput[0]);

// Check if the number is odd or even
if (numberToCheck % 2 === 0) {
    console.log("Even");
}
else {
    console.log("Odd");
}
```

## Final Solution
```javascript
// Getting input via STDIN
const readline = require("readline");

const inp = readline.createInterface({
  input: process.stdin
});

const userInput = [];

inp.on("line", (data) => {
  userInput.push(data);
});

inp.on("close", () => {
  // start-here
  // Your code goes here … replace the below line with your code logic

  // Assuming the first element in userInput is the number to check
  const numberToCheck = parseInt(userInput[0]);

  // Check if the number is odd or even
  if (numberToCheck % 2 === 0) {
    console.log("Even");
  } else {
    console.log("Odd");
  }

  // end-here
});
```

## Explanation

1. `const numberToCheck = parseInt(userInput[0]);`
   - This line assumes that the first element in the `userInput` array contains the number you want to check (as per the problem statement). It uses `parseInt()` to convert the string representation of the number into an actual integer. This step is necessary because user input is initially collected as strings, and we want to perform numerical operations.

2. `if (numberToCheck % 2 === 0) {`
   - This line checks if `numberToCheck` is divisible evenly by 2. The `%` operator gives the remainder after division. So, `numberToCheck % 2 === 0` checks if the remainder is 0, indicating that the number is even.

3. `console.log("Even");`
   - If the condition in the previous line is true (i.e., the number is even), this line prints "Even" to the console.

4. `} else {`
   - If the condition in the `if` statement is false (i.e., the number is not even), the code inside the `else` block will be executed.

5. `console.log("Odd");`
   - This line prints "Odd" to the console, indicating that the number is not even.

So, in summary, the code takes user input, extracts the number to check, determines if it's even or odd using the modulo operator, and prints the result to the console. It's a simple and effective way to solve the Odd or Even Checker problem.

## What's Next?

Let's solve more problems.
### Problem-Solving Checklist

- [x] **Print the `userInput` array:**
   - This step helps in understanding the input format and allows us to visualize the data we're working with.

- [x] **Spread values into variables:**
   - Assign meaningful variable names to different elements in the `userInput` array. For example, `numberToCheck` and `numberToPrint` are good choices.

- [x] **Convert input values to the desired data type:**
   - Since the input values are initially collected as strings, use appropriate conversion functions (`parseInt`, `parseFloat`, etc.) to convert them to the desired data type.

- [x] **Proceed to solve the problem:**
   - Apply the necessary logic to solve the specific problem using the variables created. Break down the problem into smaller steps if needed.

Now that you've learned how to solve a problem, let's move on to the next problem in the series.

## Beginner-Friendly Problem Categories

Welcome, coding enthusiast! 🚀 If you're just starting your coding journey, consider following these problem categories to enhance your skills and build a solid foundation:

- Input/Output
- Absolute Beginner
- Basics
- Maths
- Array
- String
- Looping
- Patterns

---

*Thank you for taking the time to read my article. Your engagement is the driving force behind the words on these pages. Whether you found information, inspiration, or simply enjoyed the content, your presence is deeply appreciated. Writing is a shared journey, and I'm grateful to have you as a reader. Cheers to the joy of exploration and discovery! 🌟*

*If you enjoyed the article, consider giving it more stars!*

*With gratitude,*

*Pugazharasan C*
