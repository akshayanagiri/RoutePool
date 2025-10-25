# RoutePool - Smart Carpooling Platform

It is an application designed to connect drivers with empty seats to riders heading in the same direction, promoting eco-friendly, affordable, and safe commuting.

## ✨ Features

- **Owner (Driver) Ride Posting**: Car owners can post rides by specifying the source, destination, route (map integration is implied), date, time, and available seats.
- **Ride Searching**: Passengers can efficiently search for rides based on their source and destination requirements.
- **Request & Approval System**: Riders can send ride requests to owners, who can then approve or reject the request.
- **Secure Authentication**: User login and registration secured using JWT tokens and password hashing.
- **Modern UI/UX**: A fully responsive and intuitive interface for seamless usage on any device.
  
## 🛠️ Tech Stack

- **Frontend** : React, Vite (for the modern build system), Tailwind CSS (for styling)
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication** : Passport.js (as the core middleware), JWT, Bcrypt


## 🚀 Quick Start


### Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-username/RoutePool.git
cd RoutePool
```

2. **Install root dependencies**
```bash
npm install
```

3. **Set up Backend**
```bash
cd backend
npm install

# Create environment file
cp .env.example .env
# Edit .env with your MongoDB URI and other settings
```

4. **Set up Frontend**
```bash
cd ../frontend
npm install

# Create environment file
cp .env.example .env
# Edit .env with your API URL and other settings
```

5. **Start Development Servers**

Backend (Terminal 1):
```bash
cd backend
npm run dev
```

Frontend (Terminal 2):
```bash
cd frontend
npm run dev
```

The application will be available at:
- Frontend: http://localhost:5173
- Backend: http://localhost:5000

## 📁 Project Structure

```
RoutePool/
├── backend/
│   ├── src/
│   │   ├── config/         # Database and app configuration
│   │   ├── controllers/    # Route handlers
│   │   ├── middleware/     # Custom middleware
│   │   ├── models/         # Database models
│   │   └── routes/         # API routes
│   ├── server.js          # Server entry point
│   └── package.json
├── frontend/
│   ├── public/            # Static assets
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/         # Page components
│   │   ├── services/      # API services
│   │   ├── hooks/         # Custom hooks
│   │   ├── utils/         # Utility functions
│   │   └── assets/        # Images, icons, etc.
│   ├── index.html
│   └── package.json
└── README.md
```

## 🔧 Configuration

### Environment Variables

**Backend (.env)**
```env
NODE_ENV=development
PORT=5000
MONGO_URI=mongodb://localhost:27017/cogo
JWT_SECRET=your-super-secret-jwt-key
SESSION_SECRET=your-session-secret
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
CLIENT_URL=http://localhost:5173
```

**Frontend (.env)**
```env
VITE_API_URL=http://localhost:5000/api
VITE_APP_NAME=RoutePool
VITE_GOOGLE_CLIENT_ID=your-google-client-id
```



## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.






