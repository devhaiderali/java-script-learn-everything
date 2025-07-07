# Hoisting


**🎩 What is Hoisting?**
Hoisting means JavaScript moves variable declarations to the top of the code before running it.
But here’s the fun part:
It only moves the name (declaration), not the value (initialization).

## 📦 Real-Life Example:
Imagine you're packing a school bag:
- You write your name on the bag first (declaration).
- But you put your books in later (initialization).
In JavaScript, it does the same thing — it lifts the variable name up, but not the value.

**✅ Example with var**
```
console.log(a); // 👉 undefined (no error!)

var a = 2;
```
*Behind the scenes, JavaScript treats it like this:*
```
var a;        // 👈 declaration is hoisted
console.log(a); // 👉 undefined
a = 2;        // 👈 initialization happens here
```
**That’s Hoisting!**


**❌ Example with let and const**
```
console.log(b); // ❌ Error!

let b = 5;
```
```
console.log(c); // ❌ Error!

const c = 10;
```
- JavaScript hoists the name of b and c too...
- BUT! It doesn’t give them any value (not even undefined).
- This causes an error if you try to use them before they’re defined.


## ⚙️ How Hoisting Works for Each Type

| Keyword | Hoisted? | Gets a Value? Before Code Runs | What Happens if Accessed Early?            |
|---------|----------|--------------------------------|---------------------------------------------|
| `var`   | ✅ Yes   | ✅ `undefined`                 | ✅ No error, just `undefined`               |
| `let`   | ✅ Yes   | ❌ No                         | ❌ Error *(Temporal Dead Zone)*            |
| `const` | ✅ Yes   | ❌ No                         | ❌ Error *(Temporal Dead Zone)*            |


**🔍 Behind the Scenes (Example)**
```
var a = 2;
```
*JavaScript sees it like this:*
```
var a;      // 🛫 Hoisted to top
a = 2;      // ✍️ Assigned later
```


## 🧠 Quick Summary
- JavaScript lifts declarations to the top = this is called Hoisting.
- var is hoisted with the value undefined.
- let and const are also hoisted but do not get a value = 🧨 causes an error if used too early.
- Only declarations are hoisted — not values.


## 📝 Practice Questions:
1. What will this show?
```
console.log(x);
var x = 10;
```
2. What happens here?
```
console.log(y);
let y = 5;
```
3. Will this code work?
```
var score = 100;
console.log(score);
```
4. Try writing a program using `let` and see what happens if you use the variable before declaring it.
5. In your own words: What is hoisting?


*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck.  ♥*
