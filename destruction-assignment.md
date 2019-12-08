# Destruction Assignment

```javascript
const AVG_TEMPERATURES = {
  today: 77.5,
  tomorrow: 79
};

const { tomorrow : tempOfTomorrow } = AVG_TEMPERATURES; // change this line

console.log(tempOfTomorrow);
```

### Output:

```
79
```

## Nested 

```javascript
const LOCAL_FORECAST = {
  today: { min: 72, max: 83 },
  tomorrow: { min: 73.3, max: 84.6 }
};

const { tomorrow : { max : maxOfTomorrow }} = LOCAL_FORECAST; 

console.log(tempOfTomorrow);
```

### Output:
```
84.6
```

## Destruction parameter

```javascript
const stats = {
  max: 56.78,
  standard_deviation: 4.34,
  median: 34.54,
  mode: 23.87,
  min: -0.75,
  average: 35.85
};
const half = ({ max, min }) => (max + min) / 2.0;

console.log(half(stats)); 
```
### Output:
```
28.015
```

## Array

```javascript
const [z, x, , ,y] = [1, 2, 3, 4, 5, 6];
console.log(z, x, y);
```
### Output:
```
84.6
```

## Swifting elements

```javascript
let a = 1, b = 2;

(() => {
  "use strict";
  [a, b] = [b, a]
})();

// or simply [a, b] = [b, a]

console.log(a); 
console.log(b); 
```
### Output:
```
2
1
```

## Reassigning array elements

``` javascript
const source = [1,2,3,4,5,6,7,8,9,10];
const [ , , ...arr] = source; 
console.log(arr); 
console.log(source);
```

### Output:
```
[99, 3, 4, 5, 6, 7, 8, 9, 10]
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```
