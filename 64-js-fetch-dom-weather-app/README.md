# 🌤️ Dynamic Weather API Project

This project demonstrates the integration between DOM events, asynchronous data fetching, and object-oriented encapsulation using a Fetch wrapper.

## 🚀 Key Learning Objectives

### 1. Asynchronous Flow with Fetch
The application uses a `GET` request to retrieve real-time weather data. By using `.then()`, we ensure the UI only updates once the data has successfully arrived from the Firebase server.



### 2. The Power of the Wrapper Class
Instead of writing the full `fetch()` boilerplate every time, we use `PacoteBuscador`. This abstraction handles:
- Base URL concatenation.
- Automatic JSON parsing with `response.json()`.
- Error handling foundations for CRUD operations.

### 3. Change Event Handling
Unlike a search input where we use `input`, for a `<select>` element, the `change` event is the most efficient. It triggers only when the user confirms a new selection from the list.

### 4. Dynamic Endpoints
The endpoint is constructed dynamically: `${cidade}.json`. This allows a single function to handle an infinite number of cities, provided the API follows a consistent naming convention.

## 🛠️ Requirements Checklist
- [x] Listen for city selection changes.
- [x] Fetch data from the specific city endpoint.
- [x] Extract the `temperature` property from the JSON response.
- [x] Update the `#resultado-tempo` element with the exact required string.