# Real-Time Chat Application

A full-stack real-time chat application built with React and Spring Boot, featuring WebSocket for instant messaging and MongoDB for data persistence.

## 🚀 Tech Stack

### Frontend
- **React** (v18.3.1)
- **Vite** (Build tool)
- **Tailwind CSS** (Styling)
- **React Router** (v7.6.3) for navigation
- **Axios** (v1.7.9) for HTTP requests
- **@stomp/stompjs** (v7.0.0) for WebSocket communication
- **React Hot Toast** for notifications

### Backend
- **Spring Boot** (v3.4.0)
- **Spring WebSocket** for real-time communication
- **Spring Data MongoDB** for database operations
- **MongoDB** (NoSQL database)
- **Java 21**

## 🏃‍♂️ How to Run the Project

### Prerequisites
- Node.js (v18+)
- Java 21 JDK
- MongoDB (local instance or MongoDB Atlas)
- Maven (for backend build)

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd chat-app-backend
   ```
2. Configure MongoDB connection in `application.properties`
3. Build and run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```
   The backend will start on `http://localhost:8080`

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd front-chat
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
   The frontend will be available at `http://localhost:5173`

## 🏗️ Project Structure

### Frontend Structure
```
front-chat/
├── src/
│   ├── components/     # Reusable UI components
│   ├── config/         # Configuration files (routes, API endpoints)
│   ├── context/        # React context providers
│   ├── App.jsx         # Main application component
│   └── main.jsx        # Application entry point
```

### Backend Structure
```
chat-app-backend/
├── src/main/java/com/substring/chat/
│   ├── config/         # Configuration classes (WebSocket, Security)
│   ├── controller/     # REST controllers
│   ├── model/          # Data models
│   ├── repository/     # MongoDB repositories
│   ├── service/        # Business logic
│   └── ChatAppBackendApplication.java  # Main application class
```
