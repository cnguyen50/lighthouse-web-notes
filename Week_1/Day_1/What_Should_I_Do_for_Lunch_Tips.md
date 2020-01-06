

const whatToDoForLunch = function(hungry, availableTime) {

  if (!hungry) {
    console.log("Get back to work");
  } else if (hungry && (availableTime < 20)) {
    console.log("I'll pick something up and eat it in the lab");
  } else if (hungry && (availableTime >= 20 && availableTime <= 30 )) {
    console.log("I'll try a place nearby");
  } else if (hungry && availableTime > 30) {
    console.log("Wait, I'm in a bootcamp and I should reconsider how much time I have to spare");
  } else {
    console.log("I don't know what to do!");
  }

};





/*
 * This is some test runner code that's simply calling our whatToDoForLunch function
 * defined above to verify we're making the right decisions. Do not modify it!
 */

console.log("I'm hungry and I have 20 minutes for lunch.");
whatToDoForLunch(true, 20);
console.log("---");

console.log("I'm hungry and I have 50 minutes for lunch.");
whatToDoForLunch(true, 50);
console.log("---");

console.log("I'm not hungry and I have 30 minutes for lunch.");
whatToDoForLunch(false, 30);
console.log("---");

console.log("I'm hungry and I have 15 minutes for lunch.");
whatToDoForLunch(true, 15);


### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascripting
function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}
```