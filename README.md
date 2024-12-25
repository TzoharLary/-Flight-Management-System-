# Flight Management System

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Table of Contents
- [Description](#description)
- [Features](#features)
- [Design Patterns](#design-patterns)
  - [Strategy Pattern](#1-strategy-pattern)
  - [Composite Pattern](#2-composite-pattern)
  - [Observer Pattern](#3-observer-pattern)
- [Installation](#installation)
- [Usage](#usage)
- [Contact](#contact)

## Description

The **Flight Management System** is a Java-based console application designed for managing and searching flights based on various criteria such as price, departure time, flight duration, and airline. This project is developed as a homework assignment for an Object-Oriented Programming (OOP) course and incorporates several design patterns to enhance flexibility, maintainability, and scalability.

## Features

- **Flight Search**: Search flights by price, airline, duration, or departure time.
- **Airline Management**: Manage airlines, including parent and sub-airlines.
- **Real-time Notifications**: Receive updates on flight changes using the Observer pattern.
- **Hierarchical Structure**: Organize airlines and flights using the Composite pattern.
- **Flexible Search Strategies**: Utilize different search strategies with the Strategy pattern.
- **Client Management**: Create and manage client profiles with name and account balance.

## Design Patterns

### 1. Strategy Pattern

Allows dynamic selection of flight search strategies (e.g., by price, departure time).

**Advantages:**
- **Flexibility**: Change search strategies at runtime without altering existing code.
- **Extensibility**: Easily add new search strategies.
- **Maintainability**: Separate algorithms from their usage.

**Example:**
```java
public class SearchByPrice implements SearchStrategy {
    // Implementation for searching flights by price
}
```

### 2. Composite Pattern

Enables the hierarchical organization of airlines and sub-airlines, allowing centralized management of flights.

**Advantages:**
- **Flexibility**: Easily manage hierarchical structures of airlines.
- **Extensibility**: Add new airlines or sub-airlines without affecting existing code.
- **Maintainability**: Uniform treatment of individual airlines and composites.

**Example:**
```java
public class Airline {
    Set<Flight> flights = new HashSet<>();
    Set<Airline> subAirlines = new HashSet<>();
    // Methods to add flights and sub-airlines
}
```

### 3. Observer Pattern

Facilitates real-time notifications to clients about changes in flight details (e.g., price updates, seat availability).

**Advantages:**
- **Real-time Updates**: Clients receive immediate notifications on flight changes.
- **Customization**: Clients can subscribe to specific updates.
- **Efficiency**: Manage and send updates to multiple observers efficiently.

**Example:**
```java
public class ObservableFlight extends Flight {
    // Implementation of Observer pattern
}
```

## Installation

### Prerequisites

- **Java Development Kit (JDK) 8** or higher
- **Git**

### Steps

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/TzoharLary/FinalEX_OOP.git
    ```

2. **Navigate to the Project Directory:**
    ```bash
    cd FinalEX_OOP
    ```

3. **Compile the Project:**
    ```bash
    javac -d bin src/OOP_Q1/*.java
    ```

4. **Run the Application:**
    ```bash
    java -cp bin OOP_Q1.Main
    ```

## Usage

Upon running the application:

1. **Create a Client:**
   - Enter your name and press Enter again.
   - Enter your account balance.

2. **Choose a Search Option:**
   - **1**: Search by price
   - **2**: Search by airline
   - **3**: Search by duration
   - **4**: Search by departure time

3. **Perform Searches:**
   - Follow prompts to input search criteria.
   - View search results based on chosen criteria.

4. **Continue or Exit:**
   - After each search, choose to perform another search or exit the application.

## Contact

- **Name:** Tzohar Lary
- **Email:** tzohary1234@gmail.com

---

Thank you for using the **Flight Management System**! If you have any questions or encounter any issues, feel free to reach out.
