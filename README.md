# RoleBasedLoginServletApp

## Description
A Java Servlet-based Maven web application demonstrating **login authentication** and **role-based redirection**. The project shows how to implement **Admin and User login**, validate credentials, and redirect users to role-specific dashboards.

## Features
- Login page with username and password input.
- Valid credentials:
  - Admin → `admin` / `admin123`
  - User → `user` / `user123`
- Invalid credentials reload login page with an error message.
- Role-based redirection:
  - Admin → AdminDashboard.html
  - User → UserDashboard.html
- Use of `RequestDispatcher.forward()` and `RequestDispatcher.include()`.
- Use of `sendRedirect()` for role-based navigation.

## Technologies Used
- Java 8+
- Servlet API
- Maven
- HTML
- Tomcat 9+ (for deployment)

## Project Structure
src/main/java/com/example/servlet/ → Servlets (LoginServlet.java, RoleServlet.java)
src/main/webapp/ → HTML pages (login.html, AdminDashboard.html, UserDashboard.html)
pom.xml → Maven configuration
.gitignore → Excludes target folder and IDE files
