# 🔄 NodeList Traversal & Quantification

This project explores the nuances of handling **NodeLists** in JavaScript. Unlike standard Arrays, NodeLists require a specific approach when interacting with their internal elements, especially when following strict architectural patterns.

## 🚀 The Challenge
The goal was to count all anchor tags (`<a>`) in a document. While `.length` is the most direct method, this project focuses on the **Iteration Technique**, ensuring each node is accessed individually—a crucial skill for performing bulk updates or data extraction.

## 🧠 Technical Insights
- **Individual Access**: Properties like `textContent` or `href` cannot be called on the NodeList itself; they must be accessed on individual elements.
- **Traversal Logic**: Using `.forEach()` to loop through the collection, which is the standard way to interact with each element in a NodeList safely.
- **NodeList vs. Array**: Reinforcing that while a NodeList has a `.length` property and supports `forEach`, it lacks array methods like `.filter()` or `.map()`.

## 💻 Code Implementation (The Iteration Method)
```javascript
const obterNumerosDeLinks = () => {
    const links = document.querySelectorAll("a");
    let count = 0;

    // Iterating through each node to calculate the total
    links.forEach(() => {
        count++;
    });

    return count;
}
