[DocAI Frontend](https://github.com/nizamsalim/docai_frontend)   
[DocAI Backend](https://github.com/nizamsalim/docai_backend)

# AI-Powered Document Generation App

This project is an AI-powered document generation platform designed to help users create, edit, and export richly formatted documents. It leverages advanced language models to convert markdown content into professional Word documents and provides a seamless editing experience through a modern frontend and robust backend.

The application consists of two major components:

- **Frontend (React)** – Handles the user interface, markdown editor, and document preview.
- **Backend (Flask)** – Processes document generation, authentication, and communication with AI services.

---

## 🚀 Installation & Setup

### **Frontend Setup**

1. Clone the repository:
   ```bash
   git clone https://github.com/nizamsalim/docai_frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### **Backend Setup**

1. Clone the repository:
   ```bash
   git clone https://github.com/nizamsalim/docai_backend
   ```
2. Install dependencies using Poetry:
   ```bash
   poetry install
   ```

---

## 🔐 Environment Variables

### **Frontend Environment Variables**

| Variable       | Description                  |
| -------------- | ---------------------------- |
| `VITE_API_URL` | URL of the backend Flask API |

---

### **Backend Environment Variables**

Create a `.env` file with the following variables:

```
FLASK_APP=docai_backend.app
FLASK_ENV=development
FLASK_DEBUG=1
DATABASE_URL
JWT_SECRET
GEMINI_API_KEY
```

**Descriptions:**

- **FLASK_APP**: Entry point for the Flask application.
- **FLASK_ENV**: Sets the environment mode (development/production).
- **FLASK_DEBUG**: Enables Flask debug mode.
- **DATABASE_URL**: Connection string for the database.
- **JWT_SECRET**: Secret key used to sign JWT tokens.
- **GEMINI_API_KEY**: API key used for AI model access.

---

## ▶️ How to Run the Application

### **Frontend**

Run the development server:

```bash
npm run dev
```

### **Backend**

1. Generate SSL certificates (self-signed) using OpenSSL:

   ```bash
   openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365 -nodes
   ```

2. Start the Flask server:
   ```bash
   poetry run flask run --cert=cert.pem --key=key.pem
   ```

---

## 📄 About the AI Document Generation App

This application allows users to:

- Write and edit content in **markdown**.
- Automatically convert markdown into **Microsoft Word (.docx)** documents.
- Use **AI-assisted generation** for refining or expanding document content.
- Seamlessly manage sections, formatting, and previews through an intuitive interface.

The backend orchestrates AI interactions and document rendering, while the frontend delivers a modern, responsive editing experience.

This system is ideal for projects requiring automated report generation, structured documentation, dynamic content drafting, or AI-assisted editing.

---

## ✔️ You're all set!

Follow the above steps to run both services and start using the AI-powered document creation workflow.
