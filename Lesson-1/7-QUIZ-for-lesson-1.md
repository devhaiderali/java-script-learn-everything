# Quiz:


**BE HONEST WITH YOURSELF DON'T TRY TO CHEAT, IF YOU STUCK SOMEWHERE GO TO THE TOPIC AND STUDY AGAIN BUT DONT CHEAT!**
1. True or False: JavaScript is a language that helps make websites interactive.

3. Give one example of something JavaScript can do on a webpage.

5. Fill in the blank: “JavaScript is a _______ language.”

7. What’s the difference between declaration and initialization?

9. Which line only declares a variable named `score`?

  A) `var score = 0;`
  
  B) `let score;`
  
  C) `score = 10;`
  
7. Write code to declare a variable `name` and then initialize it with `"Alex"` on a separate line.
8. If you write `var x = 5;` outside any `{ }` or function, what kind of scope does `x` have?

10. What happens if you try to use a `let` variable outside the `{ }` block where it was declared?

12. True or False: A `var` inside a function can be used outside that function.

14. What does re-assignment mean?

16. Can you re-declare the same `let` variable name in the same spot? (Yes/No)

18. What will this show?
```
var a = 3;
var a = 7;
console.log(a);
```
13. Which keywords have a Temporal Dead Zone: `var`, `let`, `const`?

15. What happens if you do `console.log(age); let age = 8;`?

17. Fill in the blank: “Before you give a `let` or `const` a value, it lives in the _______.”

19. What does “hoisting” move to the top of the code: declarations, initializations, or both?

21. What will this print?
```
console.log(score);
var score = 20;
```
18. What error (if any) happens here?
```
console.log(name);
let name = "Ayesha";
```
19. (Bonus) In your own words, explain why using `var` before its initialization shows `undefined`, but using `let` or `const` gives an error.
---


## Hard Part (only some of you can solve these - MUST TRY)
1. What does the following code print, and why?
```
console.log(x, y);
var x = 'first';
let y = 'second';
{
  var x = 'third';
  let y = 'fourth';
}
console.log(x, y);
```

2. Consider this function. What happens when you call mystery()—does it log a value, or throw an error? Explain the reason.
```
function mystery() {
  console.log(secret);
  const secret = '🕵️‍♂️';
}
mystery();
```

3. Predict the output (or errors) of this snippet. Write down each line’s result in order, and explain how hoisting and scope affect it.
```
var a = 1;
function foo() {
  a = 2;
  console.log(a);
  var a;
  console.log(a);
}
foo();
console.log(a);
```
---
*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck. ♥*
