# Classes in JavaScript

A class is a blueprint for creating objects.  It defines properties (data) and methods (functions) that the objects created from the class will have.  In JavaScript, the `class` keyword is used to define a class.  Class names conventionally start with a capital letter.

## Example: `Car` Class
exmp1:
```javascript


class Person {
    constructor(){
      this.name = 'Angela';
     this. age = 24;
      this.height = 1.59;
    }
  }
  const person = new Person();
  //console.log(Person.name);
  console.log("My name is " + person.name +". I am "+person.age + "years old.");
  
  ```

exmp2
```javascript
class Car {
  constructor(color) {  // Constructor with a parameter
    this.color = color; // Assigns the passed color to the instance
  }

  drive() { // Example method
    console.log("The " + this.color + " car is driving!");
  }
}

const myCar = new Car("red"); // Create a new Car object with the color "red"
console.log(myCar.color);      // Output: "red"
myCar.drive();                 // Output: "The red car is driving!"


const blueCar = new Car("blue"); //Create another instance with a diffrerent color
blueCar.drive(); // Output: "The blue car is driving"

```