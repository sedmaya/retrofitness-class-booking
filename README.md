# 🏋️ retrofitness-booking-automation

An automated UI testing suite built with **Selenium**, **Cucumber (BDD)**, and **TestNG** designed to automate the process of enrolling in gym classes or joining waitlists on the RetroFitness member portal.

## 🌟 Features

*   **Automated Enrollment:** Automatically signs up for specific classes (Pilates, Barre, Yoga, etc.) based on predefined schedules.
*   **Waitlist Management:** Smartly handles "Join Waitlist" actions if a class is full.
*   **Parallel Execution:** Configured for parallel test execution using TestNG for faster results.
*   **Rich Reporting:** Integrated with **Cluecumber** and **Cucumber HTML reports** for detailed visual feedback.
*   **Page Object Model:** Modular design for high maintainability.

---

## 🛠️ Prerequisites

*   **Java 17** or higher.
*   **Maven** installed.
*   **Chrome** or **Firefox** browser.

---

## 🚀 Getting Started

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/sedmaya/retrofitness-booking-automation.git
    cd retrofitness-booking-automation
    ```

2.  **Configuration:**
    The project uses environment variables or a properties file for credentials. Ensure you do not commit real credentials to the repository.
    
    Update `src/main/java/properties/config.properties`:
    ```properties
    browser=chrome
    ```

3.  **Run the Automation:**
    Execute the following Maven command to run all features:
    ```bash
    mvn clean verify
    ```

---

## 📂 Project Structure

*   `src/main/java/pageObjects`: Contains reusable Page Objects.
*   `src/test/java/stepDefinitions`: BDD step implementations.
*   `src/test/resources/features`: Cucumber feature files defining class booking scenarios.
*   `src/main/java/driver`: Custom `DriverFactory` utilizing Selenium Manager for automatic driver handling.

---

## 📊 Reporting

After execution, reports can be found in:
*   `target/generated-report/index.html` (Cluecumber Report)
*   `target/cucumber-html-report.html` (Standard HTML Report)

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
