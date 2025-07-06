# Declaration & Initialization


Let’s learn how we give names and values to things in JavaScript using variables.  
Think of a variable like a box where you can store something — like a number or a word.


**📦 What is a Variable?**

A variable is a name for something you want to remember in your program —  
like a score, your name, or how many apples you have.

We can create (or “declare”) a variable using `var` or `let`.

---

**1️⃣ What is Declaration?**
👉 Declaration means you're telling the computer,
*"Hey! I'm going to use a box called `a`, but I’m not putting anything inside it yet."*
```
 var a;

```
OR
```
let a;

```
- You create the variable.
- But you don’t give it a value yet.
- It's like saying: "I have an empty box."
---
**2️⃣ What is Initialization?**
  👉 Initialization means you're putting the first value inside the box.
```
  a = 5;

```
- Now you're saying: “Let’s put the number 5 in the box called a.”
- This is the first time you’re giving it a value.
---

**3️⃣ Declaration + Initialization Together**
You can also declare and initialize a variable at the same time:
```
var a = 5;

```
OR
```
let a = 5;

```
- This means:

   - You made a box (a)

   - And put the number 5 in it right away.
---

**🔁 Same Works With let**
Just like `var`, you can also use `let`:
```
let name;
name = "Ali"; // Initialization
```
OR:
```
 let name = "Ali"; // Declaration + Initialization;

```
---

## ✅ Quick Recap

| Step           | What it means                   | Example                     |
|----------------|----------------------------------|-----------------------------|
| Declaration    | Making the box (no value yet)   | `var a;` or `let a;`        |
| Initialization | Giving it a first value         | `a = 10;`                   |
| Both Together  | Make box and put value right away | `var a = 10;`              |
---

## 🎯 Practice Questions:

Try these on your own! (Use your computer or a code playground like JSFiddle or Replit).

1. Declare a variable called `age` using `var`.
2. Now give `age` the value `12`.
3. Declare and initialize a variable called `color` with the value `"blue"` using `let`.
4. What’s the difference between:
  - `let fruit;`
  - `let fruit = "apple";`?
5. Can you create a variable named `score`, and set it to `100`?
---

*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck. ♥*
