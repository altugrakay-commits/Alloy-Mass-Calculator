# Alloy-Mass-Calculator
A Python script to calculate elemental mass from a JSON database with robust error handling.

### Goal
This project was developed during my first year of Materials Technology Engineering studies at Bergsskolan. The primary objective was to create a reliable Python script that takes user input (total batch mass and alloy grade) and dynamically extracts the precise elemental masses required from a JSON database.

The core challenge was building a solution that could handle the variability in real-world data, specifically missing minimum values, maximum-only data, string values (e.g., "less than 0.75"), and standard numerical ranges.

### Technical Stack
*   **Python:** The primary programming language used for logic and calculations.
*   **Pandas:** Used for efficient data processing and filtering of the JSON data structure.
*   **JSON:** The data source format for the steel alloy percentages.
*   **JupyterLab/Notebooks:** The development environment used for rapid iteration and testing.

### Key Achievements & Problem Solving
This project showcases my ability to implement resilient logic for complex scenarios:

*   **Advanced Error Handling:** Implemented comprehensive `try/except` blocks to manage runtime errors gracefully, preventing the program from crashing due to unexpected data types (e.g., trying to do math on a string or a dictionary).
*   **Nested Conditional Logic:** Utilized nested `if/elif/else` statements within the `except` blocks to differentiate between three distinct data variations:
    *   Single numerical values (e.g., grade 304).
    *   Dictionaries with only a `'max'` key (e.g., grade 321).
    *   String descriptions (e.g., grade 430).
*   **Data Validation:** Ensured all variables are correctly assigned and utilized professional f-string formatting for clear, user-friendly output in the console.

### How to Run the Project
1.  Clone or download this repository to your local machine.
2.  Ensure Python and the Pandas library are installed (`pip install pandas`).
3.  Run the main Python script (e.g., `python your_script_name.py`) in your terminal or Jupyter environment.
4.  Follow the prompts to enter a total mass and a grade number (e.g., 304, 310, 316, 321, or 430).

### Contact: altug.akay@bergsskolan.se

### License
This project is covered under the [MIT License](LICENSE).
