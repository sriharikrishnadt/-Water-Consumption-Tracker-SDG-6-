# 📊 SDG Progress Analyzer

A simple Python data visualization project that analyzes Sustainable Development Goals (SDG) progress of different countries using Pandas and Matplotlib.

The program loads SDG data from a CSV file, allows the user to select a country, and displays a bar graph showing SDG scores.

This project demonstrates basic data analysis and visualization using Python.

## 🚀 Features
Load SDG dataset using Pandas

Filter SDG data by country

Visualize SDG scores using Matplotlib

Simple command-line interaction

Easy to extend with more countries and SDGs
## 🛠 Technologies Used
Python

Pandas

Matplotlib

CSV dataset

## 📂 Project Structure
```py
SDG-Progress-Analyzer
│
├── sdg_analyzer.py
├── sdg_data.csv
├── requirements.txt
└── README.md
```
## 📦 requirements.txt
### Create a file named requirements.txt
```py
pandas
matplotlib
```
### Install dependencies:
```py
pip install -r requirements.txt
```
## 🐍 Python Code (sdg_analyzer.py)
```py
import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
data = pd.read_csv("sdg_data.csv")

print("\nSDG Dataset:\n")
print(data)

# Select country
country = input("\nEnter country name (India/USA/Germany): ")

# Filter data
country_data = data[data["Country"] == country]

if country_data.empty:
    print("Country not found!")
else:
    # Plot graph
    plt.figure(figsize=(8,5))

    plt.bar(country_data["SDG"], country_data["Score"])

    plt.title(f"SDG Progress for {country}")
    plt.xlabel("Sustainable Development Goals")
    plt.ylabel("Score")

    plt.xticks(rotation=30)

    plt.tight_layout()

    plt.show()
```

## ▶️ How to Run

### 1️⃣ Install dependencies
```py
pip install pandas matplotlib
```
2️⃣ Run the program
```py
python sdg_analyzer.py
```
3️⃣ Enter country name
```py
Enter country name (India/USA/Germany): India
```
## Output:
<img width="996" height="706" alt="image" src="https://github.com/user-attachments/assets/9454e36d-2d36-474c-85e9-b11910131998" />

## Result:
Thus the project created is executed using VS code.
