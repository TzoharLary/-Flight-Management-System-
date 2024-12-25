# Flight Management System

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

### Strategy Pattern:

Used for dynamic flight search strategies (e.g., by price, airline).


### 2. Composite Pattern

Organizes airlines and sub-airlines in a hierarchical structure

### 3. Observer Pattern

Notifies clients in real-time about flight updates (e.g., price, seat availability).

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
