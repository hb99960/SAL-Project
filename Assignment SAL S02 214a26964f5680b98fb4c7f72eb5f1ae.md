# S02

**Question 1 : Tasks:**

1. Create a `Student` class with:
    - `name` (string)
    - `age` (number)
    - `rollNo` (number)
    - A constructor to initialize all properties
    - A method `displayDetails()` that logs `Student: {name}, Age: {age}, Roll No: {rollNo}`
2. Create two instances of `Student` and call their `displayDetails()` method.

### 

**Question Task:**

1. Create a `Book` class with:
    - `title`, `author`, and `price`
    - Use `this` keyword in the constructor
    - Create an instance using `new Book(...)` and log all properties

 **Question Tasks:**

1. Create a class `Vehicle` with properties `brand` and `speed`, and a method `drive()` that logs `Driving at {speed} km/h`.
2. Create a class `Car` that **extends** `Vehicle` and adds:
    - A property `fuelType`
    - A method `refuel()` that logs `Refueling {fuelType}`
3. Create an instance of `Car` and call `drive()` and `refuel()` methods.

**Question Task:**

1. Create a base class `User` with:
    - `protected username`
    - A constructor accepting `username`
2. Extend this in `Admin` class and add:
    - A method `showUsername()` that accesses the protected variable using `super`

### 

**Question Tasks:**

1. Create an interface `Printable` with a method `print(): void`.
2. Create a class `Document` that implements `Printable`, and its `print()` method should log: `"Printing Document..."`
3. Create another class `Photo` that implements `Printable`, and logs: `"Printing Photo..."`
4. Call `print()` on both instances and store them in an array of type `Printable[]`.

---

### 

**Question Task:**

1. Create a class `Person` with a method `walk()`.
2. Create an interface `Coder` with method `code()`.
3. Create a class `Developer` that:
    - Extends `Person`
    - Implements `Coder`
    - Implements both `walk()` and `code()`.