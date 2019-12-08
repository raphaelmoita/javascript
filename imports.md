# Imports

### Links
- https://javascript.info/import-export

### One mmethod:
- import { capitalizeString } from "./functions";

### Everything
- import * as functions from "./functions";

```javascript
# functions.js
const capitalizeString = str => str.toUpperCase()
export { capitalizeString };

export const foo = "bar";
export const bar = "foo";

# runner.js
 
import { capitalizeString } from "./functions"
const cap = capitalizeString("hello!");

console.log(cap);
```

### Output:

```
HELLO
```
