# ATM-Simulator-System

ATM-Simulator-System is a Java Swing-based desktop application that simulates the core functionalities of an Automated Teller Machine (ATM). It allows users to perform banking operations such as login, deposit, withdrawal, fast cash, balance enquiry, mini statement, and PIN change.

## Features

- **User Authentication:** Login with card number and PIN.
- **Account Signup:** Multi-step signup process for new users.
- **Deposit & Withdraw:** Deposit and withdraw money with validation.
- **Fast Cash:** Quick withdrawal of preset amounts.
- **Balance Enquiry:** Check current account balance.
- **Mini Statement:** View recent transactions.
- **PIN Change:** Change account PIN securely.

## Project Structure

```
ATM-Simulator-System/
├── build.xml
├── manifest.mf
├── nbproject/
│   ├── build-impl.xml
│   ├── project.properties
│   └── ...
├── src/
│   └── ASimulatorSystem/
│       ├── Login.java
│       ├── Signup.java
│       ├── Signup2.java
│       ├── Signup3.java
│       ├── Deposit.java
│       ├── Withdrawl.java
│       ├── FastCash.java
│       ├── BalanceEquiry.java
│       ├── MiniStatement.java
│       ├── Pin.java
│       └── ...
```

## Prerequisites

- Java JDK 8 or higher
- MySQL database (for backend storage)
- [JCalendar library](https://toedter.com/jcalendar/) (for date selection)

## Setup & Build

1. **Clone the repository:**
    ```sh
    git clone <repo-url>
    cd ATM-Simulator-System
    ```

2. **Configure Database:**
    - Create a MySQL database and tables as required by the application.
    - Update database connection details in `Conn.java`.

3. **Add Dependencies:**
    - Ensure the MySQL JDBC driver and JCalendar JAR are included in your classpath.
    - Update the paths in `nbproject/project.properties` if needed.

4. **Build the Project:**
    - Using NetBeans: Open the project and click **Build**.
    - Using Ant:
      ```sh
      ant clean
      ant build
      ```

## Running the Application

- **Main Entry Point:**  
  Run `Login.java` to start the ATM simulator.

    ```sh
    java -cp dist/ASimulator.jar ASimulatorSystem.Login
    ```


## License

This project is for educational purposes.

---

**Note:**  
- For customization, refer to `build.xml` and `nbproject/build-impl.xml`.
- For troubleshooting, check the output pane in your IDE or terminal for error messages.

---
