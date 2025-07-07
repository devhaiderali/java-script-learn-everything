#  Scope (Global, Block, Functional).


In JavaScript, where you create your variable decides where you can use it.
This is called Scope — it’s like the area where your variable is allowed to play.

**🏡 1. Global Scope — "I can go anywhere!"**
**What it means:**
- If you make a variable outside of any curly braces `{}` or functions, it is global.
- You can use it anywhere in your program — even on line 3 or line 30000!

```
var game = "Football"; // Global

console.log(game); // Works here

function play() {
  console.log(game); // Works here too!
}
```
*💡 `var` is usually global if it’s made outside of a function.*


**📦 2. Block Scope — "I only stay in my block!"**
**What is a block?**
A block is anything inside curly braces `{ }`.
- let and const respect blocks.
- You can only use them inside the block where they were made.

```
{
  let color = "red";
  console.log(color); // ✅ This works
}

console.log(color); // ❌ Error! color is only inside the block
```
*💡 This is called Block Scope.*


**🧰 3. Function Scope — "I'm only inside my function!"**
- If you make a variable inside a function using `var`, it will only work inside that function.
- It won’t be available outside the function.
- 
```
function sayHi() {
  var message = "Hello!";
  console.log(message); // ✅ Works here
}

sayHi();
console.log(message); // ❌ Error! message is inside the function
```
*💡 var is function-scoped if it's created inside a function.*


## 🎨 **Quick Summary**

| Scope Type       | Where it works                  | Made with                       | Example use                    |
|------------------|----------------------------------|----------------------------------|--------------------------------|
| 🌐 Global Scope   | Anywhere                         | `var`, `let` (outside blocks/functions) | `var a = 5;`                  |
| 🛠️ Block Scope    | Only inside `{}`                 | `let`, `const`                  | `{ let x = 10; }`              |
| 🧪 Function Scope | Only inside function             | `var`                           | `function test() { var y = 2; }` |


## 🧠 Helpful Tips
- `va`r does not respect `{ }` blocks, but it does respect functions.
- `let` and `const` only work inside the block they’re made in — they respect curly braces `{}`.
- Global means: "I'm free to go anywhere!"
- Block means: "I stay in my room (block)."
- Function means: "I'm only in my function’s home."


## 📝 Practice Questions
1. Create a `var` variable outside any function. Can you use it inside a function?
2. Create a `let` inside a `{ }` block. Try using it outside the block. What happens?
3. Make a function with a `var` variable inside it. Try using that variable outside the function. What do you see?
4. What kind of scope is this?
```
{
  let fruit = "apple";
  console.log(fruit);
}
```
5. True or False: let variables can be used anywhere in the program once declared.
---

*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck.  ♥*
