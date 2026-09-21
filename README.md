📔 Personal Journal Manager

A simple Python console-based application for managing personal journal entries.

The program allows users to add, view, search, and delete journal entries. Entries are stored in a text file with the date and time.

✨ Features
Add a new journal entry
View all journal entries
Search entries using a keyword
Delete all journal entries
Automatic date and time
File error handling
Menu-driven interface

🛠️ Requirements
Python 3.x
No external libraries required
Built-in Modules
import os
from datetime import datetime

📂 Project Structure
Personal-Journal-Manager/
│
├── journal_manager.py
├── journal.txt
└── README.md

journal.txt is created automatically when the first entry is added.

▶️ How to Run
1. Check Python
python --version
2. Run the program
python journal_manager.py

🖥️ Sample Output
=====================================
     WELCOME TO PERSONAL JOURNAL
=====================================
1. Add a New Entry
2. View All Entries
3. Search for an Entry
4. Delete All Entries
5. Exit
=====================================
Enter your choice: 1

Enter your journal entry: Today I learned Python.

Entry added successfully!
View Entries
Enter your choice: 2

----- ALL JOURNAL ENTRIES -----

[2026-09-21 21:57:30]
Today I learned Python.
----------------------------------------
Search Entry
Enter your choice: 3

Enter keyword to search: Python

----- SEARCH RESULTS -----
Today I learned Python.
Exit
Enter your choice: 5

Thank you for using Journal Manager!

🧠 Concepts Used
Object-Oriented Programming (OOP)
Classes and Objects
Constructor (__init__)
Methods
File Handling
try-except Exception Handling
os module
datetime module
String Operations
if-elif-else
while loop
Menu-driven programming

📌 Main Methods
Method	Purpose
add_entry()	Add a new journal entry
view_entries()	View all entries
search_entry()	Search for an entry
delete_all_entries()	Delete all entries
menu()	Display the main menu
🎯 Project Goal

The main goal of this project is to practice Python OOP, file handling, exception handling, and menu-driven programming.
