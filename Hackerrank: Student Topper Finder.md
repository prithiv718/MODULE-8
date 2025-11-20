# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
```
Dictionary with student names and their marks in five subjects
student_marks = {
 'Alice': [85, 92, 78, 90, 88],
 'Bob': [75, 80, 70, 85, 90],
 'Charlie': [95, 85, 92, 88, 91],
 'Daisy': [60, 65, 70, 58, 62],
 'Ethan': [88, 82, 85, 87, 90]
}
# Dictionary to store total marks
 Saveetha Engineering College
total_marks = {}
# Calculate total marks
for name, marks in student_marks.items():
 total = sum(marks)
 total_marks[name] = total
# Find the topper
topper = max(total_marks, key=total_marks.get)
top_score = total_marks[topper]
# Display results
print("Total Marks of Each Student:")
for name, total in total_marks.items():
 print(f"{name}: {total}")
print(f"\nTopper: {topper}")
print(f"Top Score: {top_score}")
```
## OUTPUT
<img width="538" height="123" alt="image" src="https://github.com/user-attachments/assets/ed73c5fd-ee21-4261-8d27-d0b70854aeb5" />

## RESULT
Thus the program has been successfully executed.
