# Ayush Gurung VIVA Preparation

This document is designed to help you prepare for your VIVA, focusing on your assigned tasks and the core C# and OOP concepts that may be asked. It includes both basic and advanced questions, with clear explanations and examples relevant to your project.

---

## 1. Core Concepts & Definitions

### What is Inheritance?
- **Definition:** Inheritance is an OOP principle where a class (child/derived) inherits properties and methods from another class (parent/base).
- **Example in Project:**
  - If you have a base class `Person` and `Customer` or `Staff` inherit from it, they get all properties/methods of `Person`.
  - In C#: `public class Customer : Person { ... }`
- **Why Use It?**
  - Code reuse, logical hierarchy, and easier maintenance.

### What is a Constructor?
- **Definition:** A constructor is a special method in a class that is called when an object is created. It initializes the object’s state.
- **Example in Project:**
  - `public Customer(string name) { this.Name = name; }`
- **Default vs Parameterized:**
  - Default: No parameters.
  - Parameterized: Takes arguments to set initial values.

### What is Dependency Injection?
- **Definition:** A design pattern where dependencies (services, repositories) are provided to a class, rather than the class creating them itself.
- **Example in Project:**
  - Controllers receive services via constructor injection: `public StaffSalesInvoicesController(ISalesInvoiceService service) { ... }`
- **Why Use It?**
  - Improves testability, flexibility, and decouples components.

### What is a DTO?
- **Definition:** Data Transfer Object. Used to transfer data between layers (e.g., from frontend to backend) without exposing internal models.
- **Example:** `SalesInvoiceDto`, `CustomerDto`

### What is an Interface?
- **Definition:** An interface defines a contract (methods/properties) that implementing classes must fulfill.
- **Example:** `public interface ICustomerService { ... }`

---

## 2. OOP Four Pillars (with Project Examples)

1. **Encapsulation:**
   - Wrapping data and methods into a single unit (class).
   - Example: `Customer` class with private fields and public methods.
2. **Abstraction:**
   - Hiding complex implementation details and showing only the necessary features.
   - Example: Service interfaces hide logic from controllers.
3. **Inheritance:**
   - Explained above.
4. **Polymorphism:**
   - Ability to use different classes through the same interface.
   - Example: Multiple services implementing the same interface, used interchangeably.

---

## 3. Project-Specific Questions

### Q: How is the loyalty program implemented?
- When a sales invoice is created, the backend checks if the total exceeds 5000. If yes, a 10% discount is applied before saving the invoice.
- This logic is encapsulated in the service layer, not the controller.

### Q: How is payment handled?
- After invoice creation, payment details are sent to the backend, which updates the payment status in the database.
- Only after successful payment is the loyalty discount finalized.

### Q: Which controllers and DTOs are involved in your tasks?
- Controllers: `StaffCustomersController`, `StaffSalesInvoicesController`, `StaffPartsController`, `CustomerPaymentsController`
- DTOs: `CustomerDtos`, `SalesInvoiceDtos`, `PartDtos`, `VehicleMaintenanceAiDtos`

---

## 4. Advanced/External Questions

### Q: What is the difference between an abstract class and an interface?
- **Abstract Class:** Can have method implementations and fields. Used for base classes.
- **Interface:** Only method/property signatures, no implementation. Used for contracts.

### Q: How does polymorphism work in your project?
- Services implement interfaces, so you can swap implementations without changing the controller code.

### Q: What is the SOLID principle?
- Five design principles for writing maintainable code:
  1. **S**ingle Responsibility
  2. **O**pen/Closed
  3. **L**iskov Substitution
  4. **I**nterface Segregation
  5. **D**ependency Inversion

### Q: How do you ensure security in your API?
- Use authentication (e.g., JWT), authorization, input validation, and avoid exposing sensitive data.

### Q: How is error handling managed?
- Using try-catch blocks, returning appropriate HTTP status codes, and error messages in API responses.

---

## 5. Sample Answers

- **Q:** What is inheritance?
  - **A:** Inheritance allows a class to acquire properties and methods from another class. For example, in our project, if `Customer` inherits from `Person`, it gets all the fields and methods of `Person`.

- **Q:** What is a constructor?
  - **A:** A constructor is a special method that initializes a new object. For example, `public Customer(string name)` sets the name when creating a customer.

- **Q:** How is dependency injection used?
  - **A:** Services are injected into controllers via constructors, making the code more modular and testable.

---

## 6. Tips for VIVA
- Be confident and clear in your explanations.
- Relate answers to your project whenever possible.
- If you don’t know an answer, explain your thought process.
- Use examples from your codebase to illustrate concepts.

---

Good luck! You are well prepared for both basic and advanced questions.
