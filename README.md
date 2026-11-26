
# Task Manager (Python)

A command-line task manager. You can add, view, filter, and remove tasks, and chart them by priority. Tasks are saved to a local JSON file, and the core functions are covered by `pytest` tests.

[Video demo](https://youtu.be/n5WrlCtDvek)

**Built with:** Python, matplotlib, pytest

## Table of Contents

1. [Setup](#setup)
2. [Usage](#usage)
   - [Interactive Task Manager](#interactive-task-manager)
3. [Running the Tests](#running-the-tests)
4. [Visualizing Tasks](#visualizing-tasks)
5. [Screenshots](#screenshots)

---

## Setup

To set up and run this project, follow these steps:

1. **Clone the Repository**

   ```bash
   git clone https://github.com/LearnA1/project-taskmanager-python.git
   cd project-taskmanager-python
   ```

2. **Install Dependencies**

   Requires Python 3 and `pip`. Dependencies (`matplotlib`, `pytest`) are listed in `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

3. **Check Project Structure**

   The project directory should have the following structure:

   ```
   project-taskmanager-python/
   ├── project.py           # Main source code for the task manager
   ├── test_project.py      # Test file using pytest
   ├── requirements.txt     # List of dependencies
   ├── mytasks.json         # JSON file storing tasks
   └── README.md            # This file
   ```

---

## Usage

### Interactive Task Manager

An interactive command-line interface is provided to manage tasks without manually writing code. Run the following command to start the task manager:

```bash
python project.py
```

### Options Available:

1. **Add a Task**: Enter the description, due date (format `YYYY-MM-DD`), and priority (high, medium, low).
2. **View All Tasks**: Displays all tasks currently in the JSON file.
3. **View Tasks by Priority**: Filter tasks based on priority level.
4. **Remove a Task**: Delete a task by specifying its ID.
5. **Visualize Tasks by Priority**: Displays a bar chart of tasks categorized by priority.
6. **Pretty Print Tasks**: Outputs the JSON representation of tasks in a readable format.
7. **Exit**: Exit the interactive interface.

---

## Running the Tests

This project uses `pytest` for testing. All tests are contained in the `test_project.py` file.

### 1. Run All Tests

   To run all tests, execute:

   ```bash
   pytest -v
   ```

### 2. View Output Without Capturing

   To see print statements and other output during testing, use:

   ```bash
   pytest -v --capture=no
   ```

---

## Visualizing Tasks

The project includes a function to visualize tasks based on priority. To visualize tasks:

```python
from project import visualize_tasks_by_priority

visualize_tasks_by_priority()
```

This will generate a bar chart showing the count of tasks for each priority (e.g., high, medium, low).

---

## Screenshots

### Task Visualization
![Task Visualization](images/task_visualization.png)

### Running Tests
![Running Tests](images/running_tests.png)
