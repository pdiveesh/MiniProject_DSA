

# SDN Bank Management System

Welcome to **SDN Bank** — a simple command-line application that demonstrates **CRUD operations** for bank account management using C.

This project helps you understand fundamental data structures (like linked lists) while implementing practical banking features.

## 🚀 Features

- **Create Account**  
  Store customer details like name, Aadhar number, PAN card number, and initial deposit amount.

- **View Balance**  
  Check account balance by entering the account number.

- **Deposit Amount**  
  Add funds to your account with a simple deposit option.

- **Withdraw Amount**  
  Withdraw money, with validation to prevent overdrafts.

- **Exit**  
  Safely close the application.

## 🛠️ How It Works

The system maintains a linked list of accounts, where each node stores account details. Operations like creation, search, and balance updates traverse this list.

## 📂 CRUD Operations

Here’s a quick breakdown of the CRUD actions:

### 1. 🟢 Create Account (C in CRUD)

```
1. Create Account
```

- Enter your **name**, **initial deposit**, **Aadhar number**, and **PAN card number**.
- The system generates a unique account number.
- A success message shows your newly created account number.

### 2. 🟡 View Balance (R in CRUD)

```
2. View Balance
```

- Enter your account number to view the **account holder's name** and **current balance**.
- If the account doesn’t exist, you'll get an **Account not found** message.

### 3. 🟠 Deposit Amount (U in CRUD)

```
3. Deposit Amount
```

- Enter your **account number** and **deposit amount**.
- The system updates the balance and confirms the deposit.

### 4. 🔴 Withdraw Amount (U in CRUD)

```
4. Withdraw Amount
```

- Enter your **account number** and **withdrawal amount**.
- If you have sufficient funds, the amount is debited, and the updated balance is shown.
- If not, you’ll see an **Insufficient balance** warning.

### 5. 🏁 Exit

```
5. Exit
```

- Gracefully terminate the program.

## 🏃‍♀️ Usage

1. **Compile the Code**:

```bash
gcc bank_management.c -o bank_management
```

2. **Run the Program**:

```bash
./bank_management
```

3. **Follow the On-Screen Menu** to interact with the system!

## ⚠️ Important Notes

- **Data Persistence:** Currently, account data is stored in memory (linked list). Data is lost when the program is terminated.
- **Input Validation:** Basic validation is done (e.g., insufficient funds for withdrawal). However, you can improve the program by handling edge cases like negative amounts.

## 📘 Example Flow

```
Welcome to SDN Bank!!

How may I help you?
 1. Create Account
 2. View Balance
 3. Deposit Amount
 4. Withdraw Amount
 5. Exit

Enter your choice: 1

Enter Account Holder Name: Alice  
Enter Initial Deposit Amount: 5000  
Enter Aadhar Card Number: 123456789012  
Enter Pan Card Number: ABCDE1234F  

Account Creation Successful! Your Account Number: 1

Enter your choice: 3

Enter account number: 1  
Enter deposit amount: 1500  

Deposit successful! Current balance: 6500

Enter your choice: 4

Enter account number: 1  
Enter withdrawal amount: 2000  

Withdrawal successful! Current balance: 4500
```

## 💡 Future Enhancements

- **File I/O for Persistence:** Save and load account data from a file.
- **Account Deletion (D in CRUD):** Add an option to close/delete an account.
- **Error Handling & Validation:** Handle invalid inputs (like negative deposits) more gracefully.

