📱 SmartCoach — AI-Powered Personal Coaching App

SmartCoach is a full-stack AI personal development assistant built with:

React Native (Expo) — mobile app

Node.js + Express — backend API

OpenAI GPT-4o-mini — AI engine

It generates personalized 3-day action plans for any goal the user enters.
The app runs directly on a physical iPhone using Expo Go.

🚀 Features
Mobile App (React Native + Expo)

Clean and intuitive UI

Input field for personal goals

“Generate 3-Day Plan” button

Real-time AI responses displayed on-device

Backend (Node.js + Express)

REST API endpoint: POST /coach

Secure .env API key handling

JSON body parsing

CORS enabled for mobile device access

AI Integration

Uses OpenAI gpt-4o-mini

Produces actionable, structured 3-day plans

Prompt designed for clarity and usefulness

📸 Screenshot (Example)

Replace this with your own screenshot from Expo Go.

[ Insert screenshot here ]

🗂 Project Structure
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

📲 Running the Mobile App (Frontend)
1. Install dependencies
cd smartcoach/smartcoach-app
npm install

2. Start Expo
npx expo start

3. Run on iPhone

Install Expo Go from the App Store

Scan the QR code printed in the terminal

🛠 Running the Backend (Express Server)
1. Install dependencies
cd smartcoach/smartcoach-api
npm install

2. Add your OpenAI API key

Create .env:

OPENAI_API_KEY=sk-proj-xxxxxx

3. Start the server
node server.js


Server runs at:

http://localhost:8080

🌐 API Endpoint
POST /coach

Generate a 3-day coaching plan.

Request Example
{
  "goal": "I want to improve my study habits"
}

Response Example
{
  "plan": "Day 1: ...\nDay 2: ...\nDay 3: ..."
}

🧠 How It Works

User enters a personal goal

React Native app sends it to /coach

Express backend forwards it to OpenAI

OpenAI returns a structured plan

The mobile app displays it in real time

⚙️ Tech Stack
Frontend

React Native

Expo

JavaScript / TypeScript

Fetch API

Backend

Node.js

Express

CORS

dotenv

OpenAI API

🚧 Future Enhancements

Chat-based coaching mode

User accounts / authentication

Progress tracking

MongoDB integration

Voice input + speech output

Coaching categories (fitness, study, career, etc.)

👤 Author

Ethan (xyydcoldcold)
Computer Science @ University of Toronto
Full-stack & AI application developer
