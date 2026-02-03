# NoteHub API

A full-featured RESTful API for managing notes with user authentication, built with Node.js and Express. This backend service provides secure note management with JWT authentication, email verification, file uploads, and MongoDB integration.

🔗 **Live Demo:** [NoteHub API Documentation](https://notehub-api-nodejs.vercel.app)

## 📋 Description

NoteHub API is a robust backend service that allows users to create, read, update, and delete notes with secure authentication. The API features user registration with email verification, JWT-based authentication, password reset functionality, and Cloudinary integration for file uploads.

## 🛠️ Technologies

- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **MongoDB** + **Mongoose** - Database and ODM
- **JWT** (jsonwebtoken) - Authentication tokens
- **Bcrypt** - Password hashing
- **Nodemailer** - Email sending
- **Cloudinary** - Cloud storage for file uploads
- **Multer** - File upload middleware
- **Celebrate** (Joi) - Request validation
- **Pino** - Logging
- **CORS** - Cross-origin resource sharing
- **Cookie Parser** - Cookie handling
- **Handlebars** - Email templates

## ⚡ Features

### Authentication
- User registration with email verification
- Login with JWT tokens
- Password reset via email
- Secure cookie-based session management
- Token refresh mechanism

### Notes Management
- Create, read, update, and delete notes
- User-specific notes
- File attachments via Cloudinary

### Additional Features
- Request validation with Celebrate (Joi)
- HTTP request logging with Pino
- Error handling middleware
- CORS support for frontend integration

## 🚀 Installation

```bash
npm install
```

## 💻 Usage

```bash
# Development mode with nodemon
npm run dev

# Production mode
npm start
```

## 📚 API Endpoints

### Authentication Routes
- `POST /auth/register` - Register a new user
- `POST /auth/login` - Login user
- `POST /auth/logout` - Logout user
- `POST /auth/refresh` - Refresh access token
- `POST /auth/request-reset-email` - Request password reset
- `POST /auth/reset-password` - Reset password
- `POST /auth/verify` - Verify email address

### Notes Routes
- `GET /notes` - Get all user notes
- `GET /notes/:noteId` - Get note by ID
- `POST /notes` - Create new note
- `PATCH /notes/:noteId` - Update note
- `DELETE /notes/:noteId` - Delete note

## 👤 Author

**Olena Akatieva**

- LinkedIn: [linkedin.com/in/olena-akatieva](https://linkedin.com/in/olena-akatieva)
- GitHub: [@helen-akateva](https://github.com/helen-akateva)

---

*This project was created as part of a Node.js learning curriculum.*
