# NumPy-Data-Filtering

## 📌 Project Overview

This project demonstrates numerical data filtering using NumPy in Python. It uses student average marks from a CSV dataset to identify values above, below, and equal to specified thresholds.

The project focuses on **Boolean conditions, Boolean indexing, and filtering numerical data**.

Completed as part of **Task 13 (Level 1, Day 13)** of the AI & ML Internship at **Veda Technology**, using Google Colab.

## 🎯 Objective

To learn how to use NumPy conditions to filter numerical values based on specified thresholds.

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Google Colab
- GitHub

## 📂 Dataset

The project uses the `grade-records(1).csv` dataset containing student grade records.

The `Student Average` column is used as the numerical data for filtering. Percentage symbols, if present, are removed before converting values to numbers.

## 📚 Task Requirements

This project covers the following requirements:

- Create a NumPy array containing numerical values.
- Filter values above a specified threshold.
- Filter values below a specified threshold.
- Filter values equal to a specified threshold.
- Try different thresholds.
- Use Boolean indexing to return matching values.

## 💻 Implementation

### 1. Create a NumPy Array

Student averages are converted into a NumPy array for filtering.

```python
data = df["Student Average"].to_numpy()
```

### 2. Filter Values Above a Threshold

```python
threshold = 50
above = data[data > threshold]
print(above)
```

This returns values greater than 50.

### 3. Filter Values Below a Threshold

```python
threshold = 50
below = data[data < threshold]
print(below)
```

This returns values less than 50.

### 4. Filter Values Equal to a Threshold

```python
threshold = 50
equal = data[data == threshold]
print(equal)
```

This returns values exactly equal to 50. The result may be empty if no matching value exists.

### 5. Boolean Indexing

```python
condition = data > 50
filtered_data = data[condition]

print("Boolean condition:", condition)
print("Filtered values:", filtered_data)
```

Boolean indexing selects only the values for which the condition evaluates to `True`.

## 🔍 Filtering with Different Thresholds

The notebook tests multiple thresholds, such as 40, 60, 70, and 80, to demonstrate how filtering results change.

```python
thresholds = [40, 60, 70, 80]

for threshold in thresholds:
    print(f"Values above {threshold}:", data[data > threshold])
```

## ⚡ Key Concept: Boolean Indexing

Boolean indexing uses a condition to create a Boolean array containing `True` and `False` values.

For example:

```python
data = np.array([35, 45, 50, 65, 80])
print(data[data > 50])
```

Output:

```text
[65 80]
```

Only values greater than 50 are returned.

## ▶️ How to Run the Project

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `NumPy_Data_Filtering.ipynb`.
3. Upload the `grade-records(1).csv` dataset when prompted by the notebook.
4. Run the cells in order.
5. Review the filtered values and Boolean indexing results.

NumPy and Pandas are generally preinstalled in Google Colab.

## 📁 Project Structure

```text
NumPy-Data-Filtering/
│
├── NumPy_Data_Filtering.ipynb
├── grade-records(1).csv
└── README.md
```

The CSV file should be included in the repository only if you have permission to share it. Otherwise, upload it to your Colab session when running the notebook.

## 📈 Learning Outcomes

Through this task, I learned how to:

- Create and work with NumPy arrays.
- Apply Boolean conditions to numerical data.
- Filter values above, below, and equal to thresholds.
- Use Boolean indexing to select matching values.
- Experiment with different filtering thresholds.
- Use NumPy for basic data analysis.

## 🏁 Conclusion

This task provided practical experience with NumPy data filtering. By applying Boolean conditions and indexing to student average marks, I learned how to select numerical values that meet specific criteria.

## 👨‍💻 Internship Details

- **Organization:** Veda Technology
- **Track:** AI & ML
- **Task:** Task 13 — NumPy Data Filtering
- **Level:** Level 1
- **Day:** Day 13
- **Platform:** Google Colab

---

⭐ This project is part of my AI & ML internship learning journey.
