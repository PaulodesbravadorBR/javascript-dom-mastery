# 🧭 Interactive Sidebar Toggle (Exercise 45)

This exercise focuses on creating an interactive side menu (off-canvas) using JavaScript to manipulate CSS states.

### 🛠️ Key Concepts Used:
* **`document.querySelector()`**: To grab the menu button and the sidebar container from the DOM.
* **`addEventListener("click", ...)`**: To detect when the user wants to open or close the menu.
* **`classList.toggle("show")`**: This is the most efficient way to switch states. If the `.show` class is there, it removes it; if not, it adds it.

### 🎨 The CSS Connection
The sidebar uses a `transform: translateX(-100%)` to stay hidden off-screen by default. When the `.show` class is added by our script, the CSS updates to `translateX(0)`. Because we have a `transition` property defined in CSS, the menu slides in smoothly rather than appearing instantly.



### ✅ Why use .toggle()?
Instead of writing complex `if/else` statements to check if the menu is open, `.toggle()` provides a clean, one-line solution to handle binary states (On/Off, Open/Closed, Dark/Light).