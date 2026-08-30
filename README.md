# Employee Management System — Frontend Made with ❤️‍🔥 by Loki

A responsive **Employee Management System frontend** built with **React JS**, integrated with a Spring Boot REST API.

The application provides authentication, role-based UI, employee management, search with debounce, Redux state management, and responsive Bootstrap-based UI.

## 🚀 Tech Stack

* React JS
* JavaScript (ES6+)
* React Router DOM
* Redux Toolkit
* React Redux
* Axios
* Bootstrap 5
* Custom CSS

## ✨ Features

### 🔐 Authentication

* Login page
* JWT-based authentication
* JWT token stored in localStorage
* Redux authentication state
* Automatic JWT attachment using Axios interceptor
* Automatic redirect to login when token is unauthorized
* Logout functionality

### 🛡️ Role-Based UI

#### USER

* View employees
* Search employees
* Add/Edit/Delete buttons are hidden

#### ADMIN

* View employees
* Search employees
* Add employee
* Edit employee
* Delete employee

### 👨‍💼 Employee Management

* Employee list
* Add employee
* Edit employee
* Delete employee
* Employee search
* Department selection
* Salary display
* Delete confirmation
* Loading states
* Error handling

### ⚡ React Features

* Functional components
* React Hooks
* React Router
* Redux Toolkit
* Axios
* Axios request interceptor
* Axios response interceptor
* Debounce search
* Dynamic route parameters
* Protected API integration
* localStorage

### 🎨 UI

* Bootstrap 5
* Responsive layout
* Responsive employee table
* Clean login page
* Dashboard layout
* Custom CSS
* Loading spinner
* Alert messages
* Mobile-friendly design

---

## 🏗️ Folder Structure

```text
src/
│
├── components/
│
├── pages/
│   ├── Login.js
│   ├── Dashboard.js
│   └── EmployeeForm.js
│
├── redux/
│   ├── store.js
│   └── authSlice.js
│
├── services/
│   └── api.js
│
├── utils/
│   └── debounce.js
│
├── App.js
├── index.js
└── index.css
```

## 🔄 Application Flow

### Login

```text
Login Page
    ↓
Axios
    ↓
Spring Boot REST API
    ↓
JWT Token
    ↓
Redux Store
    ↓
localStorage
    ↓
Dashboard
```

### API Request

```text
React Component
      ↓
Axios
      ↓
Request Interceptor
      ↓
Bearer JWT Token
      ↓
Spring Boot REST API
      ↓
Response
      ↓
React UI
```

---

## 🔍 Debounced Search

Employee search uses a custom debounce utility to avoid sending an API request for every keystroke.

```text
User types
    ↓
Wait 500ms
    ↓
No new input?
    ↓
API request
```

This reduces unnecessary API calls and improves frontend performance.

---

## 🧭 Routes

| Route                 | Page               | Access        |
| --------------------- | ------------------ | ------------- |
| `/login`              | Login              | Public        |
| `/dashboard`          | Employee Dashboard | Authenticated |
| `/employees/add`      | Add Employee       | ADMIN         |
| `/employees/edit/:id` | Edit Employee      | ADMIN         |

---

## 🔌 API Configuration

The frontend communicates with the Spring Boot backend through Axios.

Default API URL:

```text
http://localhost:8080/api
```

Configured in:

```text
src/services/api.js
```

JWT authentication is automatically added to protected requests:

```text
Authorization: Bearer <JWT_TOKEN>
```

---

## 📦 Installation

Clone the repository:

```bash
git clone <your-repository-url>
```

Navigate to the project:

```bash
cd employee-frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm start
```

Application runs at:

```text
http://localhost:3000
```

---

## 🔗 Backend

This frontend requires the Employee Management Spring Boot REST API to be running on:

```text
http://localhost:8080
```

Make sure the backend is started before testing login and employee operations.

---

## 🧪 User Roles

### USER

```text
Login
   ↓
Dashboard
   ↓
View Employees
   ↓
Search Employees
```

### ADMIN

```text
Login
   ↓
Dashboard
   ↓
View Employees
   ↓
Add / Edit / Delete Employees
```

---

## 📸 Screenshots

Add project screenshots here:

```text
screenshots/
├── login.png
├── dashboard.png
├── add-employee.png
└── edit-employee.png
```

Example:

![Login Page](screenshots/login.png)

![Dashboard](screenshots/dashboard.png)

---

## 🎯 Key Learning & Implementation

This project demonstrates practical implementation of:

* React JS
* JavaScript ES6+
* React Hooks
* React Router
* Redux Toolkit
* Axios
* JWT authentication handling
* Role-based UI rendering
* REST API integration
* Axios interceptors
* Debouncing
* localStorage
* Responsive Bootstrap UI
* CRUD interface
* Form handling
* Error handling
* Loading states

---

## 👨‍💻 Author

**Loki**

Built with ❤️ using React JS.
