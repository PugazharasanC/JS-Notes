## [JS CheatSheet](https://drive.google.com/file/d/14mSzInQ674Drdu_iKULASF1XsCDKjJcm/view?usp=sharing)


// ! varibale => Value box => can be updated any time => can access the value anytime
// ! How to declare a variable => <keyword> <variable_name> = <value>;
Example:
```
var num = 10;
```
// ! KeyWord => Compiler known word => it is already defined in programming language itself
// ? Example => var
// ! DataType => It means the type of data which we are going to store
// ? Number => 1,2,3,-1,-5,-100, 10.5, 25.65
// ? String => "", ''
// ?  Array => [<any number of data> , <any type of data>]
// ! How to access the values from the array?
// ? WE have to use index => index starts from zero(0) and goes till length-1
// ? first element index is 0, second element index is 1

// ? Procedure to follow while starting coding.
// TODO whenever we are starting a program, we have to check the userInput by printing it in console.
// TODO Whatever the input format, we have to change it to our own format.
// TODO now we have to implement our logic to get the answer
// ! Typecasting => converting data from one type to another type
// ! String to Number => We have to use one of the following
// * parseInt => var num = parseInt("1234")
// * parseFloat => var num = parseFloat("1234.5")
// * Number => var num = Number("1234" or "1234.5")
// * + => var num = +"1234" or +"1234.5"
// ! converting array of strings to array of numbers
// * .map(Number) => var numArr = arr.map(Number)
// ! Code Blocks {}
// * {} is used to specify block of code or grouping code

// ! Operator
// * Arithmatic Operator => +,-,*,/,%
// * Relational Operator => < , > , <= , >= ,== ,!=, ===, !==
// * Logical Operator => && , || , !
// * Assignment Operator => =, +=,-=,*=
// * Conditional Operator => ?:

// ! Looping Statements
// * For loop
// * while loop
// * do...while loop

// TODO Num => Super Pugazh Number => 1563548 => 001+563+548 => if sum is even => Super pugazh, otherwise it is not a super pugazh number

// TODO num1, num2 => check how many numbers can divided by 3, 5 and both 3 and 5

// !    *
// !    * *
// !    * * *
// !    * * * *
// !    * * * * *
//  1  2  3  4 5
// 16 17 18 19 6
// 15 24 25 20 7
// 14 23 22 21 8
// 13 12 11 10 9

// Prime Or Not
// Swapping

// let a = 10;
// let b = 15;
// console.log(a, b);
// a = a + b;
// b = a - b;
// a = a - b;
// console.log(a, b);
// a = 15
// b = 10
// Sorting

// let arr = [54, 53, 542, 5, 245, 436, 3];

// let sortedArr = [3, 5, 53, 54, 245, 436, 542];
// let descSortedArr = [542, 436, 245, 54, 53, 5, 3];

// bubble sort
// [54, 53, 542, 5, 245, 436, 3];
// [53, 54, 542, 5, 245, 436, 3];
// [53, 54, 542, 5, 245, 436, 3];
// [53, 54, 5, 245, 436, 3, 542];
// console.log(...arr);
// for (let j = 0; j < arr.length; j++)
//   for (let i = 0; i < arr.length - 1; i++) {
//     if (arr[i] < arr[i + 1]) {
//       // swap
//       let temp = arr[i];
//       arr[i] = arr[i + 1];
//       arr[i + 1] = temp;
//     }
//   }
// console.log(...arr);

// selection sort
// [3, 54, 542, 53, 245, 436, 5];

// console.log(...arr);
// for (let ind = 0; ind < arr.length; ind++)
//   for (let i = ind; i < arr.length; i++) {
//     if (arr[i] < arr[ind]) {
//       let temp = arr[i];
//       arr[i] = arr[ind];
//       arr[ind] = temp;
//     }
//   }

// console.log(...arr); //Spread Operator

// ? command to run
// ! type <inputfile name> | node <js code>

// spread & rest operators => ...

// 10 + 15 => 25
// "Pugazh"  + "arasan" => "Pugazharasan"

const dummyFunction = ({ name, place, EXP, salary }) => {
  //   console.log(obj);
  console.log(name, place, EXP, salary);
};

let obj = {
  name: "Pugazh",
  place: "Chennai",
  company: "GUVI",
  stack: "MERN",
  height: "Podhumana Alavu",
  EXP: "5+",
};
// dummyFunction(obj);

let { name, place, EXP, salary } = obj;
console.log(name, place, EXP, salary);