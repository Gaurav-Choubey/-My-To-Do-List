# -My-To-Do-List
I'll break down how the `TodoListApp` code works and how you can run it on another PC.

### Explanation of the Code

#### 1. **Imports**
   - **`tkinter`**: A standard GUI library in Python used for creating graphical user interfaces.
   - **`ttk`**: A module within `tkinter` that provides themed widgets.
   - **`messagebox`**: Provides a way to show message dialogs.
   - **`json`**: Used for reading from and writing to JSON files.

#### 2. **`TodoListApp` Class**
   - **Inherits from `tk.Tk`**: This makes `TodoListApp` a subclass of `tk.Tk`, which is the main application window.

#### 3. **Constructor (`__init__` method)**
   - Sets up the main window's title and size.
   - Configures the style for various widgets.
   - Initializes a text entry for inputting tasks with placeholder text.
   - Adds buttons for adding, marking as done, deleting tasks, and viewing stats.
   - Initializes a `Listbox` for displaying tasks.
   - Calls `load_tasks` to load previously saved tasks from a file.

#### 4. **Event Handlers and Methods**
   - **`view_stats`**: Shows a message box with statistics about the total and completed tasks.
   - **`add_task`**: Adds a new task to the list if the input is valid.
   - **`mark_done`**: Marks the selected task as done (green color).
   - **`delete_task`**: Deletes the selected task.
   - **`clear_placeholder`**: Clears the placeholder text when the entry field is focused.
   - **`restore_placeholder`**: Restores the placeholder text if the entry field is empty.
   - **`load_tasks`**: Loads tasks from a JSON file and populates the listbox.
   - **`save_tasks`**: Saves the current tasks and their states (colors) to a JSON file.

### Running the Code on Another PC

To run this application on another PC, follow these steps:

#### 1. **Install Python**
   - Make sure Python is installed on the target PC. You can download it from the [official Python website](https://www.python.org/downloads/).

#### 2. **Prepare the Code**
   - Save the provided code to a file named `todo_list_app.py` or another `.py` file of your choice.

#### 3. **Install Required Libraries**
   - This application uses standard libraries, so you generally don’t need to install additional packages. Just make sure you have `tkinter`, which is included with Python's standard library.

#### 4. **Run the Application**
   - Open a terminal or command prompt.
   - Navigate to the directory where your `todo_list_app.py` file is located.
   - Run the script with the following command:
     ```bash
     python todo_list_app.py
     ```
   - The application window should open, and you can interact with it as intended.

#### 5. **Manage Files**
   - The application reads from and writes to a file named `tasks.json` for storing tasks. Ensure that the script has permission to read from and write to this file in its directory.

#### 6. **Troubleshooting**
   - **File Not Found**: If the JSON file (`tasks.json`) is missing, the application will create a new one when saving tasks.
   - **Permissions Issues**: Make sure the script has the necessary permissions to create and modify files in its directory.
   - **Python Version**: Ensure that you're using a compatible Python version (Python 3.x is recommended).

By following these steps, you should be able to run the `TodoListApp` on another PC with minimal issues. If you encounter specific errors or issues, feel free to ask for further assistance!
