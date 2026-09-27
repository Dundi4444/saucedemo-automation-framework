# SauceDemo QA Automation Framework

![Java](https://img.shields.io/badge/Language-Java-orange.svg)
![Selenium](https://img.shields.io/badge/Tools-Selenium_WebDriver_4.x-green.svg)
![TestNG](https://img.shields.io/badge/Framework-TestNG-blue.svg)
![Build](https://img.shields.io/badge/Build-Maven-red.svg)
![Design Pattern](https://img.shields.io/badge/Pattern-Page_Object_Model_(POM)-yellow.svg)

## 📌 Overview

This project is a functional, production-ready QA Automation Testing Framework built for **[SauceDemo (Swag Labs)](https://www.saucedemo.com/)**. 

Transitioning from initial manual test cases, this repository implements an enterprise-standard **Page Object Model (POM)** architecture using Java, Selenium WebDriver, TestNG, and Maven. It features robust dynamic locator strategies, clean driver management, cross-browser parameterization, and automated execution logging.

---

## 🛠️ Tech Stack & Dependencies

* **Programming Language:** Java 17+
* **Automation Tool:** Selenium WebDriver 4.x
* **Testing Framework:** TestNG 7.x
* **Build & Management Tool:** Apache Maven
* **IDE:** Eclipse / IntelliJ IDEA
* **Design Pattern:** Page Object Model (POM)

---

## 📁 Project Architecture

```text
saucedemo-automation-framework/
├── src/
│   ├── main/java/com/saucedemo/
│   │   ├── pages/                   # Page Object Classes
│   │   │   ├── BasePage.java        # Core explicit wait & interaction wrappers
│   │   │   ├── LoginPage.java       # Locators & actions for Login
│   │   │   └── HomePage.java        # Locators & actions for Product Catalog
│   │   └── utils/
│   │       └── DriverFactory.java   # WebDriver initialization (Chrome, Firefox, Edge)
│   └── test/java/com/saucedemo/
│       └── tests/                   # Automated Test Suites
│           ├── BaseTest.java        # Setup (@BeforeMethod) and Teardown (@AfterMethod)
│           ├── LoginTest.java       # Authentication validation tests
│           └── CartAndSearchTest.java # Catalog interaction & cart count assertions
├── testng.xml                       # Execution suite & parameter setup
├── pom.xml                          # Maven dependencies & build configurations
└── README.md                        # Documentation
