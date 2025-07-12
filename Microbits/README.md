Getting started
---
Open MU editor or download it [here](https://codewith.mu/)

![Mu](mu_editor.png)


---

### 🌟 1. Starter - Scroll a Message

**Concept:** This is your very first Micro\:bit program! You're using a built-in function called `display.scroll()` to scroll text across the LED screen. It's a great way to check if your Micro\:bit is working and to try your first bit of Python.     
**Pseudocode:**

```
Import the microbit tools
Scroll the message "Hello!" across the screen
```

Copy into the editor and flash your microbit.    

Troubleshooting if flash fails:       
- Close the repl to enable flash button
- If flash hangs up, disconnect/reconnect cable and flash again
- Press reset button on back of microbit resets the code

```python
from microbit import *

display.scroll("Hello!")
```

![Mu](mu_editor_flash.png)


---
