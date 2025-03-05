# AI-Driven Healthcare Chatbot for Patient Triage and Support

## Overview
**AI-Driven Healthcare Chatbot** is an intelligent chatbot designed to assist patients by providing initial triage, symptom analysis, and medical support. The chatbot integrates **React.js, Node.js, Express.js, MongoDB, and Gemini API** to provide an interactive, responsive, and efficient healthcare assistant.

## Features
- **Symptom Analysis:** Identifies potential health conditions based on user input.
- **AI-Powered Responses:** Uses the Gemini API for intelligent recommendations.
- **User Authentication:** Secure login and patient data management.
- **Medical History Tracking:** Stores past interactions for better diagnosis.
- **Emergency Alert System:** Notifies healthcare providers in critical situations.
- **Responsive UI:** Optimized for mobile and desktop use.
- **Database Storage:** Patient interactions securely stored in MongoDB.


## Tech Stack
- **Frontend:** React.js
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **AI API:** Gemini API

## Installation Guide
### Prerequisites
- Install **Node.js** and **MongoDB**
- Basic knowledge of React.js and Express.js
- API Key from **Gemini API**

### Steps to Set Up the Project
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/healthcare-chatbot.git
   cd healthcare-chatbot
   ```
2. **Install Dependencies:**
   ```bash
   npm install
   ```
3. **Setup Environment Variables:**
   - Create a `.env` file and add:
   ```
   MONGO_URI=your_mongodb_connection_string
   GEMINI_API_KEY=your_gemini_api_key
   ```
4. **Start MongoDB:**
   ```bash
   mongod
   ```
5. **Run the Backend Server:**
   ```bash
   node server.js
   ```
6. **Start the Frontend:**
   ```bash
   cd client
   npm start
   ```
7. **Access the Application:**
   - Open `http://localhost:3000/` in your browser.



## How It Works
1. **User Input:**
   - The chatbot asks users about their symptoms.
2. **AI-Powered Analysis:**
   - Uses the **Gemini API** to analyze symptoms.
3. **Recommendations & Support:**
   - Suggests possible conditions and next steps.
4. **Emergency Alerts:**
   - Notifies healthcare professionals if necessary.
5. **Medical History Storage:**
   - Saves past interactions for better future recommendations.

## Sample Code for Express.js API
```javascript
const express = require('express');
const router = express.Router();
const { analyzeSymptoms } = require('../controllers/chatbotController');

router.post('/analyze', analyzeSymptoms);

module.exports = router;
```










