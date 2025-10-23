# Task Management Application

## 🚀 Introduction

The **Task Management Application** is a web-based productivity tool designed to help users organize, track, and manage tasks efficiently. Built using **React 19, Firebase, TailwindCSS, and React Query**, this app provides a seamless user experience with drag-and-drop functionality, real-time updates, and cloud storage.

## 📑 Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Environment Variables](#-environment-variables)
- [Dependencies](#-dependencies)
- [Development](#-development)
- [Build and Deployment](#-build-and-deployment)
- [Contributors](#-contributors)
- [License](#-license)

## ✨ Features

- 📝 **Task Management** – Create, update, and delete tasks.
- 📂 **Drag and Drop Support** – Organize tasks effortlessly.
- 🔥 **Firebase Integration** – Real-time data syncing.
- 🎨 **TailwindCSS & DaisyUI** – Beautiful and responsive UI.
- 🔍 **Search & Sort** – Quickly find and sort tasks.
- 🔔 **Notifications** – Get real-time updates.
- 🌐 **Deployed on Vercel** – Fast and scalable hosting.

## 🛠 Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**

   ```sh
   git clone https://github.com/alaminislam34/Task-Management-Application.git
   cd task-management-app
   ```

2. **Install dependencies:**

   ```sh
   npm install
   ```

3. **Set up environment variables:**  
   Create a `.env` file in the root directory and add the following:

   ```env
   VITE_apiKey=your-api-key
   VITE_authDomain=your-auth-domain
   VITE_projectId=your-project-id
   VITE_storageBucket=your-storage-bucket
   VITE_messagingSenderId=your-messaging-sender-id
   VITE_appId=your-app-id
   VITE_URL=your-app-url
   ```

4. **Run the development server:**
   ```sh
   npm run dev
   ```

## 🎮 Usage

1. Open the app in your browser at `http://localhost:5173/`.
2. Sign in using Firebase authentication.
3. Add, edit, or delete tasks.
4. Drag and drop tasks to change their order.
5. Get real-time updates and notifications.

## 🔑 Environment Variables

Ensure you configure the following variables in your `.env` file:

| Variable                 | Description                   |
| ------------------------ | ----------------------------- |
| `VITE_apiKey`            | Firebase API Key              |
| `VITE_authDomain`        | Firebase Auth Domain          |
| `VITE_projectId`         | Firebase Project ID           |
| `VITE_storageBucket`     | Firebase Storage Bucket       |
| `VITE_messagingSenderId` | Firebase Messaging Sender ID  |
| `VITE_appId`             | Firebase App ID               |
| `VITE_URL`               | Deployment URL (e.g., Vercel) |

## 📦 Dependencies

This project uses the following dependencies:

### ✅ Main Dependencies:

- **React 19** – Frontend library
- **Firebase** – Backend services
- **React Query** – Data fetching and state management
- **React Router** – Routing management
- **TailwindCSS & DaisyUI** – UI framework
- **Axios** – HTTP requests
- **React Hook Form** – Form management
- **React Toastify** – Notifications
- **AOS** – Animations
- **LocalForage** – Local storage handling

### 🛠 Dev Dependencies:

- **Vite** – Build tool
- **ESLint** – Linter for code quality
- **DaisyUI** – UI components
- **Types for React & ReactDOM** – TypeScript support

## 🏗 Development

- Start the development server:
  ```sh
  npm run dev
  ```
- Run the linter:
  ```sh
  npm run lint
  ```
- Build the project:
  ```sh
  npm run build
  ```
- Preview production build:
  ```sh
  npm run preview
  ```

## 🚀 Build and Deployment

The app is deployed on **Vercel**. To deploy manually:

1. Build the project:
   ```sh
   npm run build
   ```
2. Deploy to Vercel:
   ```sh
   vercel --prod
   ```

## 👥 Contributors

- **MD Al Amin Islam** – [GitHub](https://github.com/alaminislam34)

## 📜 License

This project is licensed under the **MIT License**.

---

Enjoy using **Task Management Application**! 🚀🎯

### Let me know if you need any modifications! 🚀
