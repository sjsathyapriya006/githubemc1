# TASK 1: MATRIX OPERATIONS
# This program performs addition, subtraction, and multiplication of matrices
# without using any external libraries.

a = [[1, 2], [3, 4]]
b = [[5, 6], [7, 8]]

print("Matrix A:")
print(a)

print("\nMatrix B:")
print(b)

# Matrix Addition
add = [[a[i][j] + b[i][j] for j in range(2)] for i in range(2)]
print("\nAddition (A + B):")
print(add)

# Matrix Subtraction
sub = [[a[i][j] - b[i][j] for j in range(2)] for i in range(2)]
print("\nSubtraction (A - B):")
print(sub)

# Matrix Multiplication
mul = [
    [a[0][0]*b[0][0] + a[0][1]*b[1][0],
     a[0][0]*b[0][1] + a[0][1]*b[1][1]],
    [a[1][0]*b[0][0] + a[1][1]*b[1][0],
     a[1][0]*b[0][1] + a[1][1]*b[1][1]]
]

print("\nMultiplication (A x B):")
print(mul)

# TASK 2: STUDENT MARK DATA ANALYSIS
# This program stores student marks and calculates the average for each student.

students = [
    {"name": "a", "maths": 78, "science": 85, "english": 74},
    {"name": "b", "maths": 88, "science": 90, "english": 82},
    {"name": "c", "maths": 65, "science": 70, "english": 68},
    {"name": "d", "maths": 92, "science": 95, "english": 89},
    {"name": "e", "maths": 55, "science": 60, "english": 58},
]

print("Student Marks Data:\n")

for s in students:
    print(s)

print("\nAverage Marks:\n")

for s in students:
    avg = (s["maths"] + s["science"] + s["english"]) / 3
    print("Name:", s["name"], "| Average:", round(avg, 2))

    # TASK 3: HOUSE PRICE PREDICTION
# This program calculates the average price per square foot
# using a simple dataset.

houses = [
    {"area": 800, "price": 3500000},
    {"area": 1000, "price": 5000000},
    {"area": 1200, "price": 6200000},
    {"area": 1500, "price": 8000000},
    {"area": 1800, "price": 9500000}
]

print("House Price Dataset:\n")

for h in houses:
    print(h)

total_price = 0
total_area = 0

for h in houses:
    total_price += h["price"]
    total_area += h["area"]

price_per_sqft = total_price / total_area
print("\nAverage Price per Sqft:", round(price_per_sqft, 2))

# Python Development Internship Tasks

This repository contains Python programs completed as part of a
**Python Development Internship**.

All tasks are implemented using **core Python only**, without using
any external libraries.

---

## Task 1: Matrix Operations
- Performs matrix addition, subtraction, and multiplication
- Uses lists and basic Python logic

---

## Task 2: Student Mark Data Analysis
- Stores student data using dictionaries
- Calculates average marks for each student

---

## Task 3: House Price Prediction
- Uses area and price dataset
- Calculates average price per square foot
- Demonstrates basic prediction logic

---

## Technologies Used
- Python 3
- Core Python concepts

---

## Author
**Vaishnavi**  
Python Development Intern
