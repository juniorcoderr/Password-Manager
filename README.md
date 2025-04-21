## 🔐 Password Manager using Python & Tkinter

This is a simple yet functional **Password Manager** built with **Python** using the **Tkinter GUI library**. The application allows you to **generate secure passwords**, **copy them to your clipboard**, and **store them locally** in a text file along with the associated **website** and **email/username**.

---

### 📌 Features

- ✅ GUI built using **Tkinter**
- 🔐 Secure **random password generation** using letters, numbers, and symbols
- 📋 **Clipboard support** to auto-copy generated passwords (via `pyperclip`)
- 💾 Passwords and credentials are saved in a local `.txt` file
- 🛑 Input validation with alerts for empty fields
- ✅ Confirmation dialog before saving credentials

---

### 🧠 Concepts & Technologies Used

#### 1. **Python Standard Libraries**
- **`random`**: Used for generating random letters, numbers, and symbols for passwords.
  - Functions like `choice()` and `randint()` are used to ensure random and secure password creation.
  - The `shuffle()` function is used to randomize the final password string.
  
- **`tkinter`**: Python's standard GUI toolkit.
  - `Tk()`: Initializes the main application window.
  - `Label`, `Entry`, `Button`, and `Canvas` widgets: Used for building the user interface.
  - `messagebox`: Used to display alerts and confirmation dialogs.
  
#### 2. **`pyperclip` Module**
- Used to **automatically copy the generated password** to the system clipboard so users can directly paste it when needed.
- Enhances usability and reduces the need to manually select and copy text.

#### 3. **File Handling**
- Saves website, email, and password in a file called `data.txt`.
- Uses Python's built-in `with open(...) as file:` syntax for safe file writing (ensures file is properly closed after writing).

#### 4. **Input Validation**
- Checks for empty website or password fields before saving using basic `if len(...) == 0` conditions.
- Displays error messages using `messagebox.showinfo()` to ensure the user fills in all necessary fields.

#### 5. **GUI Layout Management**
- Uses `grid()` layout manager to place widgets in a clean, structured format.
- Widgets are configured with `sticky`, `pady`, and `columnspan` to improve alignment and spacing.

---

### 📂 Project Structure

```
password-manager/
│
├── logo.png               # Logo displayed in the UI
├── data.txt               # File to store website/email/password data
└── main.py                # The main script with all functionality
```

---

### 🛠 How to Run

1. Make sure you have Python installed.
2. Install the required module:
   ```bash
   pip install pyperclip
   ```
3. Run the application:
   ```bash
   python main.py
   ```
4. Add a `logo.png` image in the same directory for the app to show a logo in the top section.

---

### 📌 Future Improvements (Optional Ideas)
- Encrypt stored passwords for added security.
- Add search functionality to find saved credentials.
- Integrate with a database (e.g., SQLite) instead of a `.txt` file.
- Build login authentication for accessing the app.

---

### 🙌 Acknowledgements

This project is inspired by basic password managers and is a great starting point for beginners looking to understand:
- GUI development
- Random password generation
- File handling in Python
