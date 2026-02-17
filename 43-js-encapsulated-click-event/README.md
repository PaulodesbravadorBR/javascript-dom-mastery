# 📦 Encapsulated Event Listeners (Exercise 44)

In this exercise, we practice a cleaner way to organize code by wrapping our event listener initialization inside a dedicated function.

### ⚙️ How it works:
1. **Initialization**: The `iniciarCumprimentoClique()` function is called immediately.
2. **Variable Creation**: Inside the function, a variable `botao` is created to hold the reference to `#meu-botao`.
3. **Binding**: The `.addEventListener("click", ...)` binds the logic to that specific button.
4. **Action**: Even after the function finishes executing its main thread, the listener stays "active" in the browser's memory, waiting for the user to interact.



### 🧪 Key Takeaway
Encapsulating logic in functions like `init()` or `setupEventListeners()` is a best practice. It prevents the global scope from being cluttered with variables and allows you to control exactly **when** certain interactions should become available to the user.

### ⚠️ Common Pitfall
If you define the variable `botao` outside the function but try to use it inside a function that hasn't been called yet, you might run into errors. Always ensure the element exists in the DOM before you try to attach a listener to it!