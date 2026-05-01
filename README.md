# 🔐 Rail Fence Cipher – MIPS Assembly Project

# Author

Renad Amr

# Overview

This project implements an interactive **encryption and decryption utility** using the **Rail Fence Cipher** in **MIPS Assembly Language**.
The program runs on the **QTSPIM simulator** and allows users to input a message and a numeric key (number of rails) to perform encryption. It also provides an option to decrypt the generated ciphertext, demonstrating both forward and reverse cipher operations.

# Key Features

* Interactive console-based program (QTSPIM)
* Supports encryption of:

  * Uppercase and lowercase letters
  * Numbers
  * Spaces and special characters
* Input validation for encryption key
* Optional decryption of generated ciphertext
* Continuous execution loop until user chooses to exit

# Program Workflow

##1. User Prompt

* User is asked whether to start the program

  * **Yes** → Proceed to input
  * **No** → Exit program gracefully


### 2. Key Input & Validation

* User enters the number of rails
* The program ensures:

  * Key ≥ 2
* If invalid, an error message is displayed and the user is prompted again


### 3. Plaintext Input & Encryption

* User enters a message (any characters allowed)
* The program encrypts the message using the Rail Fence Cipher:

  * Characters are arranged in a **zigzag pattern** across rails
  * Movement follows a **downward then upward diagonal pattern**
  * Ciphertext is produced by reading rows sequentially


### 4. Optional Decryption

* User is asked whether to decrypt the ciphertext

  * **Yes** → The program reconstructs the zigzag pattern and retrieves the original plaintext
  * **No** → Skip this step


### 5. Output

* Display original plaintext
* Display generated ciphertext
* Display decrypted text (if selected)

### 6. Loop Control

* After execution, the program prompts the user to repeat
* Continues running until the user chooses to exit

# Technologies Used

* **MIPS Assembly Language**
* **QTSPIM Simulator**


# How to Run

1. Open **QTSPIM**
2. Load the `.asm` file
3. Run the program
4. Follow on-screen prompts in the console

# Highlights

* Demonstrates low-level programming using MIPS Assembly
* Implements both encryption and decryption logic
* Handles user input validation and control flow
* Simulates a real-world cryptographic technique

