# 🏧 ATM System (C++)

A console-based ATM application written in C++. It uses the same text-file database (`Clients.txt`) as my [Bank Management System](https://github.com/hail-yasin/Bank-Management-System-CPP), so clients created there can log in and make transactions here.

## ✨ Features

- 🔐 Login with account number and PIN code
- ⚡ Quick withdraw with preset amounts (20, 50, 100, 200, 400, 600, 800, 1000)
- 💸 Normal withdraw (amount must be a multiple of 5)
- 💰 Deposit (positive amounts only)
- 📊 Check balance
- ✅ Confirmation before every transaction
- ⛔ Withdrawals above the balance are rejected
- 🚪 Logout returns to the login screen

## 🔗 Shared Data with the Bank System

Both projects read and write the same file, which acts as a simple database:

`Clients.txt`

AccountNumber#//#PinCode#//#ClientName#//#Phone#//#Balance

The ATM reads `Clients.txt` from its working directory. To use the real data of the Bank Management System, run the ATM from the same folder as that project's `Clients.txt` (or copy the file next to the ATM).

## 🧪 Sample Accounts

| Account Number | PIN  | Balance |
|----------------|------|---------|
| A101           | 1111 | 1500    |
| A102           | 2222 | 3000    |

These are demonstration accounts only.

## 🛠️ Technologies Used

- C++
- Structs and Enums
- Functions
- Vectors
- File Handling
- Console Application

## 📁 Project Structure

- C++ source file
- Visual Studio solution and project files
- `Clients.txt` (sample data)
- `README.md`

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/hail-yasin/ATM-System-CPP.git
   ```
2. Open the `.sln` file in Visual Studio.
3. Build and run the project. Make sure `Clients.txt` is in the working directory.
4. Log in with a sample account, for example:
Account Number: A101
PIN: 1111

## ⚠️ Requirements and Limitations

- Windows only (uses `conio.h` and `system("cls")`).
- PIN codes are stored as plain text, which is not secure. This is a learning project.
- There is no limit on failed login attempts.
- The whole file is rewritten on every transaction, so do not run the ATM and the Bank System at the same time.

## 📚 What I Learned

- Sharing a text-file database between two programs
- Reading, updating and saving records with `fstream`
- Validating user input
- Structuring a console application with menus and reusable functions

## 👨‍💻 Author

**Hail Yasin**

GitHub:
https://github.com/hail-yasin
