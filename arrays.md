# Arrays

### Copy array

```javascript
const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;

(function() {
  arr2 = arr1; // Copy array instance
  arr1[0] = 'potato'
})();

console.log(arr2);
```
### Output:
```
["potato", "FEB", "MAR", "APR", "MAY"]
```


## Copy array elements (Spread Operator)
```javascript
const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;

(function() {
  arr2 = [...arr1]; // Spread Operator - Copy array elements
  arr1[0] = 'potato'
})();

console.log(arr2);
```

### Output:
```
["JAN", "FEB", "MAR", "APR", "MAY"]
```
