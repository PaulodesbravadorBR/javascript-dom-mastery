# 🎯 Exclusive Selection Logic (Exercise 53)

This exercise transitions from a "checkbox" style (multiple items) to a "radio" style (one item) selection. This is a critical pattern for settings, payment methods, or currency preferences.

### 🛠️ The Logic Breakdown:


1. **The Reset Phase**: By running `cartoes.forEach(c => c.classList.remove("active"))`, we ensure the UI is "clean." No matter which button was selected previously, it will be turned off.
2. **The Activation Phase**: We immediately use `evento.currentTarget.classList.add("active")` to highlight the user's new choice.
3. **User Experience (UX)**: This provides instant visual feedback that a single choice has been registered.

### 🔍 Performance Note:
While we are looping twice (once to add listeners and once inside the click event), for a small number of elements (like 6 currency cards), this is extremely fast and the most readable way to write the code.