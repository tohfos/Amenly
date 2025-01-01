# Amenly Password manager 🔒

This project is a **Password Manager API** built with **Node.js**, **Express.js**, and **MongoDB**, designed to securely manage user credentials and platform passwords. It provides robust features such as user authentication, password encryption, profile management, and secure storage for sensitive information.

---

## Features 🛠️

### User Authentication
- **Register and Login**:
  - Users can create accounts and log in using secure, hashed credentials.
  - Passwords are hashed with **bcrypt** before being stored in MongoDB.
- **Token-Based Authentication**:
  - Uses **JWT (JSON Web Tokens)** for secure and stateless authentication.
  - Tokens are stored as HTTP-only cookies to prevent XSS attacks.

### Password Management
- **Add Platform Credentials**:
  - Securely store platform credentials (e.g., username, email, password).
  - Passwords are encrypted using AES-based encryption before being stored.
- **Retrieve Stored Passwords**:
  - Decrypt and retrieve stored platform passwords securely.
- **Update and Delete Credentials**:
  - Update platform credentials or remove them as needed.

### Profile Management
- **Profile Updates**:
  - Update user information, such as username, email, and password.
- **Profile Picture Management**:
  - Upload, retrieve, and delete profile pictures stored in the system.

### Security Highlights
- **Password Encryption**:
  - Platform passwords are encrypted using a secure encryption algorithm before storage.
  - Password decryption is performed only when explicitly requested by authenticated users.
- **User Password Hashing**:
  - User account passwords are hashed using **bcrypt** for added security.
- **Middleware Integration**:
  - Routes are protected by an authentication middleware to prevent unauthorized access.
