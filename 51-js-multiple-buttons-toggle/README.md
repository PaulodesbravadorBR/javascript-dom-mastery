# 🔘 Multiple Elements Interaction (Exercise 51)

In this project, we scale up our interactivity. Instead of one button, we manage an entire group using a clean, dry (Don't Repeat Yourself) approach.

### ⚙️ How it works:
1. **The NodeList**: `querySelectorAll(".botao")` grabs every button on the page and stores them in a collection.
2. **The Loop**: We use `.forEach()` to visit every button in that collection exactly once.
3. **The Listener**: Inside the loop, we attach an `addEventListener`. Even though the code looks the same for all of them, the browser keeps track of which button belongs to which listener.
4. **Independent Toggling**: Because we use `evento.currentTarget`, clicking "Botão #2" only affects "Botão #2".



### 🛠️ Key Technical Concept: NodeList vs. Array
While `querySelectorAll` returns a `NodeList` (which looks like an array), it's important to remember that in older browsers, NodeLists didn't always support `.forEach()`. In modern JavaScript (ES6+), however, this is the standard way to handle multiple UI elements at once.

### ✅ Result:
Each button now functions as an independent toggle switch, allowing for complex UI states like selecting multiple items in a list.