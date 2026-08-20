# PrepForge AI
PrepForge AI is a full-stack AI-powered interview preparation platform that helps candidates prepare for job interviews by analyzing their resume, self-description, and target job description.
The platform uses Google's Gemini API to generate personalized interview reports, including job match scores, technical and behavioral questions, skill gaps, and a day-wise preparation plan. It also provides AI-generated ATS-friendly resumes that can be downloaded as PDF files.


## 🚀 Live Demo
https://prepforge-ai-six.vercel.app


## 📂 GitHub Repository
https://github.com/rounakbhardwaj01/PrepForge-AI


## ✨ Features
- User registration and login
- JWT-based authentication
- HTTP-only cookie-based authentication
- Protected routes
- Resume PDF upload
- Job description and self-description input
- AI-powered interview report generation
- Resume-to-job matching score
- Technical interview questions
- Behavioral interview questions
- Skill-gap analysis
- Personalized day-wise preparation plan
- Interview report history
- AI-generated ATS-friendly resumes
- Resume PDF generation
- Responsive user interface



## 🛠️ Tech Stack

### Frontend
- React.js
- React Router
- Redux Toolkit
- SCSS
- Tailwind CSS
- Axios
- Vite

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcryptjs
- Cookie Parser
- Multer

### AI & PDF Generation
- Google Gemini API
- Zod
- Zod-to-JSON-Schema
- Puppeteer
- PDF parsing

### Deployment
- Frontend: Vercel
- Backend: Render
- Database: MongoDB


## 🏗️ Project Structure

```
PrepForge AI/
│
├── Backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middlewares/
│   │   ├── models/
│   │   ├── routes/
│   │   └── services/
│   │
│   ├── server.js
│   ├── package.json
│   └── .gitignore
│
├── Frontend/
│   ├── src/
│   │   ├── features/
│   │   │   ├── auth/
│   │   │   └── interview/
│   │   ├── App.jsx
│   │   ├── app.routes.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```


🔄 How It Works
```
User
  │
  ├── Register / Login
  │
  ▼
Authentication
  │
  ▼
Enter Job Description
+ Self Description
+ Upload Resume
  │
  ▼
Backend API
  │
  ▼
Google Gemini API
  │
  ▼
Structured Interview Report
  │
  ├── Match Score
  ├── Technical Questions
  ├── Behavioral Questions
  ├── Skill Gaps
  └── Preparation Plan
  │
  ▼
MongoDB
  │
  ▼
Interview Report
```


For resume generation:
```
Interview Report
      │
      ▼
Google Gemini API
      │
      ▼
ATS-friendly HTML Resume
      │
      ▼
Puppeteer
      │
      ▼
PDF Resume
      │
      ▼
Download
```


🔐 Authentication

PrepForge AI uses JWT-based authentication with HTTP-only cookies.

The authentication system includes:

User registration
Password hashing using bcrypt
Login authentication
JWT token generation
Protected backend routes
HTTP-only authentication cookies
Logout and token blacklisting



🤖 AI Integration

Google Gemini API is used to analyze candidate information and generate structured interview preparation data.
Zod is used to define the expected structure of AI responses, helping maintain consistent and predictable output from the AI service.

The generated report contains:

Candidate-job match score
Technical interview questions
Behavioral interview questions
Skill gaps
Personalized preparation plan



📄 AI Resume Generation

PrepForge AI can generate an ATS-friendly resume based on:

Candidate resume information
Self-description
Target job description

The AI generates structured HTML content, which is then converted into a PDF using Puppeteer.



⚙️ LocalSetup
Prerequisites

Make sure you have installed:

Node.js
npm
MongoDB
Git



1. Clone the repository
git clone https://github.com/rounakbhardwaj01/PrepForge-AI.git
cd PrepForge-AI

2. Setup Backend
cd Backend
npm install

Create a .env file inside the Backend directory:
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GOOGLE_GENAI_API_KEY=your_google_gemini_api_key

Start the backend:
npm run dev
The backend will run on:
http://localhost:3000



3. Setup Frontend
Open another terminal:
cd Frontend
npm install


Create a .env file inside the Frontend directory:

VITE_API_URL=http://localhost:3000

Start the frontend:
npm run dev

The frontend will run on:
http://localhost:5173



🌐 Deployment

Frontend
The React frontend is deployed using Vercel.

Backend
The Node.js/Express backend is deployed using Render.

Environment variables are configured separately in the deployment platforms to keep sensitive credentials out of the source code.


🔒 Environment Variables
Never commit .env files or API keys to GitHub.

Required backend variables:

PORT=
MONGO_URI=
JWT_SECRET=
GOOGLE_GENAI_API_KEY=

Required frontend variable:

VITE_API_URL=
🎯 Future Improvements
Real-time mock interview mode
Voice-based interview practice
More detailed resume analytics
Interview performance tracking
Additional AI-powered career recommendations
Improved PDF resume templates


👨‍💻 Author

Rounak Bhardwaj

GitHub: https://github.com/rounakbhardwaj01

LinkedIn: https://linkedin.com/in/rounak-bhardwaj01/
