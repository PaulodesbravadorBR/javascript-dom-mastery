# 📑 DOM Text Extractor

This project focuses on the programmatic extraction of information from the Document Object Model (DOM). It demonstrates how to handle multiple elements simultaneously to retrieve their human-readable content.

## 🚀 The Goal
The challenge was to access every link (`<a>`) on a page and log its specific text. This simulates real-world tasks like SEO auditing, where you might need to list all "Call to Action" labels on a landing page.

## 🧠 Key Learnings
- **The .textContent Property**: Unlike `innerHTML`, `textContent` retrieves only the raw text, making it safer and more performant for data extraction.
- **Implicit Iteration**: Reinforcing that properties must be accessed on individual nodes. Calling a property on a `NodeList` directly returns `undefined`.
- **Arrow Function Scoping**: Using clean ES6 syntax to handle each element within the `forEach` loop.

## 💻 Implementation
The following logic ensures that each link's text is isolated and processed:

```javascript
const logarTextosComLinks = () => {
    const links = document.querySelectorAll("a");

    // Accessing individual elements within the collection
    links.forEach(link => {
        console.log(link.textContent);
    });
}
