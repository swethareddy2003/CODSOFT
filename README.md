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









NumberGame
Here is explanation for code of NumberGame

Certainly! The provided Java code is a simple console-based number guessing game. Here's a description of how the code works:

Welcome and Setup:

The program starts by welcoming the player and informing them about the number of chances they have to guess the correct number (8 chances in this case).
The finals variable is used to keep track of the number of successful guesses.
Game Loop:

The program enters a loop (while (playAgain)) that allows the player to play the game multiple times if they choose to play again.
Inside the loop, a random number (rand) between 1 and 100 (inclusive) is generated using the getRandNum method.
Another loop (for (int i = 0; i < chances; i++)) is used to give the player multiple chances to guess the correct number.
User Input and Comparison:

The program prompts the user to enter their guess for the current chance.
The user's guess is compared with the randomly generated number (rand).
If the guess is correct, the guess variable is set to true, the finals count is incremented, and a message is displayed indicating a win. The loop is then exited with break.
If the guess is too high or too low, corresponding messages are displayed.
Game Outcome:

If the player exhausts all chances without a correct guess (!guess), a message is displayed, indicating that the player lost and revealing the correct number.
The player is then asked if they want to play again.
End of Game:

The game loop continues until the player decides not to play again (playAgain set to false).
After exiting the loop, a closing message is displayed, along with the player's final score (number of successful guesses).
Random Number Generator:

The getRandNum method generates a random integer within a specified range (inclusive).
Overall, the code provides a simple and interactive number guessing game where the player has multiple chances to guess a randomly generated number, and the program keeps track of their score.









