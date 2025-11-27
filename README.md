# Homyz - Real Estate Platform

A modern MERN stack application for property listing, search, and booking.

![Homyz Banner](https://github.com/Ananya01Agrawal/Real-estate-Booking-Website/assets/99130567/9dce86bd-771c-493a-821f-bce92039c688)

---

## 🛠️ Tech Stack

**Frontend**
- React 18.2
- React Router 6.x
- Axios
- CSS3/SCSS

**Backend**
- Node.js 18+
- Express.js 4.x
- MongoDB 6.x
- Mongoose 7.x

**Authentication & Security**
- JWT (jsonwebtoken)
- bcryptjs
- Google OAuth 2.0

**Additional Services**
- Cloudinary (Image storage)
- Mapbox/Google Maps API

---

## 🚀 Setup Steps

### Prerequisites
```bash
Node.js v18+ and npm v8+
MongoDB (local or Atlas)
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/homyz-real-estate.git
cd homyz-real-estate
```

2. **Install dependencies**
```bash
# Install server dependencies
npm install

# Install client dependencies
cd client
npm install
cd ..
```

3. **Configure environment variables**

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

4. **Setup MongoDB**

**Local MongoDB:**
```bash
mongod --dbpath /path/to/data
```

**MongoDB Atlas:**
- Create account at [mongodb.com/cloud/atlas](https://www.mongodb.com/cloud/atlas)
- Create cluster and get connection string
- Add to `.env` file

5. **Setup Google OAuth**
- Go to [Google Cloud Console](https://console.cloud.google.com/)
- Create project and enable Google+ API
- Create OAuth 2.0 credentials
- Add authorized redirect URIs:
  - `http://localhost:3000/auth/google/callback`
- Copy Client ID and Secret to `.env`

6. **Start the application**
```bash
# Run both client and server
npm run dev

# Or separately
npm run server  # http://localhost:5000
npm run client  # http://localhost:3000
```

---

## 📸 Screenshots

### Homepage
![Homepage](https://via.placeholder.com/800x400?text=Homepage+Screenshot)

### Property Details
![Property Details](https://via.placeholder.com/800x400?text=Property+Details+Page)

### Search & Filter
![Search](https://via.placeholder.com/800x400?text=Search+and+Filter)

### User Dashboard
![Dashboard](https://via.placeholder.com/800x400?text=User+Dashboard)

**Demo Video:** [Watch Demo](https://youtube.com/watch?v=demo)

---

## 📋 Assumptions

- Users must have valid email addresses for registration
- Property listings require manual verification by owners
- All prices are in USD
- Application supports English language only
- Images are uploaded via Cloudinary CDN
- Users can book only one visit per property at a time

---

## ✨ Bonus Features

✅ **Google OAuth Integration** - One-click social login  
✅ **Image Upload with Cloudinary** - Optimized image storage and delivery  
✅ **Interactive Maps** - Location visualization with nearby amenities  
✅ **Advanced Search Filters** - Filter by type, price, location, bedrooms, bathrooms  
✅ **Responsive Design** - Mobile-first, works on all devices  
✅ **Favorites System** - Save and manage favorite properties  
✅ **Visit Scheduling** - Book property viewings with date/time selection  
✅ **User Profile Management** - Complete profiles with avatar uploads  
✅ **Real-time Availability** - Live property status updates

---

## 📁 Project Structure

```
homyz-real-estate/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── context/        # React context
│   │   └── utils/          # Helper functions
│   └── package.json
├── server/                 # Express backend
│   ├── config/            # Configuration
│   ├── controllers/       # Route controllers
│   ├── models/            # MongoDB models
│   ├── routes/            # API routes
│   ├── middleware/        # Custom middleware
│   └── server.js
├── .env                   # Environment variables
└── package.json
```

---

## 🔌 API Endpoints

### Authentication
```
POST   /api/auth/register
POST   /api/auth/login
GET    /api/auth/google
GET    /api/auth/google/callback
```

### Properties
```
GET    /api/properties
GET    /api/properties/:id
POST   /api/properties          (Auth required)
PUT    /api/properties/:id      (Auth required)
DELETE /api/properties/:id      (Auth required)
```

### Users
```
GET    /api/users/profile       (Auth required)
PUT    /api/users/profile       (Auth required)
GET    /api/users/favorites     (Auth required)
POST   /api/users/favorites/:id (Auth required)
DELETE /api/users/favorites/:id (Auth required)
```

### Bookings
```
POST   /api/bookings            (Auth required)
GET    /api/bookings            (Auth required)
DELETE /api/bookings/:id        (Auth required)
```

---

## 📧 Contact

**Harsh Kumar**  
📧 harshkumar808348@gmail.com  
🐙 [GitHub](https://github.com/yourusername)  
💼 [LinkedIn](https://linkedin.com/in/yourprofile)

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Made with ❤️ using MERN Stack

</div>
