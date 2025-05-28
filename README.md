# 📁 PDF Management & Collaboration System

A full-stack web application to upload, preview, comment on, and share PDF files — built with Angular, Node.js, MySQL, and Firebase Auth.

---

## 🚀 Features

- 🔐 User Signup & Login (Firebase Auth)
- 📤 Upload and store PDFs
- 🖼 Inline preview with secure streaming
- 🧵 Threaded comment system with replies
- 📬 Share files via email with one click
- 🔗 Generate public shareable links
- 📊 Admin-friendly dashboard
- 💬 Comment sidebar for collaboration

---

## 🧰 Tech Stack

| Frontend    | Backend       | Storage       | Auth        |
|-------------|---------------|---------------|-------------|
| Angular 16  | Node.js + Express | MySQL (local) | Firebase Authentication |
| Angular Material + TailwindCSS | Nodemailer | Local File System (PDFs) | JWT-based with Firebase tokens |

---

## 📸 Screenshots

| Dashboard | PDF Viewer | Comment System | Share Dialog |
|----------|-------------|----------------|--------------|
| ![Dashboard](screenshots/dashboard.png) | ![Viewer](screenshots/viewer.png) | ![Comments](screenshots/comments.png) | ![Dialog](screenshots/share-dialog.png) |

> Add your actual screenshots in the screenshots/ folder.

---

## 🎥 Demo Video

📹 [Watch Demo]([https://your-video-link.com](https://drive.google.com/file/d/1iCfxBRPXJxSjq2yAUEJr-OFOHhntJsv9/view?usp=drive_link))

---

## ⚙ Getting Started

### 1️⃣ Clone the repo

```bash
git clone https://github.com/shivam109/PdfCollabAndManagement-Frontend.git
cd PdfCollabAndManagement-Frontend
cd backend
npm install
cp .env.example .env # Set your Firebase and DB config

# Create MySQL DB
mysql -u root -p < db/schema.sql

node index.js
cd frontend
npm install
ng serve
