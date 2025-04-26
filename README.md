# System Control

System Control is a full-stack web application built with **React**, **Spring Boot (Java)**, **Spring Security (with JWT)**, and **MySQL** as the database.

## Features

### Authentication
- **User Registration**:  
  - Register with **name**, **email**, **password**, and **role** (`USER` or `ADMIN` — must be capitalized).
- **Login**:
  - Secure authentication using **Spring Security** and **JWT**.
- **Logout**:
  - Users can securely sign out from the system.

### User Roles
- **USER**:
  - View their **profile**.
  - Play two built-in games:
    - **Catch the Button**: A fast-paced game where players must click a moving button as many times as possible within a timed round.
    - **Tic Tac Toe**: A classic 3x3 game everyone knows and loves.
  - Access to their own dashboard only.

- **ADMIN**:
  - All the capabilities of a **USER**.
  - **User Management Panel**:
    - Perform **full CRUD (Create, Read, Update, Delete)** operations on all registered users.
    - View user list, update user details, and remove users as needed.

### Database
- All users and their information are stored securely in a **MySQL** database.

## Technologies Used

| Frontend | Backend | Database | Security |
|:--------:|:-------:|:--------:|:--------:|
| React    | Spring Boot | MySQL | Spring Security + JWT |

## How to Run the Project

### Backend (Spring Boot)
1. Clone the project.
2. Set up your MySQL database and update `application.properties` with your DB credentials.
3. Run the Spring Boot application.
4. The backend will be available at `http://localhost:8080/`.

### Frontend (React)
1. Navigate to the React project folder.
2. Install dependencies:
    ```bash
    npm install
    ```
3. Start the development server:
    ```bash
    npm start
    ```
4. The frontend will be available at `http://localhost:5173/`.

## Notes
- Roles must be entered as `USER` or `ADMIN` during registration (case-sensitive).
- JWT tokens are used for authentication and must be included in headers when making protected requests.

## Future Improvements
- Add game score tracking and leaderboards.
- Add pagination for user management.
- Add password reset functionality.

## Author

Created with ❤️ by Qiydaar W.
