# 🛡️ Form Validation with Blur Event

This project implements client-side interface validation to ensure that usernames meet the required minimum length.

## 🚀 Features

### 1. Immediate Visual Feedback
Using the `.success` and `.error` CSS classes, the input field dynamically changes its border color to green or red. This enhances User Experience (UX) by providing clear guidance without requiring a page reload.

### 2. DOM Class Manipulation
The use of `classList.add()` and `classList.remove()` ensures clean manipulation of element attributes, allowing CSS styling rules to be applied only when business logic conditions (minimum of 6 characters) are met.

### 3. Focus Events
The choice of the `blur` event is strategic: it waits for the user to finish interacting with the field before triggering validation, avoiding visual distractions during typing.

## 🛠️ Validation Criteria
* **Success**: Text length >= 6 characters.
* **Error**: Text length < 6 characters.