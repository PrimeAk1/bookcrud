# Book Management and Review Web Application

This web application is a simple book management system where users can register, log in, and leave reviews for books. The backend is built using **Spring Boot**, and the frontend is developed with **HTML, CSS**. The app implements **Spring Security** for authentication, **JWT (JSON Web Token)** for securing endpoints, and **Role-Based Access Control (RBAC)** to restrict access based on user roles.

## Features

- **User Registration and Login**: Users can register and log in with an email and password.
- **Role-Based Access Control (RBAC)**: The application defines roles such as **USER** and **ADMIN** to control access to various resources.
- **Book Management**: Users can perform **CRUD** (Create, Read, Update, Delete) operations on books.
- **Review System**: Users can leave, edit, and delete reviews for books.
- **JWT Authentication**: Secure access to endpoints with JWT tokens, which are stored in the browser’s cookies after login.
- **Restricted Access to Pages**: Pages that a user does not have permission to access will not be available, and unauthorized users will be redirected to an access denied page.

## Technologies Used

- **Backend**:
  - Spring Boot
  - Spring Security (JWT Authentication)
  - Spring Data JPA
  - PostgreSQL

- **Frontend**:
  - HTML
  - CSS

## Missing Features

- **Restricted Access to Unauthorized Pages**: The frontend currently does not fully handle the case where users try to access pages for which they don't have permission. When a user without the required role (e.g., an unauthorized user trying to access an admin page) tries to navigate to a restricted page, they are not yet redirected to an "Access Denied" page or logged out appropriately. This feature can be added to handle route protection properly.

## Future Improvements

- **Professional React Frontend**: Instead of using HTML and CSS, the frontend can be improved with a more sophisticated React-based UI, utilizing libraries such as **Material-UI** or **Bootstrap** for better design and responsiveness.

