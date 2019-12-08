# Object Literals

```javascript
const createPerson = (name, age, gender) => {

  return {
    name: name,
    age: age,
    gender: gender
  };

};

const rapha = createPerson("Raphael", 42, "M");
console.log(rapha);
```
>> {nome: "Raphael", age: 42, gender: "M"}

or

```javascript
const createPerson = (name, age, gender) => ({ name, age, gender });

const rapha = createPerson("Raphael", 42, "M");
console.log(rapha);
```
>> {nome: "Raphael", age: 42, gender: "M"}

or


```javascript
const createPerson = (name, age, gender) => ({ fullName : name, age, gender });

const rapha = createPerson("Raphael", 42, "M");
console.log(rapha);
```
>> {fullName: "Raphael", age: 42, gender: "M"}

