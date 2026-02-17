# 💱 Currency Selector Grid (Exercise 52)

This exercise moves from simple buttons to "Cards," a common UI pattern in modern web apps (like checkout pages or settings dashboards).

### 🛠️ Key Concepts Applied:
* **Grid Selection**: We manage a 3-column grid layout where each item needs independent logic.
* **State Persistence**: By using `.toggle()`, we allow the user to change their mind and "deselect" a currency by clicking it again.
* **The `evento` Object**: Using `evento.currentTarget` ensures that even if you click the text inside the button, the whole button gets the style change.



### 💡 Pro Logic Tip:
Because we are using `toggle`, the code handles both the "Add" and "Remove" logic automatically. If the `active` class is there, it's removed. If it's missing, it's added. This keeps our JavaScript clean and prevents us from writing complex `if/else` statements.