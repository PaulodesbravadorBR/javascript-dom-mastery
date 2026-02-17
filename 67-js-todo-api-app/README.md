# 📝 Task Manager API Integration

A fully dynamic To-Do application that synchronizes local UI state with a shared REST API using modern JavaScript.

## 🚀 Features & Technical Logic

### 1. Dynamic List Rendering
Instead of static HTML, the app uses `API.get("/todos")` to fetch data. We use `insertAdjacentHTML` combined with template literals to inject the task cards into the DOM. Crucially, `listaAfazeres.innerHTML = ""` is called before rendering to prevent task duplication.



### 2. State Synchronization
When a user adds a task, the following lifecycle occurs:
1. **Intercept**: Prevent the page from reloading.
2. **Payload**: Extract `value` from inputs.
3. **Persist**: Send a `PUT` request to the server.
4. **Refresh**: Trigger `obterAfazeres()` again to show the updated list from the server's perspective.

### 3. UX Improvements (Optional Requirements)
- **Button Debouncing**: The "Adicionar" button is disabled during the fetch request (`botaoAdicionar.disabled = true`). This prevents "double-submit" bugs where a user clicks twice and creates duplicate entries.
- **Input Clearing**: The task title field is reset only after a successful API response.



## 🛠️ API Constraints Checklist
- [x] Base URL correctly instantiated with `PacoteBuscador`.
- [x] Tasks formatted as `[category] title`.
- [x] Supported titles only (e.g., 'walk the dog', 'feed the cat').
- [x] Correct HTML structure used: `<li><div class="card">...</div></li>`.