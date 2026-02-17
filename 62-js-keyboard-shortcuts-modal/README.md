# ⌨️ Keyboard Shortcuts Project

This project implements global keyboard shortcuts to improve accessibility and speed in a participant management application.

## 🚀 Key Learning Objectives

### 1. Global Event Listeners
The `keyup` event is attached to the `document` object rather than a specific input. This allows the application to listen for shortcuts regardless of where the user's focus is currently located on the page.

### 2. State-Dependent Logic
To prevent bugs (like the 'n' key triggering a toggle while the user is typing a name inside the modal), the logic checks for the presence of the `.show` class:
- **Key 'n'**: Only calls `toggleModal()` if the modal is **hidden**.
- **Key 'Escape'**: Only calls `toggleModal()` if the modal is **visible**.

### 3. The `event.key` Property
Instead of using deprecated `keyCode` or `which` values, this project uses the modern `event.key` property, which returns the literal string value of the key pressed (e.g., "n", "Escape").

## 🛠️ Shortcuts Implemented
| Key | Action | Condition |
| :--- | :--- | :--- |
| **n** | Open Modal | Modal must be closed |
| **Escape** | Close Modal | Modal must be open |