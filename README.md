# codingbatjs-data

A public dataset of beginner-friendly JavaScript coding problems inspired by CodingBat.  
Served via static files on GitHub Pages — easy for any frontend or backend to consume.

---

## 📚 Overview

This repository hosts:

- `topics.json`: All problem topics and metadata.
- `/problems/{topicId}.json`: The full problem set for each topic.

All files are accessible via HTTP and can be fetched directly in your apps or projects.

---

## 🛰️ API Endpoints

### 📋 List All Topics

- **URL:** [`/topics.json`](https://mirzamitdinovs.github.io/codingbatjs-data/topics.json)
- **Description:** Returns all problem topics with metadata.

#### Example

```http
GET https://mirzamitdinovs.github.io/codingbatjs-data/topics.json
```

---

### 📦 Get All Problems for a Topic

For each topic listed in `topics.json`, fetch the full problem set at:

- **URL:** `/problems/{topicId}.json`

#### Example Endpoints

| Topic       | Endpoint URL                                                                                             |
| ----------- | -------------------------------------------------------------------------------------------------------- |
| Warmup-1    | [problems/warmup-1.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/warmup-1.json)       |
| String-1    | [problems/string-1.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/string-1.json)       |
| Array-1     | [problems/array-1.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/array-1.json)         |
| Logic-1     | [problems/logic-1.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/logic-1.json)         |
| String-2    | [problems/string-2.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/string-2.json)       |
| Array-2     | [problems/array-2.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/array-2.json)         |
| Logic-2     | [problems/logic-2.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/logic-2.json)         |
| Recursion-1 | [problems/recursion-1.json](https://mirzamitdinovs.github.io/codingbatjs-data/problems/recursion-1.json) |

---

## 🔗 Complete API List

```json
[
  "https://mirzamitdinovs.github.io/codingbatjs-data/topics.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/warmup-1.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/string-1.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/array-1.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/logic-1.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/string-2.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/array-2.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/logic-2.json",
  "https://mirzamitdinovs.github.io/codingbatjs-data/problems/recursion-1.json"
]
```

---

## 🚀 Usage Example

**Fetch all topics:**

```js
fetch('https://mirzamitdinovs.github.io/codingbatjs-data/topics.json')
  .then((res) => res.json())
  .then((data) => console.log(data));
```

**Fetch all 'Warmup-1' problems:**

```js
fetch(
  'https://mirzamitdinovs.github.io/codingbatjs-data/problems/warmup-1.json',
)
  .then((res) => res.json())
  .then((problems) => console.log(problems));
```

---

## 📝 Notes

- All endpoints are public and served as static files via GitHub Pages.
- Data can be used for coding platforms, educational apps, or personal projects.
- Contributions are welcome!

---

## 📢 License

MIT License (or specify your own)

---
