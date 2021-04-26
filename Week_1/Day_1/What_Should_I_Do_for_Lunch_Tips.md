### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.


```javascript
const whatToDoForLunch = function(hungry, availableTime) {

  if (hungry === true) {
    if (availableTime < 20) {
      console.log("Pick up some food and eat in the Lab!");
    } else if (availableTime < 30) {
      console.log("You deserve break! Go to try any place in Gastown");
    } else {
      console.log("You should probably reconsider taking that much break. You are in a bootcamp!");
    }

  } else {
    console.log("Get back to work! Wait until you are hungry.");
  }

};

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
```