# Part 2

## Question 1

At line 12, the program would print `3` to the console. The variable `i` is declared using `var`, so it is visible anywhere in the function `discountedPrices`, even outside the for loop. Once the for loop finishes running, `i` is set to `3`, so that gets logged to the console.

## Question 2

At line 13, the program will print `150` to the console. The variable `discountedPrice` was declared using `var` so it is visible throughout the entire function `discountPrices`. Once the for loop finishes running, it will be set to `150` so the console will log `150`.

## Question 3

In line 14, the program will print `150` to the console. `finalPrice` is declared using `var` inside the `discountPrices` function so it is visible all throughout the function. At the end of the for loop, it is set to `150` so `150` will be printed to the console.

## Question 4

This function will return `[50, 100, 150]`. When the function `discountPrices` is called, first the variables `discounted` and `finalPrice` are declared using the `var` keyword (making them visible throughout the entire function `discountPrices`). Next, the for loop runs. For each element of `prices`, it multiplies that price by `1 - discount`, rounds it to two decimal places, and adds it to the array contained in `discounted`. Next, `discounted` is returned by the function.

## Question 5

The code will cause an error at line 12. The variable `i` was declared using `let` in the for loop. Therefore, `i` is only visible in the for loop and does not exist outside the for loop block, where `console.log(i);` is called. 

## Question 6

The code will cause an error at line 13. The variable `discountedPrice` is declared using `let` in the body of the for loop. Therefore, it is only visible within the body of the for loop. Since `console.log(discountedPrice);` on line 13 is being called outside the body of the for loop, it cannot access `discountedPrice` so an error is given.

## Question 7

`150` will be printed to the console. `finalPrice` is declared using `let` inside the `discountPrices` function but outside the for loop. Therefore, it is visible throughout the entire `discountPrices` function. After the for loop finishes running, it is set to `150` so when we reach line 14, `150` is printed to standard output. The `console.log(finalPrice);` function is located inside the body of the `discountedPrices` function, so `finalPrice` is visible to it. 

## Question 8

This function will return `[50, 100, 150]`. The function starts by declaring the variables `discounted` and `finalPrice`. Both these variables are declared using the `let` keyword in the function `discountPrices` so they are visible throughout the entire function. Next, the for loop runs. Each time it runs, it calcualtes `discountedPrice` from the current price in `prices`. `discountPrice` is only visible in the for loop since it was declared using `let` in the for loop. Next, the for loop sets `finalPrice` to the discounted price rounded to two decimal places. It then adds the price in `finalPrice` to `discounted` which is visible both inside and outside the for loop. After the for loop runs, the function returns `discounted` which contains the array shown above.

## Question 9

The code will cause an error at line 11 because `i` is not in scope. `i` is declared using `let` in the for loop, so it is only visible inside the for loop body.

## Question 10

At line 12, the code will print `3` to the console. When the function is called, `length` is declared using the `const` keyword and is set to `prices.length`, which is `3`. `length` is never updated (it can't be updated or it would produce an error) and is simply printed to the console in line 12. Therefore, since no errors would occur, `3` would be printed to the console. 

## Question 11

The function will return `[50, 100, 150]`. The function first declares two variables, `discounted` and `length` both of which are declared using the `const` keyword and both of which cannot be updated. Next, the for loop loops thorugh each element in `discounted` and for each element, it creates a new variable `discountedPrice` which is declared using the `const` keyword, which holds the price from `prices` multiplied by `(1 - 0.5)`. Next, the value in `discountedPrice` is added to the array stored in `discounted` in line 8. This operation does not cause an error because JavaScript arrays are passed by reference and the reference itself which is stored in `discounted` is not changing. Only the array that reference is pointing to changes. After the for loop completes, the reference to the array `[50, 100, 150]` stored in `discounted` is returned.

## Question 12

A. `student.name;`

B. `student['Grad Year'];`

C. `student.greeting();`

D. `student['Favorite Teacher'].name;`

E. `student.courseLoad[0];`

## Question 13

A. `'32'` - The number `2` is converted into the string `'2'` and is then concatenated with the string `'3'`.

B. `1` - The string `'3'` is converted to the number `3`, then `2` is subtracted from it.

C. `3` - `null` is converted to `0` and then the arithmetic is performed.

D. `'3null'` - `null` is converted to the string `'null'`, which is then concatenated to the string 
`'3'`.

E. `4` - The boolean `true` is converted to the number `1` and is then added to `3`.

F. `0` - `false` is converted to the number `0` and `null` is also converted to the number `0`. The two `0`'s are then added together.

G. `'3undefined'` - `undefined` is converted to the string `'undefined'` adn is then concatenated with `'3'`.

H. `NaN` - The string `'3'` is converted to the number `3` and `undefined` is converted to `NaN`. The arithmetic `3 - NaN` is performed, which results in an output of `NaN`.

## Question 14

A. `true` - The string `'2'` is converted to the number `2` and is then compared with the number `1`.

B. `false` - The strings are compared character by character starting at the first character. Since `'2'` comes after `'1'` in unicode, the string `'2'` is greater than the string `'12'` so the comparison evaluates to `false`.

C. `true` - The string `'2'` is converted to the number `2` and the comparison is performed. Since `2` is equal to `2`, the comparison evaluates to `true`.

D. `false` - Beacuse the strict equality operator (`===`) was used, no type conversion is performed before the comparison. Because `2` and `'2'` are of different data types, the comparison evaluates to `false`.

E. `false` - `true` is converted to the number `1` before the comparison is performed. Since `1` is not equal to `2`, the comparison returns `false`.

F. `true` - The `Boolean()` function converts the number `2` to the boolean `true`. The boolean `true` is then compared with the boolean `true` using the strict equality operator (`===`). Because both values being compared are of the same data type and are the same value, the expression evaluates to `true`.

## Question 15

The `===` operator evaluate to `false` if the objects on either side of it are not of the same data type. If the objects are of the same data type, it compares them as normal. By contrast, if the `==` operator has objects of different data types on either side of it, it converts the objects to numbers and then compares the numbers.

## Questoin 16

see `part2-question16.js`

## Question 17

The function `modifyArray([1,2,3], doSomething);` will return `[2, 4, 6]`. First, `modifyArray([1,2,3], doSomething);` is called. Inside the `modifyArray` function, `newArr`, an empty array, is created. Next, the for loop iterates through each element of `array` and calls the function `doSomething` which is stored in the variable `callback` on that element of the array. The result of the call to `callback` is added to `newArr`. `doSomething` takes a number and returns the product of that number and 2. Therefore, the result returned by `modifyArray([1,2,3], doSomething);` is the array `[2, 4, 6]`.

## Question 18

see `part2-question18.js`

## Question 19

Output:
```
1
4
3
2
```

