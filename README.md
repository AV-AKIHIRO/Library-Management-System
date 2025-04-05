# 📚 Library Management System (LMS) – Terminal Application

The **Library Management System (LMS)** is a terminal-based application designed for efficient and secure management of a library's operations. It supports functionalities for managing users, books, and transactions. The system features a client-server architecture and is implemented in C using OS-level concepts such as multithreading and synchronization.

---

## 📁 Project Structure

The project is organized into the following directories:

- **`data/`** – Contains `.dat` files that store persistent data for users, books, and transactions.
- **`include/`** – Header files for the LMS source code.
- **`obj/`** – Stores compiled object (`.o`) files.
- **`src/`** – Contains the main C source files for both client and server.
- **`testing/`** – Contains unit tests and related code written using CUnit.

---

## ⚙️ Setup Instructions

Follow the steps below to build and run the LMS on your local machine:

1. **Clone or Fork the Repository**  
   Navigate to your desired folder and clone or fork the repository. Open the root directory in a terminal.

2. **Build the Project**  
   Compile the server and client programs:
   ```bash
   make server
   make client
   ```

3. **Start the Server and Client**  
   In one terminal, run the server:
   ```bash
   ./server
   ```
   In another terminal, run the client:
   ```bash
   ./client
   ```

4. **Login to the System**  
   Use the following credentials to log in as an administrator:
   ```
   Login as (admin/member): admin
   Enter username: admin_username
   Enter password: admin_password
   ```

5. **Use Admin Features**  
   Once logged in, the admin can:
   - Add new admins or members via the **"Add new user"** option
   - Manage book inventory
   - View and handle transactions

   Newly added users can then log in using their credentials to access appropriate features.

---

## 🧪 Testing Instructions

Unit tests are implemented using **CUnit**. To run the test suite:

1. **Install CUnit**  
   Refer to the installation guide in the `testing/README.md`.

2. **Compile the Test Suites**  
   Run the following command from the root directory:
   ```bash
   make -f Makefile_test test_users test_books test_transactions
   ```

3. **Execute the Tests**  
   Run each test binary individually:
   ```bash
   ./test_users
   ./test_books
   ./test_transactions
   ```

> ⚠️ **Note**: Running tests will reset the contents of data files to their base state. Be sure to back up any important data before testing.

---

## 👨‍💻 Team Members – Team 6

- **Areen Vaghasiya** (IMT2022048)  
- **Prateek Rath** (IMT2022017)  
- **Rudra Pathak** (IMT2022081)  
- **Kandarp Dave** (IMT2022115)