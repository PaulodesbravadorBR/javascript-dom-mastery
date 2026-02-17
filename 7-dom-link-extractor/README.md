# 🔗 DOM Link Extractor

This project is a technical demonstration of how to interact with multiple DOM elements simultaneously using JavaScript. It focuses on the power of `querySelectorAll` to identify and collect all links within a webpage.

## 🚀 Purpose
In web development, you often need to perform batch operations (like tracking all clicks, auditing SEO links, or styling navigation). This utility function serves as a foundation for any script that needs to analyze the link structure of a document.

## 🧠 Technical Concepts
- **`querySelectorAll`**: Unlike `querySelector`, which stops at the first match, this method scans the entire DOM and returns all matching elements.
- **NodeList Collection**: I learned that the returned value is a static `NodeList`, a specific type of collection that allows for easy iteration using methods like `.forEach()`.
- **Tag Selection**: Using the tag selector `"a"` to target anchor elements specifically.

## 🛠️ Implementation
The function efficiently captures all anchor tags as follows:

```javascript
/**
 * Retrieves all anchor elements (<a>) from the current page.
 * @returns {NodeList} A collection of all link elements found.
 */
const obterTodosLinks = () => {
    return document.querySelectorAll("a");
}
