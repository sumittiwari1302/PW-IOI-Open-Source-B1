callback is a function that is passed as an argument to another function, so that it can be called later when needed.
Think of it like this:
"I'm busy right now. When you're done, call this function."
Simple example
function greet(name) {
  console.log("Hello " + name);
}

function processUser(callback) {
  const name = "Om";
  callback(name); // Calls the callback function
}

processUser(greet);