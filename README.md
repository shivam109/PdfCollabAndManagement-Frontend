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
## 🔌 API Endpoints
Endpoint	Method	Description
/api/auth/signup	POST	Register a new user
/api/auth/login	POST	Authenticate user
/api/files/upload	POST	Upload a PDF file
/api/files/user/:uid	GET	List user's PDFs
/api/files/view/:filename	GET	Stream PDF preview
/api/files/:id/share	GET	Generate public share link
/api/files/:id/share/email	POST	Share link to email address
/api/files/:id/comments	GET	Fetch all comments
/api/files/:id/comments	POST	Add comment or reply
---

## 📸 Screenshots
| ![WhatsApp Image 2025-05-28 at 11 03 02 PM](https://github.com/user-attachments/assets/f04341d5-e267-4773-b843-7e2da7de11aa)
![WhatsApp Image 2025-05-28 at 11 02 59 PM](https://github.com/user-attachments/assets/4ced34d2-10c8-4c7e-8a17-d9692b69e558)
![WhatsApp Image 2025-05-28 at 11 02 58 PM (1)](https://github.com/user-attachments/assets/9b49547a-ba29-4d9d-b4bb-16562cf31d03)
![WhatsApp Image 2025-05-28 at 11 02 58 PM](https://github.com/user-attachments/assets/761d7b7f-6b07-4fd2-aae6-f4632f42eb6d)
|

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
