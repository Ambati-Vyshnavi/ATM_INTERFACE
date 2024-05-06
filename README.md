# ATM_INTERFACE
Developed an ATM interface using JAVA programming language. In which one can experience depositing , withdrawing , transfering and can view mini statement.
Simple Banking Transaction of a Person
----------------------------------------

Transactions that can be done:
View Transactions History
Withdraw Amount
Deposit Amount
Transfer



Project Structure
------------------

Interface: ATM_INTERFACE
public void viewTransactionsHistory();
public void withdraw(double amount);
public void deposit(double amount);
public void transfer(double amount,String recipientAccount);

Interface:UserAuthentication
boolean authenticateUser(int userId, int pin);

Class: Account implements ATM_INTERFACE
Variables: balance, transaction history
Constructor : public Account(double initialBalance) 
Methods:
{Overriding methods in  ATM_INTERFACE}

Class : ATM implements UserAuthentication 
Variables: account , userId,pin
Constructor : public ATM(Account account)
Methods:
{Overriding methods in  UserAuthentication}

Class: ATMTASK
Main method

Program Execution:
--------------------

Welcome to the ATM
Enter your user ID: 1234
Enter your PIN: 456

ATM Menu:
1. View Transactions History
2. Withdraw
3. Deposit
4. Transfer
5. Quit
Enter your choice: 3
Enter amount to deposit: 1000
Deposit successful. Current balance: $2000.0

ATM Menu:
1. View Transactions History
2. Withdraw
3. Deposit
4. Transfer
5. Quit
Enter your choice: 4
Enter amount to transfer: 500
Enter recipient account: 78965
Transfer successful. Current balance: $1500.0

ATM Menu:
1. View Transactions History
2. Withdraw
3. Deposit
4. Transfer
5. Quit
Enter your choice: 2
Enter amount to withdraw: 3000
Invalid amount or insufficient balance.

ATM Menu:
1. View Transactions History
2. Withdraw
3. Deposit
4. Transfer
5. Quit
Enter your choice: 2
Enter amount to withdraw: 1000
Withdrawal successful. Current balance: $500.0

ATM Menu:
1. View Transactions History
2. Withdraw
3. Deposit
4. Transfer
5. Quit
Enter your choice: 1
Transactions History:
Deposit: +$1000.0
Transfer to 78965: -$500.0
Withdrawal: -$1000.0

ATM Menu:
1. View Transactions History
2. Withdraw
3. Deposit
4. Transfer
5. Quit
Enter your choice: 5
Exiting ATM. Goodbye!
