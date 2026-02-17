# ⏳ Event Removal via Timeout

This project focuses on memory management and the DOM event lifecycle by using timers to disable interactions.

## 🚀 Key Concepts

### 1. Named Callback Functions
I learned that anonymous functions (direct arrow functions) are impossible to remove. Extracting logic into a constant (`handleClick`) is the essential step to allow full control over the event listener.

### 2. `removeEventListener` in Practice
This method requires two parameters identical to those used during creation: the event type (e.g., 'click') and the specific function reference.

### 3. Timers (`setTimeout`)
We use `setTimeout` to automate code cleanup, a common technique to prevent obsolete functions from consuming processing power after a certain period.

## 🛠️ How to Test
1. Click the button within the first 1.5 seconds; the text will appear in the console.
2. Wait for the "Ouvinte removido!" (Listener removed) log.
3. Click again; nothing will happen, proving the cleanup was successful.