# WhatsApp Clone (Full-Stack)

A full-stack, real-time messaging application inspired by WhatsApp. This project allows users to sign up, search for friends, create 1-on-1 private chats, and form group chats—all with instant, real-time message delivery.

## 🚀 Technologies Used

### Frontend
* **React.js** - UI components and routing
* **Redux Thunk** - Global state management
* **Tailwind CSS** - Styling and responsive design
* **SockJS & StompJS** - WebSocket client for real-time messaging

### Backend
* **Java & Spring Boot** - REST APIs and WebSocket server
* **Spring Security & JWT** - Stateless, secure authentication
* **Hibernate / Spring Data JPA** - Database ORM
* **MySQL** - Relational database management

---

## ✨ Features

* **JWT Authentication:** Secure Sign up and Login system using JSON Web Tokens.
* **Real-time Messaging:** Instant message delivery using WebSockets (STOMP protocol). No page refreshes needed!
* **Global User Search:** Find friends by searching their partial name or email address.
* **1-on-1 Chats:** Start private, secure conversations with other registered users.
* **Group Chats:** Create groups with multiple participants.

---

## 💻 Getting Started (Local Setup)

Follow these steps to clone and run the project on your local machine.

### Prerequisites
Make sure you have the following installed:
* **Java 17** or higher
* **Node.js**
* **MySQL Server**

### 1. Clone the Repository
Open your terminal and run:
```bash
git clone <your-github-repository-url>
cd Whatsapp-clone
```

### 2. Database Configuration
Before running the backend, you need to prepare your local database.
1. Open MySQL (via Workbench or terminal) and create a new database:
   ```sql
   CREATE DATABASE whatsapp_db;
   ```
2. Open `backend/src/main/resources/application.properties` in your code editor.
3. Update the database credentials to match your local MySQL setup (if they are different):
   ```properties
   spring.datasource.username=root
   spring.datasource.password=your_local_password
   ```
   *(Note: The code currently defaults to username `root` and password `@R1a2h3u4l5` if no environment variables are set).*

### 3. Run the Backend
Open a terminal in the `backend` folder and start the Spring Boot server:
```bash
cd backend
./mvnw spring-boot:run
```
*The server will start on `http://localhost:8080`.*

### 4. Run the Frontend
Open a new, separate terminal in the `frontend` folder, install the dependencies, and start the React app:
```bash
cd frontend
npm install
npm start
```
*The React app will open in your browser at `http://localhost:3000`.*
