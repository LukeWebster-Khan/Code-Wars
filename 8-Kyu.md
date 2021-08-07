# Total Completed: 3

## String Repeat

https://www.codewars.com/kata/57a0e5c372292dd76d000d7e

Write a function called repeatStr which repeats the given string string exactly n times.

repeatStr(6, "I") // "IIIIII"
repeatStr(5, "Hello") // "HelloHelloHelloHelloHello"

```javascript
function repeatStr(n, s) {
  return s.repeat(n);
}
```

## My head is at the wrong end!

https://www.codewars.com/kata/56f699cd9400f5b7d8000b55

You're at the zoo... all the meerkats look weird. Something has gone terribly wrong - someone has gone and switched their heads and tails around!

Save the animals by switching them back. You will be given an array which will have three values (tail, body, head). It is your job to re-arrange the array so that the animal is the right way round (head, body, tail).

Same goes for all the other arrays/lists that you will get in the tests: you have to change the element positions with the same exact logics

Simples!

```javascript
function fixTheMeerkat(arr) {
  return arr.reverse();
}

/* Second Solution*/

function fixTheMeerkat(arr) {
  let end = arr.shift();
  let start = arr.pop();

  arr.push(end);
  arr.unshift(start);

  return arr;
}
```

## Reversed Strings

https://www.codewars.com/kata/5168bb5dfe9a00b126000018

Complete the solution so that it reverses the string passed into it.

```javascript
function solution(str) {
  return str.split("").reverse().join("");
}
```

## Return Negative

https://www.codewars.com/kata/55685cd7ad70877c23000102

In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

```javascript
function makeNegative(num) {
  if (num > 0) {
    return num * -1;
  } else {
    return num;
  }
}
```
