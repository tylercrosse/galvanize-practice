## Part-1

1. Create a function named 'mulitply', that accepts two arguments, and returns the value of the two arguments mulitplied together.

2. Test if your function works by calling the function with some arguments and seeing if it spits out what you expected

```js
multiply(3, 4) // will return 12
```

3. Save your (hopefully working) code in a text editor (ex. Atom or Sublime)

## Part-2

What is alerted in each case? Write down your answer before running the code.

1.
```js
function foo(){
  function bar() {
      return 3;
  }
  return bar();
  function bar() {
      return 8;
  }
}
alert(foo());
```
2.
```js
function foo(){
  var bar = function() {
      return 3;
  };
  return bar();
  var bar = function() {
      return 8;
  };
}
alert(foo());
```

3.
```js
function foo(){
  return bar();
  var bar = function() {
      return 3;
  };
  var bar = function() {
      return 8;
  };
}
alert(foo());
```
