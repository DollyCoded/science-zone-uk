# 🐍 Python Tip Calculator Workshop 🎉

> 🚀 **New coders**  
> ✏️ **Use Thonny to write your Python code**

---

## 🎈 Activity 1: My First Tip Calculator 🎈

### 🌟 What will you learn?

You'll make a Python program that works out how much tip to add when sharing a bill!


---

### 🔍 Step 1: Guess What Happens!

Look at this code carefully:

```python
print("Welcome to the tip calculator!")
bill = float(input("What was the total bill? $"))
tip = int(input("How much tip? 10, 12, or 15? "))
people = int(input("How many people sharing? "))

tip_percent = tip / 100
total_tip = bill * tip_percent
total_bill = bill + total_tip
amount_each = total_bill / people
final_amount = round(amount_each, 2)

print(f"Each person pays: ${final_amount}")
```

✍️ **Guess:** If the bill is `$100`, tip is `15`, and 4 people share, how much does each pay?
- open Thonny
- Use thonny to calculate your answer ```print((115/4) ```


---

### ▶️ Step 2: Let's Run It!

1. Open **Thonny**.
2. Copy the code above into Thonny.
3. Press ▶️ **Run** to test your guess!

Did you guess correctly?

---

### 🧐 Step 3: Let's Understand

Match the lines to what they do:

| Code | What it does |
|------|--------------|
| `bill = float(input(...))` | 1. Asks for the bill |
| `tip = int(input(...))` | 2. Asks for the tip |
| `tip_percent = tip / 100` | 3. Changes tip to a decimal |
| `total_tip = bill * tip_percent` | 4. Calculates the tip amount |
| `total_bill = bill + total_tip` | 5. Adds tip to the bill |
| `amount_each = total_bill / people` | 6. Splits bill between people |
| `final_amount = round(amount_each, 2)` | 7. Rounds the number |
| `print(...)` | 8. Shows the result |

---

### 🛠️ Step 4: Let's Change It!

Try these changes in Thonny:

- Add a 20% tip option:
```python
tip = int(input("How much tip? 10, 12, 15, or 20? "))
```

- Add a friendly goodbye message:
```python
print("Thanks! 😊")
```

---

### 🎨 Step 5: Now Create Your Own!

Can you add your name to the program?  
Can you put emojis into your messages?

---

## 🚀 Activity 2: Tip or No Tip! 🚀

### 🌟 What will you learn?

You'll add a choice to include or skip the tip!

---

### 🔍 Step 1: Guess Again!

Look carefully:

```python
print("Welcome to your tip calculator!")

name = input("What's your name? ")
tip_choice = input("Would you like to add a tip? yes/no: ")

bill = float(input("What was the bill? $"))
people = int(input("How many people sharing? "))

if tip_choice.lower() == "yes":
    tip = int(input("Tip amount: 10, 12, 15? "))
    tip_percent = tip / 100
    total_tip = bill * tip_percent
    total_bill = bill + total_tip
else:
    total_bill = bill

amount_each = total_bill / people
final_amount = round(amount_each, 2)

print(f"{name}, each person pays: ${final_amount}")
```

✍️ **Guess:** If you say **no** to the tip, what happens?  
✍️ **Guess:** What if the bill is `$80`, 2 people, and no tip?

---

### ▶️ Step 2: Try It in Thonny!

Test with tip and without tip. Did you guess right?

---

### 🧐 Step 3: What's New?

Write what these lines mean in your own words:

- `tip_choice = input(...)`
- `if tip_choice.lower() == "yes":`
- `else:`

---

### 🛠️ Step 4: Improve Your Code!

Make these small changes:

- Add a goodbye:
```python
print("Have a great day! 🌞")
```

- Always show two decimals:
```python
print(f"{name}, each person pays: ${final_amount:.2f}")
```

---

### 🎨 Step 5: Your Super Challenge!

Try adding a meal type or ask about service (good, okay, bad) and change the tip automatically!

---

🌟 **Great job! You are becoming a Python star! 🌟**
