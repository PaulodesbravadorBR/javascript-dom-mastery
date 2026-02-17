# 🌙 Global Theme Toggle (Exercise 46)

In this project, we implement a "Dark Mode" feature by manipulating the root element of the document.

### ⚙️ How it works:
1. **Targeting the Root**: Instead of changing individual elements, we target `document.documentElement`, which represents the `<html>` tag.
2. **Class Toggling**: We use `classList.toggle("escuro")`. 
    * If `<html>` doesn't have the class, it is added.
    * If it already has it, it is removed.
3. **CSS Inheritance**: In the style block, we have a rule `html.escuro { ... }`. Because this class is at the very top of the DOM tree, it affects everything below it.



### 🧪 Key Technical Concept: documentElement
The `document.documentElement` is a read-only property that returns the Element that is the root element of the document (the `<html>` element for HTML documents). It is the standard way to access global styles or CSS variables defined in `:root`.

### ✅ Result:
With a single click, the entire background and text color of the application shift, providing a modern user experience and protecting the user's eyes in low-light environments.