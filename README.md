# Inventory-Management-System-JSON
Here's a README.md file you can use for this inventory management system:
markdown
# Inventory Management System (Python)

This is a simple Python-based inventory and billing system that helps manage product sales using a JSON file to store inventory records and a text file to log sales. It is designed for basic command-line use.


##  Features

- Load and display product inventory from a JSON file
- Accept customer purchase details
- Check product availability
- Generate a bill with customer and purchase information
- Update inventory automatically after purchase
- Handle insufficient stock scenarios
- Log all sales in a text file with timestamp
  


##  File Structure

- `Records.json`: JSON file that contains the inventory data.
- `Mysales.txt`: Text file that logs each sale with user and purchase details.
- `inventory_system.py`: The main Python script for handling purchases.



##  Sample `Records.json` Structure

json
{
  "1001": {"Name": "Pen", "Price": 10, "Qn": 100},
  "1002": {"Name": "Notebook", "Price": 40, "Qn": 50},
  "1003": {"Name": "Pencil", "Price": 5, "Qn": 150}
}


Each product is stored with:
- `Name`: Product name
- `Price`: Price per unit
- `Qn`: Quantity available

---

##  How to Run

1. Ensure Python is installed on your system.
2. Make sure `Records.json` is present in the same directory as the script.
3. Open terminal or command prompt.
4. Run the script using:

bash
python inventory_system.py


5. Follow the prompts to:
   - Enter your name, email, and phone number
   - Enter the product ID and quantity you want to purchase

---

## Output

- If enough quantity is available:
  - A bill is printed
  - Inventory is updated
  - Sale is recorded in `Mysales.txt`
  
- If quantity is insufficient:
  - User is informed about available quantity
  - Given an option to purchase remaining stock

---

##  Notes

- Invalid product IDs will result in an error (suggested improvement: add input validation).
- Only works in a single-user terminal environment.
- For more advanced functionality (e.g., GUI, database integration), consider upgrading to frameworks like Tkinter or Flask.

---

##  License

This project is open-source and free to use for educational and personal projects.


