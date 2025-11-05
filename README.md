# TaskGeniee - Full Stack Task Manager (MERN)

A comprehensive task management application built with the MERN stack, featuring role-based authentication, team collaboration, and real-time task tracking. Designed for efficient project and team workflow management.

## 🔗 Project Repositories

### 🎨 Frontend
- **Repository:** [Task-Manager-UI](https://github.com/parivallaljv/Task-Manager-UI)
- **Tech Stack:** React.js, Redux, Ant Design, Axios, JavaScript ES6+
- **Live Demo:** [taskygeniee.netlify.app](https://taskygeniee.netlify.app/signup)

### ⚙️ Backend
- **Repository:** [Task-Manager-server](https://github.com/parivallaljv/Task-Manager-server)
- **Tech Stack:** Node.js, Express.js, MongoDB, JWT, RESTful APIs

## ✨ Key Features

### Authentication & Authorization
- **JWT-based Authentication** - Secure token-based login/signup
- **Role-Based Access Control** - Admin and User roles with different permissions
- **Protected Routes** - Authorization middleware for secure endpoints

### Task Management
- **CRUD Operations** - Create, read, update, and delete tasks
- **Task Assignment** - Assign tasks to team members
- **Status Tracking** - Track task progress (To-Do, In Progress, Completed)
- **Priority Levels** - Set task priorities (High, Medium, Low)
- **Due Dates** - Add deadlines and track overdue tasks

### Team Collaboration
- **Multi-user Support** - Team members can collaborate on shared projects
- **Task Comments** - Discussion threads on individual tasks
- **Activity Feed** - Real-time updates on task changes
- **User Management** - Admin controls for adding/removing team members

### User Interface
- **Responsive Design** - Mobile-first approach using Ant Design components
- **Intuitive Dashboard** - Clean interface with task overview and statistics
- **Filters & Search** - Quick task filtering by status, priority, assignee
- **Dark/Light Mode** - Theme customization for user preference

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Installation

#### 1. Clone Repositories
```bash
# Frontend
git clone https://github.com/parivallaljv/Task-Manager-UI
cd Task-Manager-UI

# Backend
git clone https://github.com/parivallaljv/Task-Manager-server
cd Task-Manager-server
```

#### 2. Setup Backend
```bash
cd Task-Manager-server
npm install

# Create .env file
# Add: MONGO_URI, JWT_SECRET, PORT

npm start
# Server runs on http://localhost:5000
```

#### 3. Setup Frontend
```bash
cd Task-Manager-UI
npm install

# Update API endpoint in config if needed

npm start
# App runs on http://localhost:3000
```

## 🏗️ Architecture
```
┌─────────────────┐      REST API      ┌─────────────────┐
│   React.js      │◄──────────────────►│   Express.js    │
│   (Frontend)    │    HTTP/HTTPS      │   (Backend)     │
│                 │                    │                 │
│  - Redux Store  │                    │  - JWT Auth     │
│  - Ant Design   │                    │  - Middleware   │
│  - Axios        │                    │  - Controllers  │
└─────────────────┘                    └────────┬────────┘
                                                │
                                                ▼
                                       ┌─────────────────┐
                                       │    MongoDB      │
                                       │   (Database)    │
                                       │                 │
                                       │  - Users        │
                                       │  - Tasks        │
                                       │  - Projects     │
                                       └─────────────────┘
```

## 📦 Technology Stack

### Frontend
- **React.js** - UI library
- **Redux** - State management
- **Ant Design** - UI component library
- **Axios** - HTTP client
- **React Router** - Navigation

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication
- **bcrypt** - Password hashing

## 🔐 API Endpoints

### Authentication
```
POST   /api/auth/register    - User registration
POST   /api/auth/login       - User login
GET    /api/auth/me          - Get current user
```

### Tasks
```
GET    /api/tasks            - Get all tasks
POST   /api/tasks            - Create new task
GET    /api/tasks/:id        - Get single task
PUT    /api/tasks/:id        - Update task
DELETE /api/tasks/:id        - Delete task
```

### Users (Admin only)
```
GET    /api/users            - Get all users
PUT    /api/users/:id/role   - Update user role
DELETE /api/users/:id        - Delete user
```

## 🎯 Future Enhancements

- [ ] Real-time notifications using Socket.io
- [ ] File attachments for tasks
- [ ] Kanban board view
- [ ] Calendar integration
- [ ] Email notifications
- [ ] Advanced reporting and analytics
- [ ] Mobile app (React Native)
- [ ] Third-party integrations (Slack, Jira)

## 👨‍💻 Developer

**Parivallal J**
- GitHub: [@parivallaljv](https://github.com/parivallaljv)
- LinkedIn: [parivallal-j-developer](https://www.linkedin.com/in/parivallal-j-developer)
- Email: parivallalj56@gmail.com

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Ant Design for the beautiful UI components
- MongoDB for the flexible database solution
- The MERN community for excellent documentation

---

⭐ **Star this repo if you found it helpful!**
