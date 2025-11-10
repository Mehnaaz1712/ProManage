# 🧩 ProManage

> A collaborative workspace for modern teams — streamline your projects, track tasks, analyze performance, and stay organized with real-time collaboration.

---

## 🚀 Live Demo
👉 [https://pro-manage-zeta.vercel.app/](https://pro-manage-zeta.vercel.app/)

---

## 🖥️ Overview

**ProManage** is a full-stack **Project Management Web App** that allows teams to create projects, assign tasks, track progress, view analytics, and collaborate seamlessly in real-time.  
It integrates **Clerk Authentication**, **Redux Toolkit**, and **Prisma ORM**, offering a clean UI powered by **TailwindCSS** and advanced analytics with **Recharts**.

---

## 🌟 Features

✅ User Authentication using Clerk  
✅ Workspace & Team Management  
✅ Project Creation with Priority & Status tracking  
✅ Task Management with filters, CRUD, and analytics  
✅ Real-time Comments on tasks  
✅ Project Analytics Dashboard  
✅ Invite Members via Email  
✅ Dark / Light Mode Support  
✅ Fully Responsive UI (Desktop + Mobile)  

---

## 🛠️ Tech Stack

### **Frontend**
- React 18
- Redux Toolkit
- React Router DOM
- TailwindCSS
- Recharts
- Clerk Authentication

### **Backend**
- Node.js
- Express.js
- Prisma ORM
- PostgreSQL / MySQL
- JWT Authentication
- Nodemailer (for invites)

---

## ⚙️ Installation and Setup

### 1️⃣ Clone the Repository

### 2️⃣ Install Dependencies

#### For frontend:

```bash
cd client
npm install
```

#### For backend:

```bash
cd server
npm install
```

### 3️⃣ Setup Environment Variables

Create `.env` files in both the **frontend** and **backend** directories.

#### 🌐 Frontend `.env`

```
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
VITE_API_URL=http://localhost:5000
```

#### 🗄️ Backend `.env`

```
DATABASE_URL=your_database_connection_string
JWT_SECRET=your_jwt_secret
CLERK_SECRET_KEY=your_clerk_secret_key
EMAIL_USER=your_email@example.com
EMAIL_PASS=your_email_password
```

---

## 🧩 Folder Structure

```
ProManage/
├── client/                   # React frontend
│   ├── src/
│   │   ├── components/       # Reusable UI components
│   │   ├── pages/            # Page-level components (Dashboard, Team, etc.)
│   │   ├── app/              # Redux store setup
│   │   ├── features/         # Redux slices (theme, workspace)
│   │   ├── configs/          # API configuration
│   │   ├── assets/           # Icons, images, constants
│   │   ├── App.jsx           # Main routes
│   │   └── main.jsx          # Entry point
│   └── package.json
│
├── server/                   # Node.js backend
│   ├── controllers/          # API logic
│   ├── routes/               # Express routes
│   ├── prisma/               # Prisma schema & migrations
│   ├── utils/                # Helper functions (mailer, token)
│   ├── server.js             # App entry point
│   └── package.json
│
└── README.md
```

---

## 🚀 Running the App

### 🖥️ Run Backend

```bash
cd server
npm run dev
```

### 💻 Run Frontend

```bash
cd client
npm run dev
```

Now open 👉 **[http://localhost:5173/](http://localhost:5173/)** to view the app.

---

## 📊 Key Modules

### 🔐 Authentication

* Clerk handles secure user sign-in, sign-up, and team management.
* JWT & Clerk tokens secure all API routes.

### 📁 Workspaces

* Each workspace contains multiple projects and members.
* Workspace data fetched via Redux slice.

### 📊 Projects

* Create, edit, delete projects with status & priority.
* Visualize analytics using **Recharts**.

### 🧾 Tasks

* CRUD tasks with type, status, and assignee.
* Filter, sort, and analyze task distribution.
* Real-time commenting and discussion threads.

---

## 🌈 Screenshots

Dashboard
<img width="1908" height="912" alt="Dashboard ProManage" src="https://github.com/user-attachments/assets/6709b72e-2af9-4e61-9675-94a228185096" />
Projects
<img width="1858" height="722" alt="Projects ProManage" src="https://github.com/user-attachments/assets/cc970f96-cb2c-4f42-b09c-c072526525e5" />
Task Details
<img width="1803" height="800" alt="Task Details ProManage" src="https://github.com/user-attachments/assets/15777342-f7c2-493a-ad81-c46b4a6ace53" />

---

## 🌐 API Endpoints (Overview)

| Method | Endpoint                      | Description                   |
| ------ | ----------------------------- | ----------------------------- |
| POST   | `/api/projects`               | Create new project            |
| GET    | `/api/projects/:id`           | Get project details           |
| POST   | `/api/tasks`                  | Create new task               |
| PUT    | `/api/tasks/:id`              | Update task status/details    |
| POST   | `/api/comments`               | Add comment on task           |
| GET    | `/api/comments/:taskId`       | Fetch all comments for a task |
| POST   | `/api/projects/:id/addMember` | Add member to project         |

---

## 🧑‍💻 Developer Notes

* Use `redux-devtools-extension` for debugging store.
* Update `vite.config.js` if deploying on custom domains.
* For Clerk roles and org handling, use **useOrganizationList()** hooks.

---

## 🧱 Deployment

You can deploy using:

* **Frontend:** [Vercel](https://vercel.com) or [Netlify](https://netlify.com)
* **Backend:** [Render](https://render.com), [Railway](https://railway.app), or [AWS EC2]
* **Database:** [NeonDB](https://neon.tech) or [Supabase](https://supabase.io)

Make sure to update the `VITE_API_URL` in your frontend `.env` file after deployment.

---

## 🤝 Contribution

1. Fork the repo
2. Create a new branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m "Added new feature"`
4. Push to the branch: `git push origin feature-name`
5. Submit a Pull Request 🚀

---

## 📝 License

This project is licensed under the **MIT License**.
You are free to modify and distribute it with attribution.

---

## 👩‍💻 Author

**Mehnaaz Ansari**
B.Tech CSE (AI) @ IGDTUW
📧 [mehnaazansari3@gmail.com](mailto:mehnaazansari3@gmail.com)
🌐 [LinkedIn](https://www.linkedin.com/in/mehnaaz-ansari) | [GitHub](https://github.com/Mehnaaz1712)

