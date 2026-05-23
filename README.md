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
Backend-API-para-streaming-y-gesti-n-de-podcasts/
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
```

---

# ⚙️ Installation

## Clone the repository

```bash
git clone https://github.com/isairey/Backend-API-para-streaming-y-gesti-n-de-podcasts.git
cd Backend-API-para-streaming-y-gesti-n-de-podcasts
```

## Install dependencies

Using npm:

```bash
npm install
```

Or using yarn:

```bash
yarn
```

---

# 🚀 Running the Server

## Requirements

Before starting the server, make sure you have:

- Node.js 8+
- MongoDB installed and running on port `27017`

## Start development server

Using npm:

```bash
npm run dev
```

Or using yarn:

```bash
yarn dev
```

Server will run at:

```bash
http://localhost:3001/Backend-API-para-streaming-y-gesti-n-de-podcasts/api/v1/
```

---

# 🧪 Running Tests

## Run tests

```bash
npm test
```

Or:

```bash
yarn test
```

## Run tests with coverage

```bash
npm run test:coverage
```

Or:

```bash
yarn test:coverage
```

---

# 🔗 API Routes

## Base URL

```bash
http://localhost:3001/Backend-API-para-streaming-y-gesti-n-de-podcasts/api/v1/
```

---

## Health Check

```http
GET /
```

Returns API status.

---

## Home

```http
GET /home?categories=all
```

Returns podcasts and authors based on selected categories.

---

## Categories

```http
GET /categories/:category
```

Returns podcasts and authors related to a category.

---

## Authors

### Create Author

```http
POST /authors
```

### Get All Authors

```http
GET /authors
```

### Get Author By ID

```http
GET /authors/:id
```

### Update Author

```http
PATCH /authors/:id
```

### Delete Author

```http
DELETE /authors/:id
```

### Upload Podcast

```http
POST /authors/:id/podcasts
```

Supports `.mp3` file uploads.

---

## Podcasts

### Get All Podcasts

```http
GET /podcasts
```

### Get Podcast By ID

```http
GET /podcasts/:id
```

### Stream Podcast

```http
GET /podcasts/:id/listen
```

### Download Podcast

```http
GET /podcasts/:id/download
```

---

# 📦 Models

## Author Model

```json
{
  "name": "String",
  "categories": ["science", "technology"],
  "profileImageURL": "String",
  "thumbnailProfileImageURL": "String",
  "about": "String"
}
```

---

## Podcast Model

```json
{
  "title": "String",
  "description": "String",
  "imageURL": "String",
  "thumbnailImageURL": "String",
  "category": "science",
  "stars": 5
}
```

---

# ☁️ Deployment

This project can be deployed easily on:

- Heroku
- Railway
- Render
- VPS servers

Example production command:

```bash
npm start
```

---

# 🤝 Contributing

Contributions are always welcome 🚀

1. Fork the repository
2. Create your feature branch

```bash
git checkout -b feature/new-feature
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push to GitHub

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

# 👨‍💻 Desarrollador

### Isai Reyes - FullStack Developer

- GitHub: https://github.com/isairey


---

# 📜 License

This project is licensed under the MIT License.
