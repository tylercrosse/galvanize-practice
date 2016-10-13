# JS Functions

## LO's (5)
1. Describe what a JavaScript function is and why functions are used.
- Recognize the parts of a function.
- Differentiate between referencing and invoking a function, with a use case.
- State the difference between a function's output and side effects.
- Be able to write a function in JavaScript using a declaration and an expression.

### Framing

This lessons assumes students are familiar with:
- JS variables
- JS data types
- JS conditionals
- How to run javascript, either through the browser console or in node

## 1. Function basics (7)

Code is a set of instructions:

> Get the Materials. ...
> Prepare the Bread. ...
> Apply Peanut Butter. ...
> Apply Jelly. ...
> Combine Both Slices of Bread. ...
> Eat and Repeat.

**Q. In what order are these instructions/statements executed?**

---

If I wanted to write some code to add two numbers, the simplest thing I could do is:

```js
10 + 7
```

Now, imagine that I was working on a much longer program I needed to be able to access the result of a portion of the code later. I could store some information about what operation I was performing in `variables` 

```js
let a = 10
let b = 7
let ans = a + b
ans // will 'return' the value of whatever is stored in this variable

// ....potentially a bunch of other stuff

let newAns = ans + a
newAns // again & always, will 'return' the value of whatever is stored in this variable
```

This code is more reusable than the first example where we simple added two fixed numbers

Now if I want my script to also add two other numbers.

```js
let a = 8
let b = 6
let ans1 = a + b
let c = 7
let d = 10
let ans2 = c + d
```

**Q. How do I access the values stored in the variables? Are their any problems with this code? Could this be improved at all? (3)**

```js
function add(param1, param2) {
  return param1 + param2;
};
let ans1 = add(8, 6);
let ans2 = add(7, 10);
```

#### Think / Pair / Share (1/3/4)

<details>
<summary>**Q. What’s a function?**</summary>

- Fundamental component of Javascript.
- A reusable block of Javascript code.
- Simply put, a function is a block of code that takes an input, processes that input and then produces an output.
- Analogy: Quizno's Oven

</details>


<details>
<summary>**Q. Why do we use functions?**</summary>
Benefits of functions:
- Reusability.
- DRYness.
- Naming convention (describes intent).

</details>

---
## 2. Parts of a function (5)

```js
function someName(parameter1, parameter2) {
  // the 'body' of the function, i.e. what code is run when the function is called
}
```

<details>
<summary>**Q. What are the parts of a function?**</summary>

- `function` Keyword
- Name of the function
- Parameters or arguments - the 'input'
- Body or statements of the function
- `return` value - the 'output'

</details>

#### In a new tab, complete [Part 1](./exercises.md/#[part-1) of the exercise (5)
---
## 3. Referencing vs. Invoking (5)

```js
multiply(2, 5)

// vs.

multiply
```

<details>
<summary>**Q. Which is which? What's the difference?** </summary>

`Invoking` or calling or executing or running a function asks Javascript to do whatever code is inside the body of the function using whatever (if any) parameters are passed into it.

`Referencing` a function will 'return' whatever the function is without running the function. This is most used when responding to events.

</details>

---
## 4. Output & Side Effects (5)

The **output** of a function is whatever the function returns.
- All functions 'implicitly' return `undefined` unless 'explicitly' told to return something different.
- The `return` statement ends the execution of a function, and any statements after it will not be run.

The **side effects** of a function are anything the function does other than return.
- Sometimes more important than the return.

---
## 5. Declarations, Expressions, & Arrows (5)

There are two* main ways of defining a function in javascript.

**Function declarations** 
```js
function funcDeclaration() {
  return "I'm a function declaration!"
}
```

- 'hoisted' to the top of the script

**Function expressions**
```js
let funcExpression = function() {
  return "I'm a function expression!"
}

// or 

let arrowFuncExpression = () => (
  "I'm a function expression using cool new syntax!"
)
```

- can be anonymous

#### Complete [Part 2](./exercises.md/#part-2) of the exercise (5)
