# Object.freeze

Make complex constant variables immutable

## Mutable Object

```javascript
  "use strict";
  const MATH_CONSTANTS = {
    PI: 3.14
  };
  
  MATH_CONSTANTS.PI = 99;
  
  console.log(MATH_CONSTANTS.PI);
```

### Output:

```
99
```

## Immutable Object

```javascript
  "use strict";
  const MATH_CONSTANTS = {
    PI: 3.14
  };
  
  Object.feeze(MATH_CONSTANTS);
  
  MATH_CONSTANTS.PI = 99; // error
  
  console.log(MATH_CONSTANTS.PI);
```

### Output:

```
TypeError: Cannot assign to read only property 'PI' of object '#<Object>' 
```
