# Spring Security Practice

Welcome to my Spring Security practice repository! This repository contains my learning exercises and practice tasks focused on securing a Spring Boot application using Spring Security.

## Key Learnings

### In-Memory Authentication
- **Setup**: Configured `InMemoryUserDetailsManager` to manage user details directly in memory.
- **Users**:
  - **John**: Role - `EMPLOYEE`
  - **Mary**: Roles - `EMPLOYEE`, `MANAGER`
  - **Susan**: Roles - `EMPLOYEE`, `MANAGER`, `ADMIN`

### Role-Based Authorization
- **Access Control**: Implemented role-based access control for different API endpoints.
- **Endpoint Permissions**:
  - `GET /api/employees`: Accessible by `EMPLOYEE` role.
  - `GET /api/employees/**`: Accessible by `EMPLOYEE` role.
  - `POST /api/employees`: Accessible by `MANAGER` role.
  - `PUT /api/employees`: Accessible by `MANAGER` role.
  - `DELETE /api/employees/**`: Accessible by `ADMIN` role.

### HTTP Basic Authentication
- Configured HTTP Basic authentication to protect endpoints and ensure only authorized users can access them.

### CSRF Protection
- Disabled CSRF protection for stateless REST APIs to simplify the development process.

## Tools Used
- **Spring Boot**: The foundation of the application.
- **Spring Security**: For implementing security measures.
- **Postman**: Used for testing all endpoints to ensure security configurations work as expected.

## Testing
- **Postman**: Extensively used to test API endpoints, verifying that:
  - Only authorized users can access specific endpoints.
  - Role-based access control is functioning correctly.

## Next Steps
- Continue learning deeper aspects of authentication with Spring Security.
- Explore additional security features and best practices for securing web applications.

## How to Run the Application
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spring-security-practice.git
