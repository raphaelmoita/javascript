# Functions

```javascript
function doSomething() {
   return "hey";
}

const doSomething = function() {
   return "hey";
}

const doSomething = () => {
   return "hey";
} 

const doSomething = () => "hey";

const concat = (str1, str2) => str1 + str2;

// Define a default value
const concat = (str1, str2 = "!!!") => str1 + str2;

// Params
const concat = (...strs) => strs.reduce((str1, str2) => str1 + str2);
``` 
