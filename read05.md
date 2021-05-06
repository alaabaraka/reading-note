Loops

a way to repeat code for an amount of time without copying and pasting the same code .

for loop when you want repeat the code for limited amount of times until is false

for (initialization; condition; update) {

is the code that will keep running as long as the condition is true .

Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript.

You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop

for...of statement


The for...of statement creates a loop Iterating over iterable objects
(including Array, Map, Set, arguments object and so on), invoking a custom iteration
hook with statements to be executed for the value of each distinct property.
for (variable of object)
  statement
  
  The following example shows the difference between a for...of loop and
  a for...in loop. While for...in iterates over property names, for...of iterates over property values:
  
  const arr = [3, 5, 7];
arr.foo = 'hello';

for (let i in arr) {
   console.log(i); // logs "0", "1", "2", "foo"
}

for (let i of arr) {
   console.log(i); // logs 3, 5, 7
}








