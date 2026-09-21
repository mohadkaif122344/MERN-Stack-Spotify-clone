🎵 MERN Spotify Clone

A full-stack Spotify-inspired music streaming application built with the MERN stack. The project includes a user-facing music player, album and song browsing, audio controls, and a separate admin panel for managing songs and albums.

🚀 Features

- 🎵 Browse songs and albums
- ▶️ Play and pause songs
- ⏮️ Previous and next song controls
- 🔊 Audio progress and seek control
- 📀 Album details and song listing
- 🎚️ Music player with duration tracking
- 🛠️ Admin panel
- ➕ Add songs and albums
- 🗑️ Remove songs and albums
- ☁️ Cloudinary media upload
- 🗄️ MongoDB database
- 📱 Responsive UI

🛠️ Tech Stack

Frontend

- React
- Vite
- React Router
- Axios
- Tailwind CSS

Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- Cloudinary
- Multer
- CORS
- dotenv

Admin Panel

- React
- Vite
- React Router
- Axios
- Tailwind CSS
- React Toastify

📂 Project Structure

MERN-Stack-Spotify-clone-main/
│
├── Backend/
│   ├── src/
│   │   ├── config/
│   │   │   ├── cloudinary.js
│   │   │   └── mongodb.js
│   │   ├── controllers/
│   │   │   ├── albumController.js
│   │   │   └── songController.js
│   │   ├── middleware/
│   │   │   └── multer.js
│   │   ├── models/
│   │   │   ├── albumModel.js
│   │   │   └── songModel.js
│   │   └── routes/
│   │       ├── albumRoute.js
│   │       └── songRoute.js
│   ├── server.js
│   └── package.json
│
├── Spotify frontend/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   └── package.json
│
└── spotify-admin/
    ├── src/
    │   ├── assets/
    │   ├── components/
    │   ├── pages/
    │   ├── App.jsx
    │   └── main.jsx
    └── package.json

🎧 Music Player

The frontend provides:

- Play / Pause
- Previous / Next
- Song progress bar
- Seek functionality
- Current time and total duration
- Album-based song filtering
- Dynamic songs and albums loaded from backend

🛠️ Admin Panel

The admin panel provides:

- Add Song
- List Songs
- Remove Song
- Add Album
- List Albums
- Remove Album
- Upload song audio
- Upload album/song images
- Select album while adding a song
- Album background color selection

🌐 API Endpoints

Songs

POST /api/song/add
GET  /api/song/list
POST /api/song/remove

Albums

POST /api/album/add
GET  /api/album/list
POST /api/album/remove

☁️ Cloudinary

Song audio files and images are uploaded to Cloudinary.

Required environment variables:

CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key

🗄️ MongoDB

The backend connects to MongoDB using:

MONGODB_URI=your_mongodb_connection_string

The application uses the "spotify" database.

⚙️ Backend Setup

cd Backend
npm install
npm run dev

Backend runs on:

http://localhost:4000

💻 Frontend Setup

cd "Spotify frontend"
npm install
npm run dev

🛠️ Admin Setup

Open another terminal:

cd spotify-admin
npm install
npm run dev

The admin panel communicates with the backend running on:

http://localhost:4000

🔄 Application Flow

Admin Panel
    │
    ├── Add Song
    ├── Add Album
    ├── List Song
    └── List Album
           │
           ▼
       Express API
           │
      ┌────┴────┐
      ▼         ▼
   MongoDB   Cloudinary
      │         │
      └────┬────┘
           ▼
    Spotify Frontend
           │
           ▼
      Music Player

🔮 Future Improvements

- User authentication
- User playlists
- Like/favorite songs
- Search functionality
- Real-time recommendations
- Premium subscription
- Improved mobile player
- Deployment

👨‍💻 Author

Mohad Kaif

GitHub: "https://github.com/mohadkaif122344"
