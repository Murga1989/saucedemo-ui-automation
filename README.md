# Sauce Labs Demo - UI Test Automation Framework

## 📖 Overview

This repository contains a UI Test Automation Framework for the Sauce Labs demo e-commerce website, "[Swag Labs](https://www.saucedemo.com/)". The framework is built to be scalable and maintainable, following industry best practices to ensure robust and reliable test execution.

The primary goal of this project is to automate and validate key user journeys, ensuring the core functionalities of the application work as expected.

![Sauce Demo Website](https://i.imgur.com/k2msC5d.png)

## ✨ Features Automated

The test suite covers the following critical user scenarios:

-   **Login Module:**
    -   Successful login with a valid standard user.
    -   Failed login attempt with a locked-out user, verifying the specific error message.
-   **End-to-End Purchase Flow:**
    1.  User logs in successfully.
    2.  An item ("Sauce Labs Backpack") is added to the shopping cart from the products page.
    3.  User proceeds to the shopping cart and initiates checkout.
    4.  User fills in their personal information on the checkout page.
    5.  The purchase is finalized, and a "Thank you for your order!" success message is verified.

## 🛠️ Technology Stack

This project leverages a modern stack of technologies and design patterns for effective test automation:

-   **Language:** **Java**
-   **Browser Automation:** **Selenium WebDriver**
-   **Test Framework:** **TestNG**
-   **Build & Dependency Management:** **Apache Maven**
-   **Design Pattern:** **Page Object Model (POM)** for clean separation of test logic and page elements.

## 🏗️ Project Structure

The framework is organized using the Page Object Model (POM) to enhance test maintenance and reduce code duplication.

```
selenium-saucedemo-project/
├── pom.xml
└── src/
    └── test/
        └── java/
            └── com/
                └── saucedemo/
                    ├── base/         # BaseTest class for browser setup and teardown
                    ├── pages/        # Page Object classes for each page of the application
                    │   ├── LoginPage.java
                    │   ├── ProductsPage.java
                    │   ├── CartPage.java
                    │   └── CheckoutPage.java
                    └── tests/        # TestNG test classes containing the test logic
                        ├── LoginTest.java
                        └── E2ETest.java
```

## 🚀 Getting Started

### Prerequisites

To run this project on your local machine, you will need the following installed:

-   Java Development Kit (JDK) 11 or higher
-   Apache Maven
-   Google Chrome Browser

### How to Run the Tests

1.  **Clone the repository to your local machine:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/selenium-saucedemo-project.git](https://github.com/YOUR_USERNAME/selenium-saucedemo-project.git)
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd selenium-saucedemo-project
    ```

3.  **Run the tests using Maven:**
    This command will clean the project, compile the code, and execute all the TestNG tests.
    ```bash
    mvn clean test
    ```

The test results will be displayed in your terminal.

## 🎬 Demo of Tests Running

*(Here, you can embed a GIF showing your automation scripts running. This is highly recommended as it provides an immediate, impressive visual of your work.)*

![Tests Running GIF](https://your-gif-url-here.gif)
