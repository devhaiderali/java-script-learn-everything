#  Re-assignment & Re-declaration:


In JavaScript, we use variables (boxes) to store values like numbers, words, or anything else.
Sometimes we want to change what's inside the box, and sometimes we might accidentally make the same box again.
Let’s learn both!


**🔄 1. Re-assignment — "Changing the value in the box"**
- Re-assignment means giving a new value to a variable that already has a value.
- You’re not creating a new variable — just updating the old one.
```
var a = 12;  // First value
a = 2;       // Re-assigned new value
console.log(a); // Shows 2
```
```
let b = 50;
b = 69;       // Re-assigned
console.log(b); // Shows 69
```
*💡 You can re-assign variables made with both `var` and `let`.*

---
**🆕 2. Re-declaration — "Trying to make the same box again"**
Re-declaration means using `var` or `let` to create a variable with the same name again.
This only works with `var`.
It gives an error with `let`.
**✅ `var` allows re-declaration:**
```
var x = 10;
var x = 20; // This is okay
console.log(x); // Shows 20
```
**❌ `let` does NOT allow re-declaration:**
```
let y = 5;
let y = 15; // ❌ Error! Cannot re-declare with let
```

## ✅ Quick Summary


| Action           | `var`     | `let`       |
|------------------|-----------|-------------|
| Re-assign value  | ✅ Yes    | ✅ Yes      |
| Re-declare       | ✅ Yes    | ❌ No (error) |


**🎯 Real-Life Example**
Imagine you have a notebook where you write your favorite number:
First, you write: `Favorite Number = 7`
Later, you change it to: `Favorite Number = 10` (✅ Re-assignment)
But then, you try to make a new page for `Favorite Number` again — same name, new page! That’s re-declaration.
With `var`, it's allowed. With `let`, the notebook says: ❌ "Hey! You already wrote that!"



## 📝 Practice Questions

Try these fun questions to test your understanding:

1. Can you re-assign a var variable? Try it!
2. Can you re-declare a let variable? What happens?
3. What will this show?
```
var name = "Ali";
var name = "Sara";
console.log(name);
```
4. What about this one?
```
let city = "Lahore";
let city = "Karachi";
console.log(city);
```
5. Try changing the value of a `let` variable — does it work?
---

*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck.  ♥*
