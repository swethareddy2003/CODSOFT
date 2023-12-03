# CODSOFT
ATM INTERFACE
Here is an explanation of the code:

BankAccount Class:

Represents a bank account with a balance.
Constructor initializes the account with an initial balance.
getBalance() method returns the current balance.
deposit(double amount) method deposits money into the account.
withdraw(double amount) method withdraws money from the account.
ATM Class:

Represents an ATM that operates on a BankAccount.
Constructor takes a BankAccount as a parameter.
displayMenu() method prints the menu options.
performTransaction(int choice, Scanner scanner) method performs the selected transaction based on user input.
ATM_Interface Class (Main):

Takes initial balance as user input.
Creates a BankAccount object with the provided initial balance.
Creates an ATM object using the BankAccount.
Enters into an infinite loop to display the ATM menu and perform transactions until the user chooses to exit.
The main loop repeatedly displays the menu, takes the user's choice, and performs the corresponding transaction until the user chooses to exit (option 4).

Note: It's a good practice to close the Scanner object when you're done using it. However, in this case, calling scanner.close() inside the loop will also close the underlying System.in, making it impossible to read input again. It's better to close the Scanner when you're done with all input operations.

Additionally, the use of an infinite loop (while(true)) and System.exit(0) for program termination may be reconsidered. You might want to provide a more user-friendly way to exit the program, such as adding an explicit exit option in the menu and breaking out of the loop when the user chooses to exit.






