# 🔍 Inspecting the Event Object (Exercise 48)

Every time an interaction happens, the browser doesn't just run your code; it hands you a "report" of exactly how that interaction went down.

### 🛠️ What is the `event` object?
It is the first argument passed to any event listener callback. While we often ignore it for simple clicks, it contains vital information for advanced UI logic.



### 📊 Common Properties found in Click Events:
| Property | Description |
| :--- | :--- |
| `clientX` / `clientY` | The coordinates of the mouse relative to the browser window. |
| `timeStamp` | The exact millisecond the event occurred. |
| `shiftKey` | A boolean (true/false) if the Shift key was held down. |
| `currentTarget` | **(Most Important)** The element that the event listener is attached to. |

### 💡 Practice Tip:
Open your browser's Developer Tools (**F12** or **Right-Click > Inspect**), go to the **Console** tab, and click the button. Expand the arrow next to `PointerEvent` to see the dozens of properties the browser tracks for a single click!