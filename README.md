# API Automation Framework with Cucumber and Rest Assured

This is a robust API Test Automation Framework built using **Java**, **Cucumber**, **Rest Assured**, and **Maven**.  
This project has been customized and enhanced by **Bhanu Chaitanya Abbaraju** as a Proof of Concept (POC) to showcase practical API testing implementation for scalable and maintainable testing.

---

## 🛠️ Tech Stack

- Java 11+
- Maven
- Cucumber
- Rest Assured
- JUnit / TestNG
- JSONPath
- Log4j (optional if integrated)

---

## ✅ Prerequisites

Before using this project, ensure the following are installed:

- Java JDK 11 or higher
- Maven 3.x
- IDE (such as IntelliJ or Eclipse)

---

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/bhanuchait/api_testing.git
   cd api_testing
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

---

## 🚀 Running the Tests

Run all tests:

```bash
mvn test
```

Run tests with specific tags:

```bash
mvn test -Dcucumber.filter.tags="@Smoke"
```

---

## 📁 Project Structure

```
src
├── main
│   └── java
├── test
│   ├── java
│   │   ├── stepDefinitions
│   │   ├── runners
│   │   └── utilities
│   └── resources
│       ├── features
│       └── config.properties
```

---

## ✅ Sample Test Case

```gherkin
Feature: Sample API validation

  Scenario: Validate GET User API
    Given User sets GET API endpoint
    When User sends GET request
    Then API response status should be 200
    And Response should contain user data
```

---

## 🔧 Enhancements in This POC

- Reorganized package structure for clarity
- Added environment-specific configuration support
- Enhanced step definitions for reusability and readability
- Introduced utility functions for dynamic token and header handling
- Parameterized endpoint URLs and headers via config
- Added tagging support for test selection
- (Optional) Integrated basic logging and reporting mechanisms

---

## 👤 Author

Maintained and enhanced by **Bhanu Chaitanya Abbaraju**
Made modifications from different sources in the ineternet

---

## 📄 License

This project is developed as a **Proof of Concept** and is not bound to any open-source license.
