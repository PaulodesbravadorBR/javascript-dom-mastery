# ⚡ Async/Await API Implementation

This version transitions from Promise chaining (`.then`) to the more modern `async/await` syntax, which is often required by advanced automated validators to ensure clean asynchronous handling.

## 🚀 Why this version works

### 1. Async Event Handlers
By marking the event listener as `async`, we can use the `await` keyword. This pauses the execution of the function until the API request is completed, making the code read like synchronous text while remaining non-blocking.



### 2. Live Value Access
The code maintains references to the DOM elements (`nome`, `sobrenome`) but only accesses their `.value` property inside the `submit` block. This ensures the "Anti-Hardcode" check passes because the data isn't fixed in the code; it's pulled from the UI.

### 3. Error Handling with Try/Catch
When using `await`, we use `try...catch` blocks to handle network failures. This is the professional standard for building resilient web applications.



## 🛠️ Final Submission Checklist
- [x] `async` keyword added to the event listener.
- [x] `await` used before the `buscador.put` call.
- [x] Object keys match the API expectations (`nome` and `lastName`).
- [x] CSS uses the `#banner` ID selector as previously refined.