# Java Console Task Manager

## Description

This is a simple yet effective console-based task management application built in Java. It allows users to create, view, update, and delete tasks. Tasks are persisted to a local `tasks.csv` file, so your to-do list remains available even after closing and reopening the application. This project demonstrates core Java concepts including Object-Oriented Programming (OOP), file I/O, data structures (ArrayList), and basic command-line user interaction.

## Features

* **Add New Tasks:** Create tasks with a description, due date (YYYY-MM-DD format), and priority (High, Medium, Low).
* **View All Tasks:** Display a list of all current tasks, sorted by their unique ID.
* **Update Task Status:** Mark tasks as "Pending" or "Completed".
* **Delete Tasks:** Remove tasks from the list.
* **Persistent Storage:** Tasks are automatically loaded from and saved to a `tasks.csv` file in the application's root directory.
* **Manual Save:** Option to manually save the current task list to the file.
* **Automatic Save on Exit:** Ensures no data loss when closing the application.
* **User-Friendly Console Interface:** Clear menu options and input prompts.

## How to Compile and Run

1.  **Prerequisites:**
    * Java Development Kit (JDK) installed (e.g., JDK 8 or later).

2.  **Clone the Repository (Optional - if you've pushed it to GitHub):**
    ```bash
    git clone <your-repository-url>
    cd <repository-directory>
    ```

3.  **Save the Files:**
    Ensure the following Java files are in the same directory:
    * `Task.java`
    * `TaskManager.java`
    * `Main.java`

4.  **Compile:**
    Open a terminal or command prompt in the directory containing the Java files and run:
    ```bash
    javac Main.java TaskManager.java Task.java
    ```

5.  **Run:**
    After successful compilation, run the application using:
    ```bash
    java Main
    ```

    You should see the Task Manager menu appear in your console.

## File Structure

.
├── Task.java           // Defines the Task object and its properties.
├── TaskManager.java    // Handles the core logic for managing tasks (add, view, update, delete, file I/O).
├── Main.java           // Provides the command-line user interface and main application loop.
└── tasks.csv           // (Generated at runtime) Stores the task data.


## Technologies Used

* **Java:** Core programming language.
* **Java Standard Library:**
    * `java.util.Scanner` for user input.
    * `java.util.ArrayList` for storing tasks in memory.
    * `java.io.*` classes (BufferedReader, BufferedWriter, FileReader, FileWriter) for file operations.
    * `java.util.Optional` for safer handling of potentially missing tasks.
    * `java.util.Comparator` and Streams API for sorting.

## Potential Future Enhancements

* **Advanced Input Validation:** Implement more robust checks for date formats, priority inputs, etc.
* **Edit Task Details:** Allow users to modify the description, due date, or priority of existing tasks.
* **Task Filtering:** Add options to view tasks based on status (e.g., only pending), priority, or due date range.
* **Task Sorting:** Allow users to sort tasks by due date, priority, or description in addition to ID.
* **Sub-tasks:** Implement a hierarchy where tasks can have sub-tasks.
* **Date/Time Handling:** Use `java.time` package for more sophisticated date and time management, including parsing and validation.
* **Improved CSV Handling:** Use a dedicated CSV parsing library (like Apache Commons CSV or OpenCSV) for more robust and flexible CSV processing, especially for complex data.
* **Alternative Data Storage:**
    * **JSON:** Save tasks to a JSON file for better structure and readability.
    * **Database:** Integrate with a lightweight database like SQLite for more complex querying and scalability.
* **Unit Testing:** Write JUnit tests to ensure the reliability of different components.
* **GUI Implementation:** Develop a graphical user interface using Java Swing or JavaFX for a more visual and interactive experience.

---

*This README was generated to help showcase the Java Console Task Manager project.*
