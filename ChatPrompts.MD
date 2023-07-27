What is a class in JavaScript?

ChatGPT
In JavaScript, a class is a blueprint for creating objects with shared properties and methods. It is a way to define a new data type that encapsulates data and behavior related to that data. JavaScript introduced the concept of classes in ECMAScript 6 (ES6) to make object-oriented programming (OOP) more structured and easier to work with.

A class acts as a template or a constructor for creating objects that share similar characteristics. Each object created from a class is referred to as an instance of that class. These instances have their own unique data but share the same methods defined in the class.

Here's an example of a simple class in JavaScript:

javascript
Copy code
class Car {
  constructor(make, model, year) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  // Method to get the car's details
  getDetails() {
    return `${this.year} ${this.make} ${this.model}`;
  }

  // Method to start the car
  start() {
    return 'Engine started!';
  }
}

// Creating instances of the Car class
const car1 = new Car('Toyota', 'Corolla', 2020);
const car2 = new Car('Honda', 'Civic', 2019);

// Using the methods defined in the class
console.log(car1.getDetails()); // Output: "2020 Toyota Corolla"
console.log(car2.start());      // Output: "Engine started!"