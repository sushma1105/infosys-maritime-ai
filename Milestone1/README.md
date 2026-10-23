# Agentic AI for Maritime Freight Pricing and Route Optimization

## Milestone 1: Secure Authentication System

### 1. Project Overview

**Agentic AI for Maritime Freight Pricing and Route Optimization** aims to support maritime freight decision-making through AI-driven pricing analysis and route optimization.

Milestone 1 focuses on developing a secure, user-friendly authentication system that serves as the entry point for the larger application. It provides user registration, login, password recovery, session management, and separate administrator access.

### 2. Objectives

- Develop a Streamlit-based authentication interface.
- Implement secure user registration and login.
- Validate user inputs, email addresses, and passwords.
- Support password recovery through security questions and email OTP verification.
- Implement JWT-based session management.
- Provide a protected user dashboard and logout functionality.
- Create a separate administrator login and dashboard to view registered usernames and email addresses.

### 3. Features Implemented

**User Authentication**
- User signup and login.
- Required-field and email validation.
- Password hashing using bcrypt.
- Password policy enforcement.
- JWT-based session management with token expiration.

**Password Recovery**
- Security-question-based password recovery.
- Email OTP verification for password recovery.

**User Dashboard**
- Protected dashboard accessible after successful authentication.
- User account information.
- Logout functionality.

**Administrator Dashboard**
- Separate administrator authentication.
- Display of registered usernames and email addresses.
- Restricted access to administrative information.

**User Interface**
- Maritime-themed interface using navy blue, ocean blue, and teal colors.
- Responsive, clearly structured authentication pages and dashboards.

### 4. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application logic |
| Streamlit | User interface and web application |
| SQLite | User data storage |
| bcrypt | Password hashing |
| JWT | Authentication and session tokens |
| Email OTP | Password recovery verification |
| Google Colab | Development and execution environment |
| ngrok | External access to the running application |

### 5. Project Structure

```text
Milestone1/
├── Milestone1_Maritime_Auth.ipynb
├── README.md
└── screenshots/
    ├── login.png
    ├── signup.png
    ├── forgot-security-question.png
    ├── forgot-email-otp.png
    ├── user-dashboard.png
    └── admin-dashboard.png
```

### 6. Execution Instructions

The application is designed to run in Google Colab.

1. Open `Milestone1_Maritime_Auth.ipynb` in Google Colab.
2. Configure the required credentials and secrets using Colab Secrets.
3. Ensure the notebook has permission to access the required secrets.
4. Install the required Python dependencies as specified in the notebook.
5. Run the notebook cells in the prescribed order.
6. Configure email delivery using the required Gmail credentials and an app password, if applicable.
7. Launch the Streamlit application and use the generated ngrok URL to access it.

**Security note:** Store sensitive credentials in Colab Secrets. Never commit passwords, email app passwords, JWT signing secrets, or ngrok authentication tokens to the repository.

### 7. Configuration

The application requires appropriate configuration for authentication, administrator access, and email-based OTP verification.

Configure the secret names and values expected by the notebook before running the application. Use strong, unique credentials and avoid exposing sensitive information in screenshots or logs.

### 8. Screenshots

Screenshots demonstrating the completed authentication workflow are available in the `screenshots/` directory.

- Login page
- Signup page
- Security-question password recovery
- Email OTP password recovery
- User dashboard
- Administrator dashboard

### 9. Testing

The milestone is intended to cover the following checks:

- Successful user registration and login.
- Required-field and invalid-email validation.
- Password policy enforcement.
- Password recovery through both supported methods.
- Access to protected pages after authentication.
- Separate administrator access and registered-user listing.
- Logout and session handling.

### 10. Milestone Scope

This milestone establishes the authentication foundation for the overall maritime freight project. Freight price prediction, agentic decision-making, and route optimization are planned for subsequent milestones and are not claimed as completed features of this authentication module.

### 11. Future Enhancements

- Integrate maritime freight pricing prediction.
- Develop route optimization capabilities.
- Introduce agentic AI workflows for freight-related decisions.
- Connect authentication with the complete maritime freight application.

---

**Project:** Agentic AI for Maritime Freight Pricing and Route Optimization  
**Milestone:** 1 — Secure Authentication System  
**Development Environment:** Google Colab  
**Application Framework:** Streamlit
