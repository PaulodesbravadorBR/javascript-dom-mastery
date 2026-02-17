# 🔘 Interactive Button Toggle (Exercise 50)

This final exercise solidifies the workflow of modern JavaScript DOM manipulation. 

### ⚙️ The Logic Workflow:
1. **User Interaction**: The user clicks the button.
2. **Event Capture**: The browser triggers the `click` event and passes the `evento` object to our function.
3. **Target Identification**: We use `evento.currentTarget` to pinpoint exactly which element was clicked.
4. **State Change**: `classList.toggle("active")` checks the element:
    * If `.active` is missing ➔ **Add it** (Button turns teal/accent color).
    * If `.active` is present ➔ **Remove it** (Button returns to orange/primary color).



### 💡 Why this matters:
By using `evento.currentTarget` instead of the variable `botao` inside the listener, your code is more robust. If you later decided to add a second button with a different ID but the same logic, you could reuse the same function without rewriting it!