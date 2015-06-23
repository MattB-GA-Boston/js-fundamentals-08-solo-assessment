![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Assessment for JavaScript Fundamentals

You have 20 minutes

## Instructions

Fork, clone, and npm install.

Follow the prompts below and complete each question.  You may use any resource, other than someone else in the classroom, to help you complete this assessment.

You should save your answers in this README.md file.

# Question 1

```js
var a = 2;
var b = 3;
a = b;
```

After this code executes, what are the values of a and b? Please explain your answer.

`a` and `b` are both 3, because `b` was equal to 3, and then `a` was set to the value of `b`.

## Question 2

```js
var c = 5;
var d = 2;
c = c + d;
```

After this code executes, what is the value of c?  Please explain what the last line of this program `c = c + d;` means.

The final value of `c` is 7. The last line takes the old value of `c`, adds `d`'s value to it, and sets that as the new value of `c`.

## Question 3

```js
var x = 4;
var y = 3;
x = y;
y = 10;
```

After this code executes, what are the values of x and y?  Please explain your answer.

`x` is 3 and `y` is 10. This is because we set `x` to 3 in the third line, and we set `y` to 10 in the fourth line. There is no permanent relationship between `x` and `y`, so changing `y`'s value doesn't change `x`' s value.

## Question 4

```js
var weather;
weather = "sunny";
weather === "sunny";
```

What are the values of these expressions?  Explain your answers.

`var weather` evaluates to `undefined`, because it doesn't define a value for `weather`.
`weather = "sunny";` evaluates to "sunny". This is because the assignment operator, `=`, evaluates to the value on its right side.
`weather === "sunny";` evaluates to `true`. This is because the equality operator, `===`, evaluates to either true or false, and because at the moment, `weather` is equal to "sunny".


## Question 5

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi >= 3) {
  console.log("sushi is delicious");
}

if (x > 0) {
  console.log("sushi is tasty");
}
```

Imagine that you take the code from this question, save it to a file called `food.js`, and run `node food.js` in your Terminal.

What would be the output? Explain your answer.

The output would be an error, because `x` (referenced in line 7) isn't defined anywhere.

## Question 6

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi > 0) {
  console.log("sushi is tasty");
} else if (x >= 3) {
  console.log("sushi is delicious");
} else {
  console.log("I don't like sushi");
}
```

Imagine that you take the code from this question, save it to a file called `sushi.js`, and run `node sushi.js` in your Terminal.

What would be the output? Explain your answer.

The output would be "sushi is tasty", because although `x` in line 5 is not defined, the first condition in our `if...else` is true, so line 5 (with the undefined `x`) will never be evaluated.

## Question 7

```js
//We'll learn about require later in the course
var ask = require('./ask.js');

var answer = 'not empty';

while (answer !== '' && answer !== 'SeCrEt') {
  answer = ask("Guess my secret? ");
}
```

Imagine that you take the code from this question, save it to a file called `name.js`, and run `node name.js` in your Terminal.

What would you have to type to exit the while loop?  Explain your answer.

We either have to type nothing (followed by 'Enter', of course) or type SeCrEt. The while loop is checking our answer each time, and seeing if it is either of those two values; if it isn't, it runs the loop again.

---

Commit and push your changes.

Submit a pull request.
