# 🚀 Spacecraft Search Engine

A real-time search interface that filters a dataset of spacecraft using string manipulation and DOM management.

## 🚀 Key Features

### 1. Case-Insensitive & Trimmed Search
To ensure the best User Experience (UX), the search logic normalizes all inputs. By applying `.toLowerCase()` and `.trim()` to the query, the system successfully matches " luna " with "Luna E-1 No.1".

### 2. Functional Filtering
Instead of using complex loops, this project utilizes the modern `.filter()` array method. This creates a clean, declarative way to generate a subset of data based on the user's input.

### 3. Dynamic Rendering with Clean Slate
A crucial step in the `renderizar()` function is clearing the current list (`innerHTML = ""`) before injecting new results. This prevents "ghost" entries or duplicated lists every time a user types a character.

### 4. Default Parameter Strategy
The function is defined as `renderizar(query = "")`. This allows the application to show all spacecraft immediately when the page loads by calling the function without any arguments.

## 🛠️ Performance Note
While this approach works perfectly for small to medium datasets, filtering an entire array on every keystroke can become heavy for very large lists. In professional environments, techniques like **Debouncing** are often used to limit how many times the function runs.