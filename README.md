# Python ATM Simulator

A clean, terminal-based ATM simulation program written in Python. It handles user authentication and standard banking operations like balance checks, deposits, and withdrawals with robust error handling.

---

## Features

* **PIN Verification:** Simulates security by giving the user a maximum of 3 login attempts.
* **Menu-Driven Interface:** Offers an interactive console menu supporting both numeric choices (e.g., `1`) and text commands (e.g., `check status`).
* **Input Validation:** * Rejects non-numeric PIN entries gracefully.
  * Prevents deposit or withdrawal of negative numbers or zero.
  * Blocks users from typing text into monetary fields.
  * Protects against account overdrafts.

---

## Default System Settings

The application initializes with these global configurations:

| Parameter | Value | Details |
| :--- | :--- | :--- |
| **Initial Balance** | $5000 | The baseline starting funds for transactions |
| **Default PIN** | `1234` | The passkey required to access the menu |
| **Max Attempts** | `3` | Number of retries allowed before account lockout |

---

## Supported Commands

Once logged in, the application accepts flexible inputs for its choices (case-insensitive):

* **Option 1:** Type `1` or `check status` to see current funds.
* **Option 2:** Type `2` or `deposit` to add money to the balance.
* **Option 3:** Type `3` or `withdraw` to pull money from the balance.
* **Option 4:** Type `4` or `exit` to safely close the session.

---

## How to Run the Script

1. Copy the code into a Python file on your computer (for example, name it `atm.py`).
2. Open your terminal or command prompt.
3. Move to the directory where you saved the file.
4. Run the script using the following command:

```bash
python atm.py
