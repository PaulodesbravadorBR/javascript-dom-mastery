# 🎯 Understanding currentTarget (Exercise 49)

This exercise demonstrates why the `event` object is so powerful. Instead of relying on external variables, we use the event itself to tell us which element was interacted with.

### 🛠️ Key Concepts:
* **`evento.currentTarget`**: This property always refers to the element that has the event listener attached to it. 
* **Dynamic Access**: By using `currentTarget`, your functions become more reusable. If you attached this same function to 10 different buttons, it would correctly log the text of whichever button you clicked.



### 🔍 currentTarget vs. target (Pro Tip)
* **`currentTarget`**: The element that **owns** the event listener (the Button).
* **`target`**: The actual element you clicked (could be an icon *inside* the button).

In most basic cases, they are the same, but `currentTarget` is safer when your buttons contain other HTML elements like `<span>` or `<i>`.