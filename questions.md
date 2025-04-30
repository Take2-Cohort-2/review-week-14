### 1. Identifying Components of a URI

Below is a sample URI:

```
https://www.example.com:8080/path/to/page?search=javascript#section
```

For the example URI above, identify each part that corresponds to the following
labels:

- **Path:**
- **Host:**
- **Query:**
- **Port:**

---

### 2. HTTP Methods

Match each operation with its corresponding HTTP method. Write your answers in the format `Operation: HTTP Method`.

Operations:
1. Retrieve a list of users
2. Create a new user account
3. Update a user's email address
4. Delete a user account
5. Get a specific user's profile
6. Replace all data for a user
7. Check if a user exists

Available HTTP Methods:
- GET
- POST
- PUT
- PATCH
- DELETE
- HEAD

Example format:
```
Operation: HTTP Method
```

Note: Some operations might use the same HTTP method. Make sure to explain your reasoning for each match.

---

### 3. Creating an Async Function to Fetch Data

Write an `async` function named `fetchData` that does the following:

- Uses the fetch API to request JSON data from:
`https://api.example.com/data`
- Awaits and parses the response using .json()
- Logs the data to the console if the request is successful

---

### 4. Understanding URLs and HTTP Methods

You are building a simple todo list app. For each task below, write the complete URL and HTTP method you would use:

1. Get all todo items
2. Add a new todo item
3. Mark a todo item as complete
4. Delete a todo item

Example format:
```
Operation: URL, HTTP Method
```

Example answer:
```
Get all todo items: https://api.todo.com/items, GET
```

Note: Use the base URL `https://api.todo.com` for all requests.

---

### 5. Understanding JSON and HTTP Headers

You are building a weather app that needs to fetch data from an API. The API returns weather information in JSON format.

1. Write a function that makes a request to `https://api.weather.com/forecast` with the following requirements:
   - Include the header `Accept: application/json` to specify we want JSON data
   - Include the header `Authorization: Bearer YOUR_API_KEY` for authentication
   - Use the appropriate HTTP method for retrieving data
   - Handle the response by checking if it's successful (status code 200)
   - Parse the JSON response

2. Explain why each header is necessary and what would happen if they were missing.

Example response format:
```json
{
  "temperature": 22,
  "conditions": "sunny",
  "humidity": 65
}
```

---

### 5. Understanding the Order of Console Logs in Async JavaScript

You are given the following JavaScript code snippet:

```javascript
const fetchData = async () => {
  console.log("A");
  const response = await fetch("https://api.example.com/data");
  console.log("B");
};

button.addEventListener("click", () => {
  fetchData();
  console.log("C");
});

console.log("D");
```

**Instructions:**

🔍 Instructions:
What order will the console output appear in if the button is clicked once after the page loads?
(Choose from the letters A, B, C, and D.)

Explain why the logs appear in that order.
Your explanation should reference concepts like:
- async/await
- How asynchronous code behaves
❗ Note: Simply writing the order of the console logs is not enough — full marks require a good explanation based on JavaScript's asynchronous behavior.