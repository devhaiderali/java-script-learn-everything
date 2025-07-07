# Temporal Dead Zone (TDZ)


**🧐 What is the Temporal Dead Zone?**
The Temporal Dead Zone is a fancy name for a place in your code where a variable exists, but you can’t use it yet. 😮
🔍 Simple Definition:
The time between when a `let` or `const` variable is found by JavaScript and when you give it a value is called the Temporal Dead Zone.

**🚫 Example (TDZ in Action)**
```
console.log(age); // ❌ Error! TDZ

let age = 10;
```
- Here, you are trying to use the variable `age` before it's given a value.
- JavaScript knows that `age` is declared with `let`, but it won’t let you use it until it reaches the line where it gets a value.
- So the space above `let age = 10;` is the TDZ for `age`.


**✅ But var is different!**
```
console.log(score); // ✅ Shows: undefined

var score = 20;
```
- With `var`, JavaScript says: “Okay, you didn’t give a value yet, but I’ll still let you use it as `undefined`.”
- So, `var` does not have TDZ. It just gives you `undefined` if you use it too early.


## 🎯 Quick Summary

| Feature                      | `let` / `const`             | `var`                          |
|-----------------------------|-----------------------------|--------------------------------|
| Has TDZ                     | ✅ Yes                      | ❌ No                          |
| Can use before value given? | ❌ No *(gives error)*       | ✅ Yes *(shows `undefined`)*  |

**🧠 Think of it Like This:**
Imagine you’re in school and your teacher has written your name on the roll call, but your seat is still empty.
Until you sit down and say "Here!", the teacher knows you exist, but won’t count you.
That “before-you-sit-down” time is like the Temporal Dead Zone — the name is there, but it’s not usable yet.


## 📝 Practice Questions:
Try these and see what happens:

1. What do you think this will show?
```
console.log(myName);
let myName = "Ali";
```
2. Try this one — does it work?
```
console.log(city);
var city = "Lahore";
```
3. Can you explain what the TDZ is in your own words?
4. Create a variable using `let` and try to log it before and after giving it a value.
5. Which variables will give an error if used too early: `var`, `let`, or `const`?
---

*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck.  ♥*
