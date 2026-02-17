# ⏳ UI Feedback: Loading States (Exercise 44)

In modern web development, providing immediate feedback is crucial. If a user clicks a button and nothing changes visually, they might click it multiple times or think the app is broken.

### ⚙️ The Logic:
1. **Targeting**: We identify the button via `document.querySelector("#meu-botao")`.
2. **Listening**: We wait for the `"click"` event.
3. **Transforming**: Once clicked, we access the `.textContent` property to change the label from "Obter temperatura" to "Carregando...".



### 🛠️ Key Technical Concept: textContent
The `.textContent` property is the safest and most efficient way to change the text inside an element. Unlike `innerHTML`, it does not parse the content as HTML, which prevents security risks and is slightly faster for the browser to render.

### ✅ Result:
When the user clicks the button, the text changes instantly. In a real-world scenario, this would usually be followed by a `fetch()` request to an API, and the text would change back to "Success" or "Try Again" once the data arrives.