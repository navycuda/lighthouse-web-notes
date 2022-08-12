### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  let result = "If you're not hungry, you're stalling.  Back to work.";
  if (hungry) {
    if (availableTime < 20) {
      result = "Grab a snack or prepared meal.";
    } else if (availableTime <= 30) {
      result = "Take a break, make yourself something nice to eat.";
    } else {
      result = "Unsatisfactory allocation of time, reconsider.";
    }
  }
  console.log(result);
};
```