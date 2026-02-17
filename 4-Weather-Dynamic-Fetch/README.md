# 🌤️ Dynamic Weather Dashboard

This project is part of my JavaScript API Series. It demonstrates how to build a functional weather interface that communicates with a REST API to fetch climate data for different cities dynamically.

## 🛠️ Concepts Implemented
- **Fetch Wrapper Pattern**: A reusable `FetchWrapper` class that centralizes the `baseURL` and automates the `.json()` conversion.
- **Dynamic Endpoints**: Using template literals to build API paths based on user input (dropdown selection).
- **Asynchronous Logic**: Handling Promises to ensure the UI only updates after the data is successfully retrieved.
- **JSON Data Mining**: Accessing deeply nested properties within API response objects (`data.current.temperature`).

## 🚀 How it Works
The application uses a `<select>` element to trigger a change event. Once a city is chosen:
1. The `obterTemperatura` function is called with the city name.
2. The `FetchWrapper` instance targets the specific `.json` file for that city.
3. The UI is updated in real-time with the temperature retrieved from the server.

## 💻 Code Highlight: The Wrapper
```javascript
class EmpacotadorBusca {
    constructor(baseURL) {
        this.baseURL = baseURL;
    }

    get(endpoint) {
        return fetch(this.baseURL + endpoint)
            .then(response => response.json());
    }
}
