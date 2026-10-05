# 📚 Quantum Bookstore (Java)

A console-based bookstore management system developed in pure Java during my early stages of learning Object-Oriented Programming (OOP). Inspired by the Fawry Rise internship challenge, the project simulates a bookstore that manages different book types, maintains inventory, removes outdated books, and handles purchases with stock validation and delivery.

## ✨ Features

* **Book types:** Supports paper books with stock, e-books with file types, and showcase books that are display-only and not for sale.
* **Inventory management:** Adds and manages books using their ISBN.
* **Outdated book removal:** Removes books older than a specified number of years.
* **Book purchasing:** Validates book availability and stock, calculates the total price, and processes purchases.
* **Delivery:** Paper books are shipped to a physical address, while e-books are delivered by email.
* **Error handling:** Handles unavailable books, showcase books that cannot be purchased, and insufficient stock.

## 🧱 Design

| Class                      | Responsibility                                                       |
| -------------------------- | -------------------------------------------------------------------- |
| `Book` (abstract)          | Defines common book properties and the abstract `deliver()` behavior |
| `PaperBook`                | Represents physical books and manages stock                          |
| `EBook`                    | Represents digital books with a file type and email delivery         |
| `ShowcaseBook`             | Represents display-only books that cannot be purchased               |
| `QuantumBookstore`         | Manages inventory, removes outdated books, and handles purchases     |
| `QuantumBookstoreFullTest` | Demonstrates the complete bookstore workflow                         |

## 🧠 OOP Concepts

* **Abstraction:** Defines common book behavior through an abstract `Book` class.
* **Inheritance:** `PaperBook`, `EBook`, and `ShowcaseBook` extend the `Book` class.
* **Polymorphism:** The `deliver()` method behaves differently according to the book type.
* **Encapsulation:** Book data, stock, and operations are managed through dedicated classes and methods.

## 🛠️ Technologies

* Java
* Object-Oriented Programming (OOP)
* Java Collections (`HashMap`)
* Exception Handling
* Console-based Application

## 🚀 Getting Started

**Requirements:** JDK 11 or later.

```bash
git clone https://github.com/Shahdrabea2004/Quantum-Bookstore-Management.git
cd Quantum-Bookstore-Management
javac -d out src/*.java
java -cp out QuantumBookstoreFullTest
```

Alternatively, open the project in IntelliJ IDEA and run `QuantumBookstoreFullTest`.

## 📄 Sample Output

```text
Quantum book store: Book added - Java Basics
Quantum book store: Book added - Learn Python
Quantum book store: Book added - Rare Book
Quantum book store: Removed outdated book - Rare Book
Quantum book store: Sending paper book to 123 Street
Quantum book store: Book purchased - Java Basics
Quantum book store: Amount paid: 300.0
Quantum book store: Sending ebook to ebook@buyer.com
Quantum book store: Book purchased - Learn Python
```

## 🎯 Learning Outcomes

This project was developed during my early Java learning journey to practice applying OOP principles, designing class hierarchies, working with abstract classes and polymorphism, managing inventory with collections, and implementing business rules and exception handling.

## 👩‍💻 Author

**Shahd Rabea**
