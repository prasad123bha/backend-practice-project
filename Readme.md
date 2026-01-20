# Backend Project Setup

This README provides step-by-step instructions to set up and run the backend project locally. Follow the steps carefully to avoid common configuration issues.

---

## 📦 Prerequisites

Make sure the following tools are installed on your system:

* **Node.js** (v18+ recommended)
* **npm** or **yarn**
* **Git**
* **MongoDB** (local or MongoDB Atlas)
* **Postman** (optional, for API testing)

Check versions:

```bash
node -v
npm -v
git --version
```

---

## 📁 Project Structure

```text
backend/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middlewares/
│   ├── config/
│   └── app.js
├── .env
├── package.json
├── index.js
└── README.md
```

---

## 🚀 Installation Steps

### 1️⃣ Clone the Repository

```bash
git clone <repository-url>
cd backend
```

### 2️⃣ Install Dependencies

```bash
npm install
```

or

```bash
yarn install
```

---

## ⚙️ Environment Configuration

Create a `.env` file in the root directory and add the following:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
NODE_ENV=development
```

⚠️ **Do not commit ********`.env`******** file to GitHub**

---

## ▶️ Running the Project

### Development Mode

```bash
npm run dev
```

### Production Mode

```bash
npm start
```

Server will start on:

```
http://localhost:5000
```

---

## 🔌 API Testing

You can test APIs using:

* Postman
* Thunder Client (VS Code extension)

Base URL:

```
http://localhost:5000/api
```

---

## 🛠 Common Scripts

```json
"scripts": {
  "start": "node server.js",
  "dev": "nodemon server.js"
}
```

---

## ❗ Troubleshooting

* **MongoDB connection error**: Check `MONGO_URI`
* **Port already in use**: Change `PORT` in `.env`
* **Module not found**: Run `npm install`

---

## 📌 Best Practices

* Use `.env` for secrets
* Follow MVC architecture
* Validate API inputs
* Handle errors properly

---

## 📄 License

This project is licensed under the MIT License.

---

## 🤝 Contribution

Feel free to fork this project and submit pull requests.

---

### ✅ Backend setup complete. Happy coding! 🚀
