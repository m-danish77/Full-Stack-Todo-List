# Full Stack To-Do List project

A sleek, modern, and robust Full-Stack Task Management application built with the (MongoDB, Express, Node.js) and a high-performance vanilla JavaScript frontend styled with **Tailwind CSS**.

## 🎨 Features
- **Full CRUD Functionality**: Create, Read, Update, and Delete tasks seamlessly.
- **Contextual In-place Editing**: Update task names directly within the list without distracting modals.
- **Toggle Completion**: Mark tasks as done with a single click, featuring immediate UI feedback.
- **Bulk Cleanup**: One-click "Clear Completed" to purge finished tasks from the database.
- **Cyber-Minimalist UI**: A premium dark-mode aesthetic with glassmorphism effects and responsive design.
- **RESTful API**: A clean backend architecture following industry-standard routing and controller patterns.

---

## 🛠️ Tech Stack

### Frontend
- **HTML5 & Tailwind CSS**: Semantic structure with modern, utility-first styling.
- **Vanilla JavaScript**: Lightweight, reactive DOM manipulation using the Fetch API.
- **Google Fonts (Inter)**: Clean typography for high readability.

### Backend
- **Node.js & Express**: Fast, unopinionated web framework for the API layer.
- **MongoDB & Mongoose**: NoSQL database with schema modeling for structured data storage.
- **CORS**: Cross-Origin Resource Sharing enabled for frontend-backend communication.

---

## 📂 Project Structure

```text
Full Stack To-Do-List/
├── backend/
│   ├── controllers/      # Logic for API endpoints (get,post,put,delete)
│   ├── models/           # Mongoose Schema (todoModel.js)
│   ├── routes/           # Express Router definitions (todoRoutes.js)
│   ├── server.js         # Entry point & Database connection
│   └── package.json
├── frontend/
│   ├── index.html        # Main UI structure
│   ├── script.js         # Frontend logic & API integration
│   └── assets/           # Icons and images (if any)
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) installed.
- [MongoDB](https://www.mongodb.com/try/download/community) installed and running locally (default: `localhost:27017`) or use MongoDB Atlas.

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-link>
   cd Full-Stack-To-Do-List
   ```

2. **Setup Backend**
   ```bash
   cd backend
   npm install
   ```
   *Create a `.env` file (optional) or ensure the connection string in `server.js` points to your local MongoDB.*

3. **Run the Application**
   - **Start Backend**:
     ```bash
     # Inside /backend
     node server.js
     ```
   - **Start Frontend**:
     Open `frontend/index.html` using **Live Server** in VS Code or run:
     ```bash
     cd ../frontend
     npx live-server
     ```

---

## 📡 API Reference

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/todos` | Retrieve all tasks |
| `POST` | `/api/todos` | Create a new task |
| `PUT` | `/api/todos/:id` | Update task text or status |
| `DELETE` | `/api/todos/:id` | Delete a specific task |
| `DELETE` | `/api/todos/clear` | Delete all completed tasks |

### Sample JSON Body (POST/PUT)
```json
{
  "task": "Build the next big thing",
  "completed": false
}
```

---

## 📝 Future Improvements
- [ ] User Authentication with JWT.
- [ ] Drag-and-drop task reordering.
- [ ] Dark/Light mode toggle.
- [ ] Categories/Labels for tasks.

## 🎓 Author
Developed to enhance my mainly Backend understanding and knowledge.
