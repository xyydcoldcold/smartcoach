📱 SmartCoach — AI-Powered Personal Coaching App

SmartCoach is a full-stack AI personal development assistant built with React Native (Expo) and a Node.js + Express backend powered by the OpenAI API.
It runs directly on your iPhone and generates actionable 3-day personal improvement plans for any goal the user enters.

This project demonstrates end-to-end mobile + backend integration suitable for production-grade AI applications.

🚀 Features
Mobile App (React Native + Expo)

Clean and modern UI

Text input for personal goals

“Generate 3-Day Plan” button

Real-time AI-generated responses

Auto-refresh on save

Tested on physical iPhone device

Backend (Node.js + Express)

REST API endpoint: POST /coach

Integrates directly with OpenAI chat completions

JSON request/response handling

Environment variable support using .env

CORS enabled for device communication

AI Integration

Uses OpenAI’s gpt-4o-mini model

Produces structured, actionable 3-day coaching plans

Prompts designed for clarity, motivation, and practical steps

📸 Screenshots
Mobile App Running on Real Device
<img src="YOUR_SCREENSHOT_HERE" width="300">

Replace with your actual screenshot from Expo Go.

🏗️ Project Structure
smartcoach/
│
├── smartcoach-app/      # React Native frontend (Expo)
│   ├── app/
│   ├── components/
│   ├── assets/
│   ├── package.json
│   └── ...
│
├── smartcoach-api/      # Node.js backend (Express + OpenAI)
│   ├── server.js
│   ├── package.json
│   ├── .env             # (ignored)
│   └── ...
│
└── .gitignore           # ignores node_modules and secrets

📲 Running the Mobile App
1. Install dependencies
cd smartcoach/smartcoach-app
npm install

2. Start Expo
npx expo start

3. Run on iPhone

Install Expo Go from the App Store

Scan the QR code

App loads instantly on device

🛠️ Running the Backend
1. Install dependencies
cd smartcoach/smartcoach-api
npm install

2. Add your API key

Create a .env file:

OPENAI_API_KEY=sk-proj-xxxxxx

3. Start the server
node server.js


Server runs on:

http://localhost:8080

🌐 API Documentation
POST /coach

Generate a 3-day personal development plan.

Request
{
  "goal": "I want to improve my study habits"
}

Response
{
  "plan": "Day 1: ...\nDay 2: ...\nDay 3: ..."
}

🧠 How It Works (Architecture)

1. User enters a goal in the React Native app
↓
2. App sends goal to Express backend (/coach endpoint)
↓
3. Backend sends prompt to OpenAI API
↓
4. OpenAI generates a structured coaching plan
↓
5. Backend returns plan to mobile app
↓
6. App displays the personalized plan on the iPhone

📦 Tech Stack
Frontend

React Native

Expo CLI

TypeScript

Hooks (useState)

Fetch API

Backend

Node.js

Express

CORS

dotenv

OpenAI API (chat completions)

Tools

Git / GitHub

macOS + iPhone (physical device)

Xcode (device integration)

Expo Go

🎯 Why This Project Matters

This project showcases:

Full-stack development (mobile + server)

API design and backend engineering

AI integration in real-world apps

Mobile UI development with React Native

Real-device iOS debugging and deployment

Secure environment variable setup

Perfect for roles involving:

MERN stack

Mobile development

AI application development

Software engineering internships / co-ops

📝 Possible Future Enhancements

Chat-based coaching mode

User authentication (Google/Apple login)

Progress tracking with a timeline

MongoDB integration for saved goals

Voice input + text-to-speech

Custom coaching personas

Push notifications

👤 Author

Ethan (xyydcoldcold)
Full-stack developer, AI enthusiast, Computer Science student at University of Toronto.
Experienced in React Native, Node.js, Express, Python, Git, and applied AI systems.

If you'd like, I can also:

✔ Add your screenshot
✔ Add badges, shields, icons
✔ Add a diagram of your backend flow
✔ Add instructions for building a standalone iOS IPA

Just tell me!
