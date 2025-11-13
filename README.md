# 📱 SmartCoach — AI-Powered Personal Coaching App

SmartCoach is a full-stack AI personal development assistant that helps users achieve their goals through actionable 3-day plans.

## 🎯 Overview

SmartCoach generates personalized 3-day action plans for any goal using AI. Built with React Native for mobile, Node.js for the backend, and powered by OpenAI's GPT-4o-mini, it runs directly on physical iPhones using Expo Go.

## ✨ Features

### Mobile App (React Native + Expo)
- Clean and intuitive UI
- Input field for personal goals
- "Generate 3-Day Plan" button
- Real-time AI responses displayed on-device

### Backend (Node.js + Express)
- REST API endpoint: `POST /coach`
- Secure `.env` API key handling
- JSON body parsing
- CORS enabled for mobile device access

### AI Integration
- Uses OpenAI `gpt-4o-mini`
- Produces actionable, structured 3-day plans
- Prompt designed for clarity and usefulness

## 📸 Screenshot

*Replace with your own screenshot from Expo Go*

```
[ Insert screenshot here ]
```

## 🗂 Project Structure

```
smartcoach/
│
├── smartcoach-app/          # React Native frontend
│   ├── app/
│   ├── assets/
│   ├── components/
│   ├── package.json
│   └── ...
│
├── smartcoach-api/          # Node.js backend (Express + OpenAI)
│   ├── server.js
│   ├── package.json
│   ├── .env                 # (ignored by Git)
│   └── ...
│
└── .gitignore               # ignores node_modules and .env
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Expo Go app installed on your iPhone
- OpenAI API key

### 📲 Running the Mobile App (Frontend)

1. **Install dependencies**
   ```bash
   cd smartcoach/smartcoach-app
   npm install
   ```

2. **Start Expo**
   ```bash
   npx expo start
   ```

3. **Run on iPhone**
   - Install Expo Go from the App Store
   - Scan the QR code printed in the terminal

### 🛠 Running the Backend (Express Server)

1. **Install dependencies**
   ```bash
   cd smartcoach/smartcoach-api
   npm install
   ```

2. **Add your OpenAI API key**
   
   Create a `.env` file in the `smartcoach-api` directory:
   ```env
   OPENAI_API_KEY=sk-proj-xxxxxx
   ```

3. **Start the server**
   ```bash
   node server.js
   ```

   Server runs at: `http://localhost:8080`

## 🌐 API Documentation

### POST /coach

Generate a 3-day coaching plan.

**Request Body:**
```json
{
  "goal": "I want to improve my study habits"
}
```

**Response:**
```json
{
  "plan": "Day 1: ...\nDay 2: ...\nDay 3: ..."
}
```

## 🧠 How It Works

1. User enters a personal goal in the mobile app
2. React Native app sends the goal to `/coach` endpoint
3. Express backend forwards the request to OpenAI API
4. OpenAI returns a structured 3-day plan
5. The mobile app displays the plan in real time

## ⚙️ Tech Stack

### Frontend
- React Native
- Expo
- JavaScript
- Fetch API

### Backend
- Node.js
- Express
- CORS
- dotenv
- OpenAI API

## 🚧 Future Enhancements

- [ ] Chat-based coaching mode
- [ ] User accounts / authentication
- [ ] Progress tracking
- [ ] MongoDB integration
- [ ] Voice input + speech output
- [ ] Coaching categories (fitness, study, career, etc.)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Ethan** ([@xyydcoldcold](https://github.com/xyydcoldcold))

- Computer Science @ University of Toronto
- Full-stack & AI application developer

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## ⭐️ Show your support

Give a ⭐️ if this project helped you!

---

*Built with ❤️ using React Native, Node.js, and OpenAI*
