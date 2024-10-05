## goit-neo-js-hw-04



## Task 1. Packing goods

Do this task in the filetask-1.js

Write a function isEnoughCapacity(products, containerSize) that calculates whether all goods will fit into the container during packing.


The function declares two parameters:

products — an object where keys are product names, and their values are the quantity of those products. For example, { apples: 2, grapes: 4 }.
containerSize — a number, the maximum quantity of units of goods that the container can hold.

The function should return the result of the check whether all goods fit into the container. Calculate the total quantity of goods in the products object and return true if it is less than or equal to containerSize, and false otherwise.


Take the code below and paste it after declaring your function to verify its correctness. The results of its calls will be printed in the console.


console.log(
  isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)
); // true

console.log(
  isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)
); // false

console.log(
  isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)
); // true

console.log(
  isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)
); // false


## Task 2. Calorie calculation

Do this task in the file task-2.js

Write a function calcAverageCalories(days) that returns the average daily value of calories an athlete consumes over a week. The function expects one parameter: days — an array of objects. Each object describes a day of the week and the number of calories the athlete consumes. Take the code below and insert it after declaring your function to verify its correctness. The results of its calls will be printed on the console.


console.log(
  calcAverageCalories([
    { day: "monday", calories: 3010 },
    { day: "tuesday", calories: 3200 },
    { day: "wednesday", calories: 3120 },
    { day: "thursday", calories: 2900 },
    { day: "friday", calories: 3450 },
    { day: "saturday", calories: 3280 },
    { day: "sunday", calories: 3300 }
  ])
); // 3180

console.log(
  calcAverageCalories([
    { day: "monday", calories: 2040 },
    { day: "tuesday", calories: 2270 },
    { day: "wednesday", calories: 2420 },
    { day: "thursday", calories: 1900 },
    { day: "friday", calories: 2370 },
    { day: "saturday", calories: 2280 },
    { day: "sunday", calories: 2610 }
  ])
); // 2270

console.log(
  calcAverageCalories([])
); // 0



## Task 3. Player profile

Do this task in the file task-3.js


The object profile describes a user profile on a gaming platform. Its properties store the profile name, username, and the number of active hours playTime spent in the game.


const profile = {
    username: "Jacob",
  playTime: 300,
};


Extend the profile object with methods to work with its properties.

The method changeUsername(newName) should take a string (new name) as parameter newName and change the value of the username property to the new name. It doesn't return anything.
The method updatePlayTime(hours) should take a number (hours count) as parameter hours and increase the playTime property by that amount. It doesn't return anything.
The method getInfo() should return a string in the format <Username> has <amount> active hours!, where <Username> is the profile name and <amount> is the number of gaming hours.

Take the code below and insert it after declaring your function to verify its correctness. The results of its operation will be printed on the console.


console.log(profile.getInfo()); // "Jacob has 300 active hours!"

profile.changeUsername("Marco");
console.log(profile.getInfo()); // "Marco has 300 active hours!"

profile.updatePlayTime(20);
console.log(profile.getInfo()); // "Marco has 320 active hours!"


## Requirements
- Code must be formatted with Prettier.
- There must be no errors or warnings in the console after running the tasks.
- Execution of tasks 1, 2 and 3.

## Formatting the code with Prettier:

* You must have Node.js installed, then install Prettier in your project. This can be done with the command in the terminal:

```bash
npm install --save-dev prettier
```

* Then you can run Prettier on your code with:

```bash
npx prettier --write .
```

This command will format all files in the project.