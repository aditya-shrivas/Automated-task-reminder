# Automated Task Reminder Tracking Application

A Spring Boot–based REST API application that helps manage tasks with automated email reminders.  
The system allows users to create, update, complete, schedule reminders for tasks, generate reports, and export task data in CSV format.

---

## 🚀 Features

- Create, Read, Update, Delete (CRUD) tasks  
- Schedule automated email reminders for tasks  
- Mark tasks as completed  
- Task overview reporting (total, completed, pending, overdue)  
- Export all tasks as CSV  
- MySQL database integration  
- Email notifications using Gmail SMTP  
- RESTful API architecture  

---

## 🧱 Technology Stack

- Java 17  
- Spring Boot  
- Spring Data JPA  
- Spring Scheduler  
- Spring Mail  
- MySQL  
- HikariCP  
- Maven  

---

## 📌 API Endpoints

### 🔹 Task Management

| Method | Endpoint | Description |
|------|---------|-------------|
| POST | `/tasks/add` | Create a new task |
| GET | `/tasks/list` | Get all tasks |
| GET | `/tasks/{id}` | Get task by ID |
| PUT | `/tasks/update` | Update task |
| PUT | `/tasks/complete/{id}` | Mark task as completed |
| DELETE | `/tasks/delete/{id}` | Delete task |

---

### 🔹 Scheduler APIs

| Method | Endpoint | Description |
|------|---------|-------------|
| POST | `/schedule/set/{taskId}` | Schedule or reschedule reminder |
| GET | `/schedule/reminders/{taskId}` | Get reminder status |

---

### 🔹 Reports APIs

| Method | Endpoint | Description |
|------|---------|-------------|
| GET | `/reports/overview` | Get task summary overview |
| POST | `/reports/export` | Export all tasks as CSV |




