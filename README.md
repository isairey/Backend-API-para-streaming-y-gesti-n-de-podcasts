<div align="center">

<img width="220" src="https://cdn-icons-png.flaticon.com/512/3135/3135715.png" />

# 🎙️ MindCast Server

### Backend API para streaming y gestión de podcasts 🚀

<p align="center">
  <b>MindCast Server</b> es una API RESTful desarrollada con Node.js, Express y MongoDB para gestionar autores, podcasts y streaming de archivos MP3.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge"/>
</p>

</div>

---

# 📚 Table of Contents

- [✨ Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📂 Project Structure](#-project-structure)
- [⚙️ Installation](#️-installation)
- [🚀 Running the Server](#-running-the-server)
- [🧪 Running Tests](#-running-tests)
- [🔗 API Routes](#-api-routes)
- [📦 Models](#-models)
- [☁️ Deployment](#️-deployment)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

---

# ✨ Features

✅ RESTful API architecture  
✅ Podcast audio upload & streaming  
✅ Author and podcast management  
✅ MP3 file processing and duration parsing  
✅ MongoDB database integration  
✅ Audio download support  
✅ Category filtering system  
✅ Automated testing with Jest  
✅ CI/CD integration with Travis CI  
✅ File uploads using Multer  
✅ GridFS audio streaming support  

---

# 🛠️ Tech Stack

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose

### Storage & Streaming
- Multer
- GridFS Stream
- Amazon S3

### Testing & Quality
- Jest
- Supertest
- ESLint
- Prettier
- Husky

### Deployment
- Heroku
- Travis CI

---

# 📂 Project Structure

```bash
mindcast-server/
│
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── services/
│   ├── models/
│   ├── middlewares/
│   └── utils/
│
├── tests/
├── assets/
├── uploads/
├── .env
├── package.json
└── README.md
