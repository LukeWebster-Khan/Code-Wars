# Total Completed: 13

## Convert a Number to a String!

https://www.codewars.com/kata/5265326f5fda8eb1160004c8/solutions/javascript/me/best_practice

We need a function that can transform a number into a string.

What ways of achieving this do you know?

```javascript
function numberToString(num) {
  return String(num);
}
```

## Convert boolean values to strings 'Yes' or 'No'.

https://www.codewars.com/kata/53369039d7ab3ac506000467

Complete the method that takes a boolean value and return a "Yes" string for true, or a "No" string for false.

```javascript
function boolToWord(bool) {
  //...
  if (bool == true) {
    return "Yes";
  } else {
    return "No";
  }
}
```

## Is it a Palindrome?

https://www.codewars.com/kata/57a1fd2ce298a731b20006a4

Write a function that checks if a given string (case insensitive) is a palindrom

```javascript
function isPalindrome(x) {
  let polishedString = x.replace(/\W+|_/g, "").toLowerCase();
  let reversedString = polishedString.split("").reverse().join("");

  if (polishedString != reversedString) return false;
  else {
    return true;
  }
}
```

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

## Remove First and Last Character

https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0

It's pretty straightforward. Your goal is to create a function that removes the first and last characters of a string. You're given one parameter, the original string. You don't have to worry with strings with less than two characters.

```javascript
function removeChar(str) {
  return str.slice(1, -1);
}
```

## Opposite Number

https://www.codewars.com/kata/56dec885c54a926dcd001095

Very simple, given a number, find its opposite.

```javascript
function opposite(number) {
  return -number;
}
```

## Sum of Positive

https://www.codewars.com/kata/5715eaedb436cf5606000381

You get an array of numbers, return the sum of all of the positives ones.

Example [1,-4,7,12] => 1 + 7 + 12 = 20

Note: if there is nothing to sum, the sum is default to 0.

```javascript
function positiveSum(arr) {
  var removeNeg = arr.filter(function (val) {
    return val >= 0;
  });
  return removeNeg.reduce((a, b) => a + b, 0);
}
```

## Remove String Spaces

https://www.codewars.com/kata/57eae20f5500ad98e50002c5

Simple, remove the spaces from the string, then return the resultant string.

```javascript
function noSpace(x) {
  return (x = x.replace(/\s+/g, ""));
  console.log(x);
}
```

## Even or Odd

https://www.codewars.com/kata/53da3dbb4a5168369a0000fe

Create a function (or write a script in Shell) that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.

```javascript
function even_or_odd(number) {
  if (number % 2) {
    return "Odd";
  } else {
    return "Even";
  }
}
```

## Multiply

https://www.codewars.com/kata/50654ddff44f800200000004

This code does not execute properly. Try to figure out why.

```javascript
function multiply(a, b) {
  return a * b;
}
```
