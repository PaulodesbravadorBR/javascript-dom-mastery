# 🌍 Simple Translation Selector

A practical exercise using the JavaScript `change` event to create a dynamic greeting system based on user selection.

## 🚀 Technical Insights

### 1. The `change` Event
This project demonstrates the use of the `change` listener on a `<select>` element. Unlike text inputs, where events might fire on every keystroke, the `change` event for dropdowns is perfectly suited for triggering actions only when a definitive selection is made.

### 2. Nullish Coalescing (`??`)
The internal logic uses the `??` operator within the `obterTraducao` function. This provides a safe "fallback" mechanism: if the selected language doesn't exist in our dictionary (like Spanish or Italian in this current version), the app defaults to "Welcome".

### 3. Dynamic DOM Updates
By accessing `element.value` inside the listener, we capture the current state of the UI and immediately reflect the change in the `#saida-textual` paragraph using `textContent`.

## 🛠️ How to Test
1. Select a language from the dropdown menu (Dutch, French, or English).
2. The greeting below the form will update instantly to the correct translation.
3. If you select a language not yet defined in the object, it will default to English.