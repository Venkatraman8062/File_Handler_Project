File Handler CLI App 🔢

A command-line interface (CLI) based application designed to manage product-related data using CRUD operations (Create, Read, Update, Delete). Built entirely in Python, this app allows persistent management of product files organized in a structured directory format. Ideal for inventory or catalog systems where offline file handling is essential.

🌐 Overview

Goal: Provide an interactive and user-friendly CLI to manage product details and sales information, with file-based storage and persistence.

Functionalities:

Create new product records

Read and search product/sales data

Update existing product records

Delete product entries

Save and exit

Data is stored in:

product_details.csv

sales_data.csv

product_descriptions.txt

📚 Folder Structure

main_folder/
├── product_details.csv
├── sales_data.csv
├── product_descriptions.txt

⚖️ Features

🛠️ Modular Functionality

user_menu(main_folder_path): Central controller for CLI interaction

load_data(): Loads all existing files into memory safely

create(), read(), update(), delete(): Operate directly on loaded data structures

🔄 Data Persistence

Saves the state of all files before exiting using structured write-back logic

Ensures consistency across all files during CRUD operations

⚠️ Robust Input Validation

Prevents invalid menu selections

Prompts user again until a valid choice is made

🔧 Error Handling & UX

Clear messages for invalid input, file issues, or empty data

Graceful exit with confirmation and file saving

📄 How to Run

# Clone this repo and move into the directory
git clone https://github.com/yourusername/file-handler-app.git
cd file-handler-app

# Run the Python script with the main folder path as an argument
python main.py /path/to/main_folder

🔹 Example CLI Flow

============================
 Welcome to File Handler
============================
1. Create a new product
2. Read product details
3. Update a product
4. Delete a product
5. Exit

Enter your choice: 2
--> Displaying all product records...

📊 Future Enhancements

Add backup versioning of old data

Integrate search by product category or tags

Add JSON export/import option

Extend support to connect with SQLite for hybrid storage

✨ Author

Venkatraman Svenkatraman8062@gmail.com

This project was developed as part of a practical coding exercise to manage offline product data with reliability and scalability in mind.
