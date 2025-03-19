# EduAssist - Educational Management System

A full-stack educational management system built with React, Node.js, Express, and Firebase.

## Features

- User authentication (Teachers and Students)
- Class management
- Assignment creation and tracking
- Student progress monitoring
- Real-time analytics
- Invitation system for class enrollment

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Firebase account and project
- Git

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/eduassist.git
cd eduassist
```

2. Install server dependencies:
```bash
npm install
```

3. Install client dependencies:
```bash
cd client
npm install
cd ..
```

4. Set up environment variables:
   - Create `.env` file in the server directory
   - Create `.env` file in the client directory
   - Add necessary environment variables (see `.env.example` files)

5. Set up Firebase:
   - Create a Firebase project
   - Download your serviceAccountKey.json and place it in the server directory
   - Configure Firebase in the client (see Firebase setup documentation)

## Configuration

### Server Environment Variables (.env)
```
PORT=5001
NODE_ENV=development
```

### Client Environment Variables (.env)
```
REACT_APP_SERVER_PORT=5001
REACT_APP_FIREBASE_API_KEY=your_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=your_auth_domain
REACT_APP_FIREBASE_PROJECT_ID=your_project_id
REACT_APP_FIREBASE_STORAGE_BUCKET=your_storage_bucket
REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
REACT_APP_FIREBASE_APP_ID=your_app_id
```

## Running the Application

1. Development mode (runs both server and client):
```bash
npm run dev
```

2. Run server only:
```bash
npm run server
```

3. Run client only:
```bash
npm run client
```

## Project Structure

```
eduassist/
├── client/                 # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/        # Page components
│   │   ├── services/     # API services
│   │   ├── context/      # React context
│   │   └── utils/        # Utility functions
│   └── package.json
├── server/                # Node.js backend
│   ├── routes/           # API routes
│   ├── middleware/       # Express middleware
│   ├── index.js         # Server entry point
│   └── serviceAccountKey.json
└── package.json
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Security Notes

- Never commit sensitive information like API keys or service account files
- Always use environment variables for sensitive data
- Keep your dependencies updated
- Follow security best practices for Firebase and Node.js

## License

This project is licensed under the MIT License - see the LICENSE file for details 
