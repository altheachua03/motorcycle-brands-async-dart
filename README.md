# Motorcycle Brands: Asynchronous Programming

## Week 11 Activity: Dart Programming – Async/Await

**Student Name:** Althea Chua  
**Block:** 3.1BSIT  
**Activity:** Week 11 Activity

## Learning Objectives

To understand and apply asynchronous programming in Dart using `Future`, `async`, `await`, and `Future.delayed` while retaining the Object-Oriented Programming (OOP) concepts learned in Week 10.

## Description

This Dart program extends the Week 10 Motorcycle Brands project by introducing asynchronous programming. It retains the abstract `Motorcycle` base class, the `HondaMotorcycle` and `YamahaMotorcycle` subclasses, encapsulation, polymorphism, method overriding, and the `MaintenanceReminder` mixin.

A new asynchronous method, `saveMotorcycleData()`, is added to the `Motorcycle` class. This method returns a `Future<String>` and uses `Future.delayed` to simulate saving motorcycle data with a two-second delay.

The `main()` function is declared as `async` and calls the new method using `await`. The program prints messages before and during the simulated saving operation to demonstrate that other statements can execute while the asynchronous operation is waiting. Once the operation finishes, the program displays the result.

The saving operation is simulated and does not store data in an actual database or fetch data from a real server.

## Features

- **Abstract Class:** Uses the `Motorcycle` base class to define common motorcycle properties and methods.
- **Inheritance:** Uses `HondaMotorcycle` and `YamahaMotorcycle` subclasses.
- **Polymorphism:** Displays motorcycle information through the shared `Motorcycle` type.
- **Method Overriding:** Provides specific implementations of `displayInfo()` and `describeMotorcycle()`.
- **Encapsulation:** Uses the private `_price` field and methods to retrieve and update the motorcycle price with validation.
- **Mixin:** Uses `MaintenanceReminder` to demonstrate reusable maintenance reminder functionality.
- **Constructors:** Initializes motorcycle objects using constructors and `super()`.
- **List Usage:** Stores motorcycle objects in a `List<Motorcycle>` and displays their information using a loop.
- **Asynchronous Method:** Adds `saveMotorcycleData()`, which returns a `Future<String>`.
- **Future.delayed:** Simulates a two-second saving operation.
- **Async/Await:** Uses `async` and `await` to handle the asynchronous operation and display its result after completion.
- **Non-Blocking Demonstration:** Prints messages before the delayed result to demonstrate asynchronous execution.

## Technologies Used

- Dart Programming Language
- Visual Studio Code
- Dart SDK

## How to Run

1. Make sure the Dart SDK is installed on your computer.
2. Open the project folder in Visual Studio Code.
3. Save the Dart source code in a file named `motorcycle_async.dart`.
4. Open the terminal in the project folder.
5. Run the following command:

   ```bash
   dart run motorcycle_async.dart
   ```

6. Check the terminal output to verify the motorcycle information, updated price, maintenance reminder, and asynchronous saving demonstration.
7. Run the program at least twice to confirm that the delay and the order of printed messages remain consistent.

## Expected Output

The program displays the following:

- Honda and Yamaha motorcycle information.
- Different descriptions for each motorcycle.
- The original and updated price of the Honda motorcycle.
- A maintenance reminder demonstrating the mixin functionality.
- A message indicating that the motorcycle data is about to be saved.
- A waiting message displayed before the simulated saving operation finishes.
- A success message displayed after the two-second delay.
- A completion message after the saving operation finishes.

## Conclusion

This activity extends the Week 10 Motorcycle Brands project by introducing asynchronous programming in Dart. Through `Future`, `Future.delayed`, `async`, and `await`, the program demonstrates how to simulate a time-consuming operation and retrieve its result after completion. It also retains the OOP concepts previously implemented, showing how asynchronous methods can be incorporated into an existing Dart class-based program.
