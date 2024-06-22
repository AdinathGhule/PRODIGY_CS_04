# 🖥️ Simple Keylogger
Internship Task_04 at Prodigy InfoTech

## 📜 Overview
This program creates a basic keylogger using Python. The keylogger records and logs keystrokes, and you can start logging, stop logging, and save the log to a file.
**Note:** Always consider ethics and get permission when working with keyloggers.

## 📚 What is Keylogging?

### 🔐 Keylogging
Keylogging records the keys pressed on a keyboard, usually without the user knowing. It can be used for good purposes, like monitoring employees, or bad purposes, like stealing information.

### 🛡️ Cybersecurity Concepts
- **Ethical Use:** Use keyloggers only with permission and for good reasons.
- **Privacy Concerns:** Logging keystrokes without permission can invade privacy and is illegal in many places.
- **Data Security:** Keep the logged data safe and only allow authorized people to access it.

## 📝 Prerequisites
- Basic Python programming knowledge.
- Familiarity with creating GUIs using Tkinter.
- Understanding of threading and handling keyboard events.

## 💻 Software Requirements
- Python 3.x
- Libraries: `pynput`, `tkinter`

## 🖥️ Hardware Requirements
- A computer with at least 2GB of RAM.
- Any operating system that supports Python 3.x.

## 🛠️ Tech Stack
- **Programming Language:** Python
- **Libraries:** Tkinter, Pynput, Threading

## 🚀 How to Run the Program

1. **Clone the Repository:**
   ```bash
   git clone <repository-directory> (https://github.com/trupti-K-ghenand/PRODIGY_CS_04)
   cd <repository-directory>
   ```

2. **Install the Required Libraries:**
   ```bash
   pip install pynput
   ```

3. **Run the Program:**
   ```bash
   python task4_keylogger.py
   ```

4. **Usage Instructions:**
   - Click "Start Logging" to begin capturing keystrokes.
   - Click "Stop Logging" to stop capturing keystrokes.
   - Click "Save Log" to save the captured keystrokes to a text file.

## 📄 Code Details Overview

### `task4_keylogger.py`

#### Imports
```python
import tkinter as tk
from tkinter import filedialog, messagebox
from pynput import keyboard
import threading
```
- `tkinter`: For creating the GUI application.
- `pynput`: For capturing keyboard inputs.
- `threading`: For running keylogging and GUI operations at the same time.

#### `Keylogger` Class
- **Attributes:**
  - `log`: Stores the captured keystrokes.
  - `is_logging`: Checks if logging is active.
  - `listener`: Keyboard listener object.
- **Methods:**
  - `__init__(self, root)`: Sets up the GUI components.
  - `start_logging(self)`: Starts keylogging.
  - `stop_logging(self)`: Stops keylogging.
  - `on_press(self, key)`: Captures and logs each key press.
  - `save_log(self)`: Saves the captured keystrokes to a file.

#### GUI Setup
- **Main Window**: Sets up the root window with a title and size.
- **Label**: Shows instructions to the user.
- **Buttons**: Start, Stop, and Save Log buttons to control the keylogger.

#### Running the Application
```python
if __name__ == "__main__":
    root = tk.Tk()
    app = Keylogger(root)
    root.mainloop()
```
- This starts the `Keylogger` class and the Tkinter main loop.

## ⚠️ Ethical Considerations
- Always tell users that their keystrokes are being logged.
- Get clear permission from users before using a keylogger.
- Use keyloggers only for good and legal purposes.

## Thanks👏
Thank you for using and contributing to this repository! I appreciate your interest and hope this keylogger helps you in learning Cyber Security.

## Contribute🤝
Contributions are welcome to improve these programs and add more features.

To contribute:
1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes and push them to your branch.
4. Open a pull request describing your changes.

✅ Ensure your code follows the existing style and includes appropriate documentation and tests.

## 🛡️Secure coding!🛡️
