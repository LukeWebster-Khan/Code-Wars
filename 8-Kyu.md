# Total Completed: 10

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
```
