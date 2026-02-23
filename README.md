# BankAccountThingy

**BankAccountThingy** is a Java Swing desktop application designed to manage bank accounts efficiently. It allows users to create and manage multiple "Banks" (stored as CSV files), add accounts, perform transactions like deposits and withdrawals, and track activities through a logging system.

## Features

*   **Bank Management**:
    *   Create new Bank lists (saved as `.csv` files).
    *   Open existing Bank lists.
    *   Secure serial UID system for bank file validation.
*   **Account Management**:
    *   Add new bank accounts with personal details (First, Middle, Last Name).
    *   Auto-generate valid credit card numbers using Luhn's algorithm.
    *   Add profile pictures to accounts.
    *   Edit account details.
    *   Delete accounts.
*   **Transactions**:
    *   **Deposit**: Add funds to an account, with an option to apply an interest rate.
    *   **Withdraw**: Remove funds from an account.
*   **Search & Sort**:
    *   Hybrid search functionality (Search by Name or Account Number).
    *   Sort accounts by First Name, Middle Name, Last Name, or Account Number (Ascending/Descending).
*   **Logging**:
    *   Automatic logging of all activities (Open/Close App, Transactions, Account changes) to `logger.csv`.
*   **UI/UX**:
    *   Custom Swing components.
    *   Draggable undecorated windows.
    *   Dynamic image processing for profile pictures.

## Getting Started

### Prerequisites
*   Java Development Kit (JDK) 8 or higher.

### Running the Application
1.  Clone the repository.
2.  Open the project in your IDE (IntelliJ IDEA recommended).
3.  Run the `InitialFrame.java` class located in `src/BankAccountThingy/InitialFrame.java`.

## Usage

1.  **Launch the App**: You will be greeted with a welcome screen.
2.  **Create/Open Bank**:
    *   Click **+ New Bank** to create a new CSV database.
    *   Click **o Open** to load an existing CSV database.
3.  **Manage Accounts**:
    *   Once a bank is loaded, use the **+ Add** button to create a new account.
    *   Click on specific account actions (Deposit, Withdraw, Edit, Delete) within the list view.
4.  **Search**: Use the search bar at the top to filter accounts.
5.  **Sort**: Use the dropdown menu to sort the list.

## Project Structure

The project is organized into the following packages:

*   `BankAccountThingy`: Contains the main entry point `InitialFrame`.
*   `BankAccountThingy.pp2.BankAccount`: Core logic for `BankAccount2` and list management.
*   `BankAccountThingy.pp2.BankAccount.Dialogs`: JDialog classes for user input (Add Bank, Deposit, etc.).
*   `BankAccountThingy.pp2.BankAccount.StreamIO`: Handles File I/O (CSV reading/writing, Image processing, Logging).
*   `BankAccountThingy.pp2.BankAccount.Utils`: Utility classes, Enums, and Custom Annotations (`@Intention`, `@Region`).

## Technical Highlights

*   **Data Persistence**: Uses CSV files for storing bank data, making it portable and human-readable.
*   **Custom Annotations**: Uses `@Intention` and `@Region` for code documentation and structure.
*   **Swing Customization**: Custom painting for images and undecorated frames for a modern look.

---
*Note: This project is for educational purposes.*
