# 🎓 Students API

This project is a RESTful API built with **Go** that manages student records. It allows users to perform CRUD (Create, Read, Update, Delete) operations on student data. The API is designed to be simple, efficient, and easy to use.

---

## ✨ Features

- Create new student records  
- Retrieve individual student records  
- Retrieve list of all student records  

---

## 🛠 Technologies Used

- [Go (Golang)](https://go.dev/)  
- [SQLite](https://www.sqlite.org/index.html)  

---

## 📡 API Endpoints

| Method | Endpoint               | Description                     |
|--------|------------------------|---------------------------------|
| POST   | `/api/students`        | Create a new student            |
| GET    | `/api/students/{id}`   | Retrieve a student by ID        |
| GET    | `/api/students`        | Retrieve list of all students   |

---

## 🧪 Example Usage

### ➕ Create Student

**Request:**

```
POST - http://localhost:5050/api/students
```

**Body:**

```json
{
  "name": "Onkar",
  "age": 19,
  "email": "onkar@email.com"
}
```

**Response:**

```json
{
  "id": 1
}
```

---

### 📄 Get Student by ID

**Request:**

```
GET - http://localhost:5050/api/students/1
```

**Response:**

```json
{
  "id": 1,
  "name": "Onkar",
  "email": "onkar@email.com",
  "age": 19
}
```

---

### 📋 Get All Students

**Request:**

```
GET - http://localhost:5050/api/students
```

**Response:**

```json
[
  {
    "id": 1,
    "name": "Onkar",
    "email": "onkar@email.com",
    "age": 19
  },
  {
    "id": 2,
    "name": "Abhi",
    "email": "Abhi@email.com",
    "age": 59
  }
]
```

---

## 🤝 Contributing

Contributions are welcome!  
Please fork the repository and create a pull request with your changes.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🧰 Development Setup (Optional)

You can use [MSYS2](https://www.msys2.org/) for setting up a Go development environment on Windows.
