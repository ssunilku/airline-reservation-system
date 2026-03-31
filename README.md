

---

# ✈️ Airline Reservation System (C++ & MySQL)

A robust **Backend-focused console application** designed to manage flight schedules and automate seat reservations. This project demonstrates the integration of **Object-Oriented Programming (C++)** with **Relational Databases (MySQL)** to achieve real-time data persistence.

## 🚀 Key Features
* **Database Connectivity**: Establishes a secure link with a MySQL server using the **MySQL C API**.
* **Automated Data Initialization**: Automatically populates the database with default flight information (Flight Number, Route, and Seat Capacity) upon startup.
* **Real-time CRUD Operations**:
    * **Read**: Fetches and displays live flight availability from the database.
    * **Update**: Implements reservation logic by validating seat availability and decrementing counts via SQL.
* **Data Integrity**: Includes conditional checks to prevent overbooking once a flight reaches zero capacity.
* **Clean CLI**: Features a menu-driven interface using Windows-specific process management (`cls`, `Sleep`).

## 🛠️ Technical Stack
* **Language**: C++
* **Database**: MySQL 8.0+
* **API/Driver**: MySQL C Connector (`libmysql`)
* **Key Concepts**: Object-Oriented Programming (Classes/Encapsulation), SQL Query Construction, Type-Casting (`stringstream`, `atoi`).

## 📂 Project Logic
The application acts as a **Middleware** between the user and the database:
1.  **Object Mapping**: Uses a `Flight` class to model data in memory.
2.  **SQL Execution**: Converts C++ logic into raw SQL strings for the database engine to process.
3.  **Type Synchronization**: Manages the conversion between SQL string outputs and C++ integer logic to ensure accurate calculations.

## 🔧 Setup & Installation
1.  **Prerequisites**:
    * Install **MySQL Server**.
    * Create a database named `mydb` and a table named `Airline`.
2.  **Configuration**:
    * Update the `HOST`, `USER`, and `PW` constants in the source code with your local MySQL credentials.
3.  **Compilation**:
    * Link the `include` and `lib` directories of your MySQL Connector to your C++ compiler.
    * Add `libmysql.lib` (Windows) or `-lmysqlclient` (Linux) to your linker settings.

## 📝 Future Enhancements
* **Security**: Implement **Prepared Statements** to mitigate SQL Injection risks.
* **Relational Mapping**: Expand the schema to include a `Passengers` table with Foreign Key relationships.
* **Concurrency**: Add **SQL Transactions** to handle multiple simultaneous booking requests.

---

### GitHub Tip:
Don't forget to add a **license** (like MIT) and perhaps a small screenshot of your console output to show the "Welcome To Airlines Reservation System" screen in action! 

Do you need help with the SQL commands to create the table?
