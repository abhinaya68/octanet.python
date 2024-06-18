Overview
This Python script simulates a simple ATM console application with the following functionality:

Card insertion simulation
User authentication using a PIN
Balance check
Deposit money
Withdraw money
Classes and Methods

ATM Class
The ATM class encapsulates the ATM operations and user account details.

Attributes:

balance: Stores the current balance of the user's account.
pin: Stores the user's PIN for authentication.

Methods:

__init__(self, balance=0, pin=1234): Initializes the ATM with a starting balance and PIN.
check_balance(self): Returns the current account balance.
deposit(self, amount): Adds a specified amount to the balance, if the amount is positive.
withdraw(self, amount): Deducts a specified amount from the balance, if sufficient funds are available and the amount is positive.
authenticate(self, input_pin): Verifies if the entered PIN matches the stored PIN.
Main Function
The main function handles the overall workflow of the ATM system:

Welcome Message:

Prints a welcome message and prompts the user to "insert" their card by typing "insert".
Card Insertion Check:

If the user does not type "insert", the program exits with a message indicating no card was inserted.
ATM Initialization:

Initializes an ATM instance with a default balance of $1000 for demonstration purposes.
PIN Authentication:

Allows up to 3 attempts for the user to enter the correct 4-digit PIN.
If the correct PIN is entered, the user is presented with the ATM menu.
ATM Menu:

Displays options for checking the balance, depositing money, withdrawing money, or exiting the system.
Based on the user’s choice, performs the corresponding action:
Check Balance: Displays the current balance.
Deposit Money: Prompts the user to enter an amount to deposit and updates the balance.
Withdraw Money: Prompts the user to enter an amount to withdraw and updates the balance if sufficient funds are available.
Exit: Exits the ATM system.
Invalid Input Handling:

Handles invalid PIN entries, invalid menu choices, and invalid amount inputs gracefully by providing appropriate error messages and reprompting the user.
