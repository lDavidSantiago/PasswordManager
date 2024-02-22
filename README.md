# Python Password Manager

This project is a simple password manager written in Python, a high-level, interpreted programming language known for its readability and simplicity.

## Structure

The project uses a procedural programming paradigm, where the code is organized into procedures or routines (in this case, functions) that can be invoked as needed.

## Main Functions

- `register`: This function is used to register a new user. It takes a username and a master password as input, and stores them in a JSON file called `user_data.json`. The master password is hashed before it is stored for security reasons.

- `login`: This function is used to log in an existing user. It takes a username and a master password as input, hashes the master password, and compares it to the hashed password stored in `user_data.json`. If the hashed passwords match, the user is logged in.

## Modules Used

The project also uses the `os` and `sys` modules for interacting with the system, and the `getpass` module for securely handling password inputs. The `os.path.exists` and `os.path.getsize` functions are used to check if the `user_data.json` file exists and if it is not empty, respectively.

## Program Flow

The main loop of the program asks the user to either register or log in, and calls the appropriate function based on the user's choice. If the user chooses to log in but has not registered yet, the program prints an error message and exits.
