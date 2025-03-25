# ✨ Coding Standards

To maintain code quality, consistency, and best practices across all projects, follow these coding standards.

---

## 🏗 General Guidelines
- Follow the **KISS (Keep It Simple, Stupid)** principle.
- Follow **DRY (Don't Repeat Yourself)** to avoid redundancy.
- Write **clean, readable, and maintainable** code.
- Always include **meaningful comments** for complex logic.
- Use **proper indentation** and formatting.
- Avoid hardcoding values—use environment variables or config files.
- **Commit frequently** with clear, concise messages.

---

## 📌 Naming Conventions
### ✅ Variables & Functions
- Use **camelCase** for variables and functions.
- Names should be **descriptive and meaningful**.
- Boolean variables should be prefixed with `is`, `has`, or `should`.

```javascript
let isUserLoggedIn = false;
function calculateTotalPrice() {}
```

### ✅ Classes & Interfaces
- Use **PascalCase** for class and interface names.

```java
class UserProfile {}
interface DatabaseService {}
```

### ✅ Constants
- Use **UPPER_CASE_SNAKE_CASE** for constants.

```python
MAX_RETRY_ATTEMPTS = 3
```

---

## 📂 Project Structure
Each project should follow a structured format:

```
📂 project-name/
 ┣ 📂 src/       # Application source code
 ┣ 📂 tests/     # Unit and integration tests
 ┣ 📂 docs/      # Documentation
 ┣ 📜 .gitignore # Ignore unnecessary files
 ┣ 📜 README.md  # Project documentation
 ┣ 📜 LICENSE    # License agreement
 ┗ 📜 CHANGELOG.md # Version history
```

---

## 🔍 Code Formatting
- Use **4 spaces** for indentation (no tabs).
- Keep lines **under 80-120 characters**.
- Use **trailing commas** in multi-line objects/arrays.
- Ensure **consistent spacing** around operators and brackets.
- Use **single quotes (' ')** over double quotes (" ") unless necessary.

```javascript
const user = {
    name: 'John Doe',
    age: 30,
};
```

---

## ✅ Best Practices
### 🚀 Functions & Methods
- Functions should do **one thing only**.
- Keep functions **short** (max ~20 lines when possible).
- Avoid **deeply nested** if-else statements.
- Use **arrow functions** in JavaScript when applicable.

```javascript
const getFullName = (user) => `${user.firstName} ${user.lastName}`;
```

### 🚀 Error Handling
- Always **catch and handle errors** properly.
- Log errors in a structured way.

```python
try:
    result = fetch_data()
except Exception as e:
    print(f"Error: {str(e)}")
```

### 🚀 Security & Performance
- Never store **sensitive data** in source code.
- Sanitize all **user inputs**.
- Optimize database queries and API calls.
- Use **lazy loading** and caching when applicable.

---

## 🧪 Testing Guidelines
- Write **unit tests** for core functionalities.
- Follow **TDD (Test-Driven Development)** when possible.
- Use proper **test naming conventions**.
- Ensure **code coverage** meets the required threshold.

```python
def test_user_creation():
    user = User("John", "Doe")
    assert user.full_name == "John Doe"
```

---

## 📜 Git Commit Guidelines
- Use **present tense** and imperative mood.
- Keep messages **short and descriptive**.
- Reference issues using `#` (e.g., `#123`).

✅ Example:
```
feat: add authentication middleware
fix: resolve issue with login timeout (#45)
refactor: optimize database query for reports
```

---

💡 Following these standards will ensure **maintainability, readability, and efficiency** across all projects. Happy coding! 🚀
