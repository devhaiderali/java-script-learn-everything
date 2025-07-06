### *JavaScript Variable Declarations*

*Variable Declarations in JavaScript:*
- Imagine you have boxes to store your toys or snacks. In JavaScript, we have three “box types” to store information: var, let, and const. Let’s see how each one works!
---

  **A. var**
- Scope (where it works): Think of var as a big room where all boxes live. Whether you open a box inside a smaller play‐area (a function) or in the whole room (the global area), var will be found anywhere in that room.

- Redeclaration: You can put two boxes with the same name in that room. JavaScript won’t complain!

- Hoisting: Before you start playing, JavaScript pretends you already put an empty box named var on the shelf—so it exists but is empty (undefined) until you fill it.

**Real‐life Example:**
You have a big playroom. You drop a box labeled “LEGOs” anywhere in the playroom, and it’s always reachable. You could even drop another “LEGOs” box and JavaScript won’t mind.

**NOTE:** Don't worry about the terms you dont know, just wait for next modules we'll teach you everything just be patient for now focus on concept. THANK YOU!

  **B. let**
- Scope: let boxes live inside the smallest fence (a block) you create—like inside a circle you draw on the floor with chalk. Outside that circle, you can’t see or use that box.

- Redeclaration: You can’t name two boxes the same inside that circle—JavaScript will get upset.

- Temporal Dead Zone (TDZ): JavaScript knows you plan to create a let box, but until you actually write “fill the box,” it’s off‐limits. If you try to peek inside before you fill it, you get an error.

  **Real‐life Example:**
You draw a chalk ring on the floor and place a “Crayons” box inside it. Nobody outside the ring can grab crayons. Also, you can’t secretly sneak another “Crayons” box inside that ring.

**C. const**
- Scope: Just like let, const boxes live inside the chalk ring (block scope).

- Must Initialize: You have to put something in the box right when you create it—you can’t leave it empty.

- No Reassignment or Redeclaration: Once you name and fill your “Action Figures” box, you can’t change the contents to “Toy Cars” later, and you can’t make another “Action Figures” box in that same ring.

- Temporal Dead Zone (TDZ): Just like let, you can’t try to use the box before you actually create and fill it.

**Real‐life Example:**
You draw a chalk ring, and immediately place your “Secret Candy” inside a box labeled “Secret Candy.” You can’t replace it with anything else or make a second “Secret Candy” box inside that ring.

---

| Feature         | Description                  | let                          | const                        |
|-----------------|------------------------------|------------------------------|------------------------------|
| Scope         |Function or global        |Block `(inside { })` | Block `(inside { })`
| Can redeclare?| Yes               |No | No
| Must initialize?| No   |No	| Yes
| Can reassign? |Yes      |Yes	| No
| Hoisting behavior|Initialized as `undefined` | In TDZ until first line executes | In TDZ until first line executes

---
# Practice Problems:
**1. Identify the Scope:**
```
if (true) {
  var toy = "Ball";
  let game = "Puzzle";
}
console.log(toy);  // ?  
console.log(game); // ?
```
*What will each console.log show or error?*

**2. Redeclaration Check:**
```
let snack = "Chips";
let snack = "Fruit";
```
*Will this code run fine or cause an error? Why?*

**3. Hoisting Mystery:**
```
console.log(color); 
var color = "Blue";
```
*What does JavaScript print? Explain why.*

**4.Temporal Dead Zone:**
```
console.log(score); 
let score = 10;
```
*What happens when you run this? Why?*

**5. Constant Confusion:**
```
const pet;  
pet = "Dog"; 
```
*Is this allowed? Explain.*

**6. Spot the Correct Declaration:**
You have a variable ```age``` that you want to change later, and another variable ```birthYear``` that should never change once set. Which declarations ```(var, let, or const)``` would you choose for each? Explain your choice.

---
*Good luck with these! Try writing out the answers and referring back to the examples if you get stuck. ♥*
