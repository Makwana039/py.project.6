# py.project.6

📔 Journal Manager

A simple Python-based Journal Manager that allows users to create, view, search, and delete journal entries. Entries are stored permanently in a text file (journal.txt).

📌 Project Overview

The Journal Manager is a console-based application developed using Python OOP (Object-Oriented Programming).

It uses:

Classes and objects

File handling

Exception handling

datetime for timestamps

os for file checking

Menu-driven programming

✨ Features

Add a New Entry

Takes journal text from the user.

Prevents empty entries.

Automatically adds the current date and time.

Saves the entry in journal.txt.

View All Entries

Displays all saved journal entries.

Handles cases where the journal file does not exist.

Search for an Entry

Searches entries using a keyword.

Search is case-insensitive.

Displays matching lines.

Delete All Entries

Asks for confirmation before deletion.

Clears all entries from the journal file.

Exit

Safely exits the application.

🛠️ Technologies Used

Technology

Purpose

Python

Main programming language

os

Check whether the journal file exists

datetime

Generate timestamps

File Handling

Store and read journal entries

OOP

Organize the application using a class

Exception Handling

Handle file and permission errors

📂 Project Structure

Journal-Manager/
│
├── journal_manager.py
├── journal.txt
└── README.md

journal.txt is created automatically when the first journal entry is added.

▶️ How to Run

1. Install Python

Make sure Python 3.x is installed.

Check the Python version:

python --version

2. Save the Program

Save the Python code in a file such as:

journal_manager.py

3. Run the Program

Open the terminal in the project folder and run:

python journal_manager.py

📋 Main Menu

When the program starts, it displays:

========== JOURNAL MANAGER ==========
1. Add a New Entry
2. View All Entries
3. Search for an Entry
4. Delete All Entries
5. Exit
=====================================
Enter your choice:

📝 Example Usage

Add Entry

Enter your choice: 1

Enter your journal entry: Today I learned Python file handling.

Entry added successfully.

The entry is stored approximately like this:

[2026-09-21-21:30:15]
Today I learned Python file handling.
----------------------------------------

View Entries

Enter your choice: 2

-----All Journal Entries-----
[2026-09-21-21:30:15]
Today I learned Python file handling.
----------------------------------------

Search Entry

Enter your choice: 3
Enter keyword to search: Python

----- SEARCH RESULTS -----
Today I learned Python file handling.

Delete All Entries

Enter your choice: 4
Are you sure you want to delete all entries? (yes/no): yes

All journal entries deleted successfully!

🧠 OOP Concepts Used

1. Class

The program uses a class named journalManager to organize journal operations.

class journalManager:

2. Constructor

The __init__() method initializes the journal filename.

def __init__(self, filename="journal.txt"):
    self.filename = filename

3. Object

An object of the class is created using:

journal = journalManager()

4. Methods

Different methods perform different tasks:

add_entry()
view_entries()
search_entry()
delete_all_entries()
menu()

📁 File Handling

The project uses different file modes:

Append Mode

open(self.filename, "a")

Used to add new entries without deleting previous entries.

Read Mode

open(self.filename, "r")

Used to read existing journal entries.

Write Mode

open(self.filename, "w")

Used to clear all journal entries.

⚠️ Exception Handling

The program handles common file-related errors:

except FileNotFoundError:

except PermissionError:

except OSError as e:

This prevents the program from crashing when common file errors occur.

🕒 Timestamp

Every journal entry receives a timestamp using:

datetime.now().strftime("%Y-%m-%d-%H:%M:%S")

Example:

[2026-09-21-21:30:15]

🎯 Learning Objectives

By completing this project, you can practice:

Python classes and objects

Methods and constructors

File handling

Reading and writing text files

Exception handling

try-except

datetime

os.path.exists()

String methods

Loops and conditions

Menu-driven applications

🚀 Possible Future Improvements

The project can be extended with:

Edit an existing journal entry

Delete a single entry

Search by date

Display entries by date

Add categories or tags

Use JSON or SQLite instead of a text file

Add a graphical user interface (GUI)

Add password protection

Export journal entries to PDF

👨‍💻 Author

Python Journal Manager Project

Built as a practice project for learning Python, OOP, File Handling, and Exception Handling.
