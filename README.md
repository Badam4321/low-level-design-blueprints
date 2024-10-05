# Low-Level Design Blueprints

## Table of Contents
- [Object-Oriented Programming](#object-oriented-programming)
  - [Components of OOP](#components-of-object-oriented-programming-oop-in-low-level-design-lld)
  - [Blocks of OOP](#blocks-of-oop)
  - [Pillars of OOP](#pillars-of-oop)

## Object-Oriented Programming
Once upon a time, in a bustling city, there was a young girl named Anita who loved to bake. She dreamed of opening her bakery, filled with delicious treats and happy customers. But little did she know, her baking passion would help her understand Object-Oriented Programming (OOP).
In her bakery:

- **Classes** are like recipes. A recipe for "cake" defines what ingredients (attributes) and steps (methods) are needed.
- **Objects** are the actual cakes she bakes using the recipe. Each cake can be a different flavor but follows the same recipe.
- **Encapsulation** is like wrapping the cake neatly in a box. Only Anita decides how and when to open it (control access to the cake).
- **Inheritance** is when she creates new recipes based on old ones, like "chocolate cake" from "cake," but with extra chocolate.
- **Polymorphism** is when she can bake different treats (cookies, cakes) using a common process (like "baking") but with slight differences.

### Components of Object-Oriented Programming (OOP) in Low-Level Design (LLD)

- **Classes:** A blueprint for creating objects. It defines attributes (data) and behaviors (methods). For example, a Car class may have attributes like make, model, and behaviors like start() or stop().
  
- **Objects:** Actual instances of classes. Each object has its own unique data and can perform actions. For instance, a specific Car object has a unique make and model and can start() or stop().

- **Abstraction:** Simplifies complex systems by focusing on important details and hiding unnecessary information. For example, when interacting with a Car object, you don't need to know how the engine works internally—just the methods like start().

- **Encapsulation:** Combines data and methods into a single unit (object), keeping some parts private and only allowing controlled access via methods. This prevents accidental modification and ensures data integrity.

- **Inheritance:** Allows a class (subclass) to inherit attributes and behaviors from another class (superclass). For example, ElectricCar can inherit from Car but have additional features like chargeBattery().

- **Polymorphism:** Enables one method to have different implementations in different contexts. For example, a start() method might work differently for a Car and an ElectricCar, but both use the same interface.

### Blocks of OOP
- **Classes and Objects:**
  - **Class:** A class in programming is a blueprint or template for creating objects. It defines the properties (attributes) and behaviors (methods) that the objects created from it will have. Think of a class like a recipe that outlines what ingredients (attributes) are needed and what steps (methods) to follow.
  - **Object:** Once a class is defined, objects can be created (instantiated) from it using the new keyword followed by the class name and constructor arguments.

#### Example of a Class in Java:
```java
// Defining a class named 'Cake'
class Cake {
    // Attributes (properties of the class)
    String flavor;
    double price;

    // Constructor to initialize the Cake objects
    public Cake(String flavor, double price) {
        this.flavor = flavor;
        this.price = price;
    }

    // Method (behavior of the class)
    public void bake() {
        System.out.println("Baking a " + flavor + " cake.");
    }
}
class Main{
  public static void main(String[] args){
      Cake c1 = new Cake();//Object creation
  }
}
```
- **Constructors**
  - **Defination Of Constructor :**  A constructor in object-oriented programming is a special type of method that is automatically called when an object of a class is created. Its primary purpose is to initialize the object's state, i.e., to assign values to the object's attributes (fields).
  - **Rules of constructors:**
    **Same Name as Class:** A constructor must have the same name as the class.</br>
    **No Return Type:** A constructor does not have a return type, not even void.</br>
    **Automatically Invoked:** Constructors are called automatically when an object is created using the new keyword.</br>
    **Can Be Overloaded:** A class can have multiple constructors with different parameters (constructor overloading).</br>
    **Cannot Be Inherited:** Constructors are not inherited by subclasses but can be called using super().</br>

  - **Types of Constructors**
    - **Default Constructor:**
    - If no constructor is explicitly defined, Java provides a default constructor.
    - This constructor takes no parameters and assigns default values to object attributes (like null for objects, 0 for numeric types).
    - ```java
      class Car {
    String model;
    int year;
}

public class TestCar {
    public static void main(String[] args) {
        Car myCar = new Car();  // Default constructor called
        System.out.println(myCar.model);  // null
        System.out.println(myCar.year);   // 0
    }
}
      ```

