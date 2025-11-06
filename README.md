# OOP Lab 1-2: Data Analysis with Classes

## Lab Overview

This lab focuses on refactoring procedural-style data processing code into an **object-oriented design**.  
It introduces two main classes:

- `DataLoader` 
- `Table` 

The program demonstrates how OOP principles like **encapsulation** and **abstraction** can simplify real-world data analysis workflows.

---

## Project Structure

oop_lab2/
│
├── README.md 
├── Cities.csv 
└── data_processing.py 

## Design Overview

### `DataLoader` Class

**Purpose:** Handles loading CSV files.

**Attributes:**

- `base_path`: The directory containing the dataset.

**Key Methods:**

- `load_csv(filename)`: Loads the CSV and returns a list of dictionaries.

---

### `Table` Class

**Purpose:** Represents tabular data and provides methods for data analysis.

**Attributes:**

- `name`: The name of the table.
- `table`: The list of dictionaries containing the dataset.

**Key Methods:**

- `filter(condition)`: Returns a new `Table` containing only the rows that meet the specified condition.
- `aggregate(agg_func, column)`: Applies an aggregation function (e.g., average, sum, max) to a given column.

---

## How to Test and Run

1. Ensure `Cities.csv` is in the same folder as `data_processing.py`.
2. Run the program:
   ```bash
   python data_processing.py
   ```
