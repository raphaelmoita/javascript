# Classes

```javascript

class Thermostat {

    constructor(fahrenheit) {
      this._celsius = 5/9 * (fahrenheit - 32); // to celsius
    }
    
    get temperature(){
      return this._celsius;
    }
    
    set temperature(celsius){
      this._celsius = celsius;
    }
}

const thermos = new Thermostat(76); 
let celsius = thermos.temperature; 
console.log(celsius);
thermos.temperature = 30;
console.log(celsius);
```

### Output:

```
24.444444444444446
30
```
