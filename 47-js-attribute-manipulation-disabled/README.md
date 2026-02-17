# 🚫 Attribute Manipulation: Disabled State (Exercise 47)

In this exercise, we go beyond styling and actually change the **behavior** of a DOM element by modifying its HTML attributes.

### ⚙️ Logic Workflow:
1. **Selection**: We identify the "Start" button and the two control buttons (Activate/Deactivate).
2. **Disabling**: When the user clicks "Desativar", we use `setAttribute("disabled", "true")`. This tells the browser to ignore clicks on the Start button and apply the `:disabled` CSS styles.
3. **Enabling**: When the user clicks "Ativar", we use `removeAttribute("disabled")`. Simply removing the attribute is enough to make the button interactive again.



### 🛠️ Key Technical Methods:
* **`setAttribute(name, value)`**: Adds a new attribute or changes the value of an existing attribute on the specified element.
* **`removeAttribute(name)`**: Removes an attribute from the element, effectively resetting its default behavior (in this case, making it clickable again).

### 💡 Why not just use .disabled = true?
While `element.disabled = true` works for properties, `setAttribute` is a more generic and powerful method that works for **any** HTML attribute (like `aria-labels`, `data-attributes`, or `src`), making it a vital tool in your JavaScript kit.