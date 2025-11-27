<div align="center">

# 🏡 Homyz - Real Estate Platform

### *Discover Your Dream Home*

**A modern MERN stack application for property listing, search, and booking**

![Homyz Banner](https://github.com/Ananya01Agrawal/Real-estate-Booking-Website/assets/99130567/9dce86bd-771c-493a-821f-bce92039c688)

[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](http://makeapullrequest.com)

[🚀 Quick Start](#-setup-steps) • [📸 Screenshots](#-screenshots) • [✨ Features](#-bonus-features) • [📧 Contact](#-contact)

</div>

---

## 🛠️ Tech Stack

<table>
<tr>
<td align="center" width="50%">

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=flat-square&logo=react-router&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![SASS](https://img.shields.io/badge/SASS-CC6699?style=flat-square&logo=sass&logoColor=white)

</td>
<td align="center" width="50%">

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat-square&logo=mongoose&logoColor=white)

</td>
</tr>
<tr>
<td align="center" width="50%">

### Authentication & Security
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=JSON%20web%20tokens&logoColor=white)
![OAuth](https://img.shields.io/badge/OAuth_2.0-EB5424?style=flat-square&logo=auth0&logoColor=white)

</td>
<td align="center" width="50%">

### Additional Services
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat-square&logo=cloudinary&logoColor=white)
![Google Maps](https://img.shields.io/badge/Google_Maps-4285F4?style=flat-square&logo=google-maps&logoColor=white)

</td>
</tr>
</table>

---

## 🚀 Setup Steps

<details open>
<summary><b>📦 Prerequisites</b></summary>

```bash
Node.js v18+ and npm v8+
MongoDB (local or Atlas)
Google Cloud Console Account (for OAuth)
```
</details>

<details open>
<summary><b>⚙️ Installation</b></summary>

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/homyz-real-estate.git
cd homyz-real-estate
```

### 2️⃣ Install dependencies
```bash
# Install server dependencies
npm install

# Install client dependencies
cd client
npm install
cd ..
```

### 3️⃣ Configure environment variables

Create `.env` file in root directory:
```env
# Database
MONGO_URI=mongodb://localhost:27017/homyz

# Authentication
JWT_SECRET=your_jwt_secret_key_min_32_characters
JWT_EXPIRE=7d

# Google OAuth
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

# Server
PORT=5000
NODE_ENV=development
CLIENT_URL=http://localhost:3000

# Cloudinary (Optional)
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

### 4️⃣ Setup MongoDB

<table>
<tr>
<td width="50%">

**Option A: Local MongoDB**
```bash
mongod --dbpath /path/to/data
```

</td>
<td width="50%">

**Option B: MongoDB Atlas**
1. Create account at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
2. Create cluster
3. Get connection string
4. Add to `.env` file

</td>
</tr>
</table>

### 5️⃣ Setup Google OAuth
1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create project and enable Google+ API
3. Create OAuth 2.0 credentials
4. Add authorized redirect URI: `http://localhost:3000/auth/google/callback`
5. Copy Client ID and Secret to `.env`

### 6️⃣ Start the application
```bash
# Run both client and server concurrently
npm run dev
```

#### Or run separately:
```bash
npm run server  # Backend → http://localhost:5000
npm run client  # Frontend → http://localhost:3000
```

</details>

<div align="center">

### 🎉 **Application is now running!**
**Frontend:** http://localhost:3000  
**Backend:** http://localhost:5000

</div>

---

## 📸 Screenshots

<div align="center">

### 🏠 Homepage
![Homepage](https://via.placeholder.com/900x500/4A90E2/ffffff?text=Homepage+%7C+Property+Listings)

### 🔍 Property Details
![Property Details](https://via.placeholder.com/900x500/7B68EE/ffffff?text=Property+Details+%7C+Interactive+Maps)

### 🎯 Search & Filter
![Search](https://via.placeholder.com/900x500/50C878/ffffff?text=Advanced+Search+%26+Filters)

### 👤 User Dashboard
![Dashboard](https://via.placeholder.com/900x500/FF6B6B/ffffff?text=User+Dashboard+%7C+Manage+Properties)

---

### 🎥 Demo Video

[![Watch Demo](https://img.shields.io/badge/▶️_Watch_Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/watch?v=demo)

</div>

---

## 📋 Assumptions

<table>
<tr>
<td width="33%">

💡 **User Management**
- Valid email addresses required
- Manual listing verification
- Single language (English)

</td>
<td width="33%">

💡 **Technical**
- All prices in USD
- Cloudinary for images
- One booking per property

</td>
<td width="33%">

💡 **Security**
- JWT authentication
- Secure password hashing
- OAuth 2.0 integration

</td>
</tr>
</table>

---

## ✨ Bonus Features

<div align="center">

<table>
<tr>
<td align="center" width="33%">

### 🔐 Authentication
✅ **Google OAuth Integration**  
One-click social login

✅ **JWT Security**  
Secure token-based auth

✅ **Profile Management**  
Avatar uploads & customization

</td>
<td align="center" width="33%">

### 🏡 Property Features
✅ **Advanced Search**  
Multi-criteria filtering

✅ **Interactive Maps**  
Location visualization

✅ **Image Optimization**  
Cloudinary CDN integration

</td>
<td align="center" width="33%">

### 🎨 User Experience
✅ **Responsive Design**  
Mobile-first approach

✅ **Favorites System**  
Save & organize properties

✅ **Visit Scheduling**  
Book viewings with calendar

</td>
</tr>
</table>

</div>

---

## 📁 Project Structure

```
📦 homyz-real-estate/
├── 📂 client/                    # React Frontend
│   ├── 📂 src/
│   │   ├── 📂 components/        # Reusable UI components
│   │   ├── 📂 pages/             # Page components
│   │   ├── 📂 context/           # React Context API
│   │   └── 📂 utils/             # Helper functions
│   └── 📄 package.json
│
├── 📂 server/                    # Express Backend
│   ├── 📂 config/                # Configuration files
│   ├── 📂 controllers/           # Route controllers
│   ├── 📂 models/                # MongoDB models
│   ├── 📂 routes/                # API routes
│   ├── 📂 middleware/            # Custom middleware
│   └── 📄 server.js              # Entry point
│
├── 📄 .env                       # Environment variables
└── 📄 package.json               # Dependencies
```

---

## 🔌 API Endpoints

<details>
<summary><b>🔐 Authentication</b></summary>

```http
POST   /api/auth/register       # Register new user
POST   /api/auth/login          # User login
GET    /api/auth/google         # Google OAuth login
GET    /api/auth/google/callback # OAuth callback
```
</details>

<details>
<summary><b>🏡 Properties</b></summary>

```http
GET    /api/properties          # Get all properties
GET    /api/properties/:id      # Get property by ID
POST   /api/properties          # Create property (Auth)
PUT    /api/properties/:id      # Update property (Auth)
DELETE /api/properties/:id      # Delete property (Auth)
```
</details>

<details>
<summary><b>👤 Users</b></summary>

```http
GET    /api/users/profile       # Get user profile (Auth)
PUT    /api/users/profile       # Update profile (Auth)
GET    /api/users/favorites     # Get favorites (Auth)
POST   /api/users/favorites/:id # Add to favorites (Auth)
DELETE /api/users/favorites/:id # Remove favorite (Auth)
```
</details>

<details>
<summary><b>📅 Bookings</b></summary>

```http
POST   /api/bookings            # Create booking (Auth)
GET    /api/bookings            # Get user bookings (Auth)
DELETE /api/bookings/:id        # Cancel booking (Auth)
```
</details>

---

## 📧 Contact

<div align="center">

<img src="https://img.shields.io/badge/Harsh_Kumar-Developer-blue?style=for-the-badge" alt="Developer Badge">

<table>
<tr>
<td align="center">

📧 **Email**  
[harshkumar808348@gmail.com](mailto:harshkumar808348@gmail.com)

</td>
<td align="center">

🐙 **GitHub**  
[@yourusername](https://github.com/yourusername)

</td>
<td align="center">

💼 **LinkedIn**  
[Harsh Kumar](https://linkedin.com/in/yourprofile)

</td>
</tr>
</table>

### 💬 Need Help?

[![Ask Question](https://img.shields.io/badge/Ask-Question-orange?style=for-the-badge&logo=stackoverflow)](https://github.com/yourusername/homyz-real-estate/issues)
[![Report Bug](https://img.shields.io/badge/Report-Bug-red?style=for-the-badge&logo=github)](https://github.com/yourusername/homyz-real-estate/issues)
[![Request Feature](https://img.shields.io/badge/Request-Feature-brightgreen?style=for-the-badge&logo=github)](https://github.com/yourusername/homyz-real-estate/issues)

</div>

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Made with ❤️ using MERN Stack

</div>
