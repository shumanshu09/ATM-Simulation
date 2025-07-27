ATM System in C (with PIN & Transaction History)

Project Description:

This is a console-based ATM simulation in C that allows:

* PIN generation and validation
* Balance inquiry
* Deposit & withdrawal operations
* Storing the **last 10 transactions** using a queue (linked list)

 Features:

1. PIN Generation:

    Random 4-digit PIN saved to `pin.txt`
2. PIN Validation:

  Verifies user-entered PIN against saved PINs
3. ATM Menu:

   * Check Balance
   * Deposit Money
   * Withdraw Money
   * View Transaction History
   * Exit
4. Transaction History:

   Queue stores the last 10 deposit/withdrawal messages

Files Created:

* `pin.txt` → stores generated PINs
* All transaction history is stored in memory (not in file)


Data Structures Used:

* Linked List Queue: Used to store transaction messages (FIFO)
* Each node contains a transaction statement (e.g., "Rs.500 deposited")

Sample Usage:

1. Run program → Choose `1` to generate a PIN
2. Re-run → Choose `2` and enter the PIN to access ATM menu
3. Perform transactions and view history
4. Program exits on `Quit` selection

How Transactions Are Stored:

* The queue stores only 10 recent transactions
* On the 11th transaction, the oldest one is removed (FIFO behavior)

