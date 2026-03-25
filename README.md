# -Water-Consumption-Tracker-SDG-6-
## 💧 Water Consumption Tracker (SDG 6)
## 📌 Project Overview

The Water Consumption Tracker is a Python-based project that helps users monitor their daily water usage.

The system records water used for drinking, bathing, cooking, and washing, calculates the total water consumption, and gives suggestions to save water.

This project supports Sustainable Development Goal 6: Clean Water and Sanitation by encouraging responsible water usage.

## 🎯 Objectives
To monitor daily water consumption
To promote water conservation awareness
To help users reduce unnecessary water usage
To support sustainable water management
## 🛠️ Technologies Used
Python

VS Code
## ⚙️ Features
Track water usage for different activities
Calculate total daily water consumption
Display water usage report
Provide suggestions to save water
Simple console-based interface
## ▶️ How to Run the Project
Open the project in VS Code
Open Terminal
Run:
```py
python main.py
```

## 🧪 Sample Input:
```py
Enter water used for drinking (liters): 2
Enter water used for bathing (liters): 40
Enter water used for cooking (liters): 5
Enter water used for washing (liters): 20
```
## 📊 Sample Output:
```py
💧 --- Water Consumption Report ---
Total water used today: 67 liters

⚠️ Water usage is high. Try to save water.

💡 Water Saving Tips:
- Turn off taps when not in use
- Fix leaking pipes
- Use buckets instead of showers
- Reuse water for plants
```

## 🌱 Future Enhancements
Store daily water usage data
Display charts using Matplotlib
Add monthly water consumption report
Create GUI using Tkinter

## 🌍 SDG Goal

This project supports SDG 6: Clean Water and Sanitation, which focuses on ensuring sustainable management and availability of water for everyone.

## 💻 PROGRAM
```py
# Water Consumption Tracker (SDG 6)

def get_water_usage():
    drinking = float(input("Enter water used for drinking (liters): "))
    bathing = float(input("Enter water used for bathing (liters): "))
    cooking = float(input("Enter water used for cooking (liters): "))
    washing = float(input("Enter water used for washing (liters): "))

    total = drinking + bathing + cooking + washing
    return total


def show_report(total):
    print("\n💧 --- Water Consumption Report ---")
    print(f"Total water used today: {total} liters")

    if total < 50:
        print("✅ Great! You are saving water.")
    elif total < 100:
        print("👍 Moderate water usage.")
    else:
        print("⚠️ Water usage is high. Try to save water.")

    print("\n💡 Water Saving Tips:")
    print("- Turn off taps when not in use")
    print("- Fix leaking pipes")
    print("- Use buckets instead of showers")
    print("- Reuse water for plants")


def main():
    print("💧 Water Consumption Tracker 💧")

    total_water = get_water_usage()
    show_report(total_water)


# Run program
main()
```
## Output:
<img width="1355" height="429" alt="image" src="https://github.com/user-attachments/assets/e53fa4a9-7944-493b-9cbf-7b1173cab6a6" />

## 📊 Result

The Water Consumption Tracker helps users understand their daily water usage and encourages responsible water consumption.
It promotes awareness about water conservation and sustainable living

