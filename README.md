# Try to use ES6 to let your code more powerful

### Default parameters

```
// Before ES6
function add(num1, num2) {
 return num1+num2;
}
add (5,2); //returns 7
add(3); //returns NaN as num2 is undefined

// ES6
function add(num1, num2=10) {
 return num1+num2;
}
add (5,2) //returns 7
add(3) //returns 13 as num2 has default value = 10
```

### Template literals
```
let myName = 'Diogo';
let myRole = 'Frontend engineer';
console.log(`My name is ${myName} and I am a ${myRole}.`); // My name is Diogo and I am a Frontend engineer.
```

### Destructuring assignment - with it is possible get values using variables
```
// Destructuring an array
let myName, myRole;
let array = ['Diogo', 'Frontend engineer'];
[myName, myRole] = array;
console.log(myName, my Role); //Diogo Frontend engineer

//Destructuring an object
let myName, myRole;
let object = {myName:'Diogo', myRole:'Frontend engineer'};
{myName, myRole}=object;
console.log(myName, myRole); //Diogo Frontend engineer
```

### Arrow function expressions
```
// With function
function getName(firstName,lastName){
 return `${firstName} ${lastName}`;
}
console.log(getName('Diogo','Soares');

// With Arrow function
let getName = ((firstName,lastName)=> `${firstName} ${lastName}`);
console.log(getName('Diogo','Soares');
```



