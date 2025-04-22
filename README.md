## 🔐 Password Manager using Python & Tkinter

A secure and beginner-friendly **Password Manager** built with **Python** and **Tkinter**, featuring **password generation**, **local data storage using JSON**, **clipboard support**, and **search functionality** for quick access to saved credentials.

---

### 📌 Features

- ✅ Clean and responsive **GUI** built with Tkinter
- 🔐 **Secure password generator** using letters, numbers, and symbols
- 📋 Auto-copies generated passwords to clipboard (via `pyperclip`)
- 💾 Stores credentials in a structured `data.json` file (instead of plain `.txt`)
- 🔍 **Search functionality** to quickly retrieve saved credentials
- 🛑 Input validation with alerts for empty fields
- ✅ Confirmation dialogs before saving data
- 🔄 Updates existing credentials if the website already exists

---

### 🧠 Concepts & Technologies Used

#### 🐍 **Python Standard Libraries**
- `random`: For generating secure, random passwords
- `json`: For storing and updating data in JSON format
- `tkinter`: For building the user interface
- `messagebox`: For showing alerts and confirmation messages

#### 📋 **pyperclip**
- Copies generated passwords directly to the clipboard
- Improves ease-of-use and saves time

#### 💾 **JSON File Handling**
- Securely saves website, email, and password data in `data.json`
- Uses `with open(...)` for safe file operations
- Updates existing entries seamlessly

#### ✅ **Validation & Error Handling**
- Prompts user if any required field is empty
- Notifies user if a website record is not found
- Gracefully handles missing `data.json` file

#### 🧱 **Tkinter UI & Layout**
- Utilizes `grid()` for clean layout
- Includes `Entry`, `Label`, `Button`, `Canvas`, and `PhotoImage` widgets
- Integrates a logo using `logo.png` for a polished look

---

### 📂 Project Structure

```
password-manager/
│
├── logo.png               # Logo displayed in the UI
├── data.json              # JSON file to store credentials securely
└── main.py                # Main application script
```

---

### 🛠 How to Run

1. Make sure Python is installed.
2. Install required package:
   ```bash
   pip install pyperclip
   ```
3. Place a `logo.png` image in the same directory.
4. Run the application:
   ```bash
   python main.py
   ```

---

### 🚀 Possible Future Enhancements

- 🔐 Encrypt saved credentials for enhanced security
- 🔍 Advanced search and filtering options
- 📦 Migrate storage to SQLite or another database
- 🔓 Add authentication before accessing the app

---

### 🙌 Acknowledgements

This project is a great starting point for Python beginners exploring:
- GUI development with Tkinter  
- Random password generation  
- JSON-based data persistence  
- Clipboard integration  
- Basic error handling & validation
