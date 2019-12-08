# Javascript

### Variable

- var: It has global scope (doesn't matter where it was defined)
- let: It has block scope and allows vallue change
- const: It has block scope and NOR allows value change
  
  ## Let
  ```javascript
  let name = "Rapha";
  
  if (true) {
     let name = "Mari";
     console.log("# " + name);
  }
  
  console.log("@ " + name);
  
  ```
  
  ### Output:
  ```
  # Mari
  @ Rapha
  ```
  
  ## Var
  ```javascript
  var name = "Rapha";
  
  if (true) {
     name = "Mari";
     console.log("# " + name);
  }
  
  console.log("@ " + name);
  
  ```
  Or
  
  ```javascript  
  if (true) {
     var name = "Mari";
     console.log("# " + name);
  }
  
  console.log("@ " + name);
  ```
  
  ### Output:
  
  ```
  # Mari
  # Mari
  ```
  
  ### Const
  
  ```javascript  
  if (true) {
     const name = "Mari";
     console.log("# " + name);
  }
  
  console.log("@ " + name); // ReferenceError: name is not defined
  ```
  
  ### Output:
  ```
  ReferenceError: name is not defined
  ```
  
```javascript  
  const name = "Rapha";
  
  if (true) {
     let name = "Mari";
     console.log("# " + name);
  }
  
  console.log("@ " + name);
  ```
  
  ### Output:
  ```
  # Mari
  @ Rapha
  ```
