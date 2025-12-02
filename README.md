# 💸📊PERSONAL EXPENSES TRACKER 
---

# 📝OVERVIEW
<small>
Personal Expenses Tracker is console-based program that allows the user to track, manage, and categorize their daily expenses. It is designed to make monitoring and spending simple and efficient by recording different types of expenses such as food, transportation, bills, and etc.
</small>

---

# 🧩OOP Concepts Applied
---
## 🛡️ ENCAPSULATION 
Encapsulation is applied in the Expenses class where it has four variables such as date, category, description and amount and declared it as private. This will prevent them from being accessed directly from outside the class and it will only can be accessed through the use of constructor. Also, it has getters methods which give controlled visibility to the values  when viewing the expenses.

---

## 🧬INHERITANCE 
Inheritance is applied to the most common expenses such as food, transportation, and bills by creating them as subclasses of the Expenses class. These subclasses inherit the properties of the parent class, which means they automatically receive the attributes and behavior of Expenses without rewriting them. Each subclass only sets its own category by calling super() in its constructor. For example, if the user inputs “Food” as the category, the program creates a Foodexpense object, and its behavior and data structure come from the parent Expenses class.

---

## 🎭 POLYMORPHISM
Polymorphism is applied in the program by allowing the Expenses parent type to store different subclass objects such as food, transport, and bills. Even though these objects come from different subclasses, polymorphism lets them be treated as one group while still keeping their own categories and behaviors. It is also shown through the ExpenseViewer interface, where the viewer is declared using the interface type but can use any class that implements it, allowing the same view() method to work differently depending on the specific viewer class.

---

## ⚙️ ABSTRACTION
Abstraction is applied on ExpenseViewer interface, which defines the view() method without showing how it works, and in AddExpense, where adding a new expense is grouped into one method, hiding the internal steps from the main program.

---

# 📁 Project Structure
---
**`Main.java`** - Entry point of the program. It displays the menu, handles user input, and connects all the features such as adding, viewing, totaling, and filtering expenses.

**`Expenses.java`** - Represents a single expense record. It stores four private variables (date, category, description, amount), enforcing encapsulation. It also provides getters so the data can be safely accessed when viewing expenses.

**`FoodExpense.java / TransportExpense.java / BillsExpense.java`** -Subclasses of Expenses that automatically set their own category through super(). They inherit the parent class’s properties, allowing the program to create specialized expense objects based on user input.

**`AddExpense.java`** - Handles the entire process of adding a new expense. It collects user input, validates the amount, creates the correct expense object (using the category), and stores it in the expenses array.

**`ExpenseViewer.java`** - Defines the method view() without showing how it works. This applies abstraction by letting the viewer behavior be implemented differently by any class.

**`ConsoleExpenseViewer.java`**- Implements the ExpenseViewer interface. Formats and displays all expenses in a table-like layout. 

**`ExpenseUtils.java`**- A helper class that contains useful methods for working with expenses. It computes the total amount of all expenses and can filter the list based on a specific category. This keeps the code cleaner since these functions are placed in one utility file.

---
# 🚀HOW TO RUN THE PROGRAM 
---
1. 📂Open the `src` folder in VS Code.
2. 🖥️Open a new terminal.
3. 🛠️Compile the program:
   ```sh
   javac *.java
4. ▶️Run the program:
   ```sh
   java Main
   
---
# 🖥️SAMPLE OUTPUT
---
### 🏠 MAIN MENU
<img width="276" height="179" alt="main-menu" src="https://github.com/user-attachments/assets/e899fbc0-3c3e-43ca-84fc-1e9a0a86db8a" />

### ➕ ADD EXPENSES
<img width="188" height="157" alt="add-expenses" src="https://github.com/user-attachments/assets/4c43f425-5e90-4e94-84c4-76c4a5aba362" />

### 📄 VIEW EXPENSES
<img width="495" height="144" alt="view-expenses" src="https://github.com/user-attachments/assets/c0ed2144-97fb-4cc3-a367-1fb83d60309d" />

### 💰 TOTAL EXPENSES
<img width="269" height="197" alt="image" src="https://github.com/user-attachments/assets/8b859bac-ad71-4461-a9b8-e5f9f8d8b982" />


### 🔍 FILTER BY CATEGORY
  <img width="497" height="158" alt="image" src="https://github.com/user-attachments/assets/734bc259-d215-46d3-a4a6-be0cbf1e52da" />


---
# 🙏 ACKNOWLEDGEMENT
---
I would like to express my gratitude to our instructor for the guidance and support provided throughout this project. I also want to thank my group members for their cooperation, ideas, and contributions that helped make this work successful. Their teamwork and dedication played a big role in completing this project effectively.

---

# 🔧 FUTURE ENHANCEMENTS
---
To further improve this project, the following enhancements are planned:

### 1. Add a Graphical User Interface (GUI)
This will make the application more user-friendly and easier to navigate.

### 2. Add Additional Features
   - 🎯 **Set Budget**
   - 🗓️ **Monthly summary report**
   - 🔎 **Search bar**
   - 🔁 **Add recurring expenses** (e.g., daily/weekly/monthly)




