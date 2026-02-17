# 💱 Dynamic Currency Selector

This project is part of my specialized study series on **DOM (Document Object Model) Manipulation**. It features a UI component where the system identifies in real-time which option (currency) the user has selected.

## 🚀 Key Features
Users can click on different currency cards (EUR, USD, GBP, etc.). The interface visually highlights the selected card, while JavaScript dynamically captures the inner value of the element holding the active state (`.active`).

## 🧠 Core Concepts Applied
- **Composite Selectors**: Utilizing `document.querySelector(".card.active")` to target elements with multiple classes.
- **State Management**: Identifying which element holds the "selected" state at the exact moment of interaction.
- **Event Listeners**: Integrating click events to synchronize logic with user actions.
- **Defensive Programming**: Implementation of null checks to ensure the function returns a fallback (empty string) instead of throwing an error if no element is found.

## 🛠️ Tech Stack
- **HTML5**: Semantic structure.
- **CSS3**: CSS Variables (custom properties), Grid Layout, and transitions.
- **JavaScript (ES6+)**: Dynamic selectors and arrow functions.

## 💻 Logic Breakdown
The function targets the specific intersection of classes to extract the correct value:

```javascript
const getSelectedCurrency = () => {
    // Find the element currently holding the 'active' state class
    const activeCard = document.querySelector(".card.active");

    // Return the text content if found, otherwise return an empty string
    return activeCard ? activeCard.textContent : "";
}
