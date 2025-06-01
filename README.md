# 🧾 HR Employee Analytics Dashboard (Pandas Intermediate Project)

This project is a real-world **data cleaning and analytics application** using intermediate-level Pandas functionality. It simulates a typical HR dataset and performs meaningful transformations and insights to help HR teams better understand their workforce.

---

## 📌 Features

- Clean and preprocess missing employee data (age, salary, department).
- Engineer new features like **age groups** and **name initials**.
- Perform **group-by** aggregations to analyze salaries by department and age group.
- Use **pivot tables** for multidimensional analysis.
- Filter employees based on **join date**.
- Sort employees by multiple criteria.
- Demonstrates safe, **future-proof Pandas coding** practices.

---

## 🛠️ Technologies

- Python 3.x
- Pandas

---

## 📂 Dataset

The dataset is simulated for demonstration and contains:

| Column     | Description                        |
|------------|------------------------------------|
| Name       | Employee name                      |
| Age        | Age (with some missing values)     |
| Department | Department name (HR, Engineering…) |
| JoinDate   | Date the employee joined           |
| Salary     | Annual salary                      |

---

## 🧪 Data Processing Steps

1. **Missing Data Handling**
   - Fill missing `Age` and `Salary` with column mean.
   - Fill missing `Department` with `'Unassigned'`.

2. **Feature Engineering**
   - Add `AgeGroup`: 'Junior' (<30) or 'Senior' (>=30).
   - Add `Initial`: First letter of the employee's name.

3. **Aggregations**
   - Calculate average salary by `Department` and `AgeGroup`.
   - Create a pivot table of employee counts.

4. **Filtering**
   - List employees who joined after January 1, 2021.

5. **Sorting**
   - Sort dataset by `Department` and descending `Salary`.

---

## 📈 Sample Outputs

**Grouped Salary Summary**

 Department AgeGroup   Salary
0 Engineering Senior 80000.0
1 HR Junior 51000.0
2 HR Senior 60000.0
3 Sales Junior 55000.0
4 Unassigned Senior 59400.0

**Pivot Table**
AgeGroup Junior Senior
Department
Engineering 0 1
HR 1 1
Sales 1 0
Unassigned 0 1

## 📁 File Structure

.
- ├── employee_analytics.py # Main analysis script
- ├── cleaned_data.csv # (Optional) Output file
- ├── README.md # Project documentation

## ✅ How to Run

1. Make sure Python and Pandas are installed.
2. Run the script
