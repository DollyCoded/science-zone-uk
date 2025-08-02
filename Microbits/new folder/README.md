# 🚨 Micro:bit Safety Alert System

## 👦👧 Age Group
10–12 years old

## 🎯 Learning Objectives (Based on Bloom's Taxonomy)
- **Remembering:** Understand what an alert system is and identify Micro:bit parts.
- **Understanding:** Explain how button inputs trigger outputs.
- **Applying:** Build a working safety alert using MicroPython.
- **Creating:** Design your own version with new icons and sounds.

## 🔧 Coding Concepts Used
- `print()`
- `display.scroll()`
- `display.show()`
- `Image`
- `button_a.was_pressed()` and `button_b.was_pressed()`
- `music.play()`
- `sleep()`
- `display.clear()`
- `while True:` loop

## 💡 Why This Project Matters
Children will learn how to use the Micro:bit to create a small device that shows alerts. It helps build logic, creativity, and real-world application thinking.

## 🔥 Warm-up Challenges
| Level | Task | Code |
|-------|------|------|
| Basic | Print "Hello World" in the console |
```python
print("Hello World")
```
| Medium | Show "Hello World" on the LED screen |
```python
from microbit import *
display.scroll("Hello World")
```
| Hard | Countdown from 5 then display message |
```python
from microbit import *
for i in range(5, 0, -1):
    display.scroll(str(i))
    sleep(500)
display.scroll("Hello World")
```

## 🧩 Main Project Challenge
**Build a simple safety alert system** that:
- Shows a warning when Button A is pressed
- Shows "All Clear" when Button B is pressed
- Displays icons and plays sounds

## ✅ Full MicroPython Code
```python
from microbit import *
import music

while True:
    # Alert when Button A is pressed
    if button_a.was_pressed():
        display.scroll("Warning!")
        display.show(Image.SKULL)
        music.play(music.BA_DING)
        sleep(2000)
        display.clear()

    # All Clear when Button B is pressed
    if button_b.was_pressed():
        display.scroll("All Clear!")
        display.show(Image.HAPPY)
        music.play(music.POWER_UP)
        sleep(2000)
        display.clear()
```

## 🚀 Remix Challenges
- Change the messages (e.g., "Fire!", "Help!")
- Use custom icons: `Image("09090:99999:99999:09990:00900")`
- Try sound patterns or melodies
- Add a reset function using both buttons

## 💬 Reflection Questions
1. How does the Micro:bit know when a button is pressed?
2. What could you use this alert system for in the real world?
3. How would you improve this system?

## 🔗 Helpful Links
- [Python Editor for Micro:bit](https://python.microbit.org/v/3)
- [Micro:bit Python Docs](https://microbit-micropython.readthedocs.io/en/v2-docs/)

---

Happy coding! 🎉

