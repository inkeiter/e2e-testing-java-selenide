# Bank App E2E Tests (UI + API)

> 🇷🇺 Русская версия: [README.ru.md](README.ru.md)

This project contains end-to-end (E2E) automated tests covering both the user interface (UI) and the API of a test banking application.

## 🎯 Project Goal

To demonstrate the ability to write reliable UI tests using the Page Object pattern, generate test data, and verify that the API works correctly. The project is integrated with a continuous integration (CI) system.

## 🛠 Tech Stack

* **Language:** Java 11
* **UI testing:** Selenide 6, Selenium WebDriver
* **API testing:** RestAssured, Gson (for JSON parsing)
* **Test framework:** JUnit 5
* **Data generation:** JavaFaker (random valid data for forms)
* **Build tool:** Gradle
* **CI/CD:** AppVeyor

## 🚀 Implemented Checks

1. **UI tests (Selenide):**
   * Logging in to the system.
   * Filling in forms with randomly generated data (JavaFaker).
   * Checking navigation and the display of interface elements.
2. **API tests (RestAssured):**
   * Sending requests to the application's endpoints.
   * Validating server responses and JSON structure.
3. **CI integration:**
   * An `appveyor.yml` file is configured to automatically start the application server and run the tests in headless mode (without a graphical interface) on every push.

## ⚙️ How to Run Locally

1. Make sure Java 11 is installed.
2. Clone the repository.
3. Run the tests from the terminal:
   * On Windows: `gradlew.bat test`
   * On Mac/Linux: `./gradlew test`

This project was created as part of my test automation training.
