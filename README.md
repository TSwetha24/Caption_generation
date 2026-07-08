# Smart Captions Generation
An AI-powered web application that generates engaging captions from uploaded videos using speech transcription and generative AI. The application automatically extracts audio, transcribes speech, and creates captions suitable for social media platforms.

## Features

* Upload video files
* Automatic audio extraction from videos
* AI-powered speech-to-text transcription
* AI-generated captions based on video content
* User-friendly and responsive interface
* Frontend and backend integration
* Cloud deployment support

## Tech Stack
### Frontend
* React.js
* HTML5
* CSS3
* JavaScript
### Backend
* Node.js
* Express.js
* Multer (File Upload)
* FFmpeg (Audio Extraction)
* Whisper.cpp / Tiny Model (Speech Transcription)
* Google Gemini API (Caption Generation)
* CORS
* dotenv
* 
## Project Structure
Smart_Captions/
│
├── frontend/
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── uploads/
│   ├── routes/
│   ├── services/
│   ├── app.js
│   ├── package.json
│   └── .env
│
└── README.md
```
## Installation

### Clone the Repository

```bash
git clone https://github.com/TSwetha24/Caption_generation.git
cd Caption_generation
```

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the backend folder.

```env
GEMINI_API_KEY=YOUR_GEMINI_API_KEY
PORT=5000
```

Start the backend server.

```bash
npm start
```
---

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

The application will run at:

```
http://localhost:3000
```

## How It Works

1. Upload a video.
2. The backend extracts audio using FFmpeg.
3. The audio is transcribed using Whisper Tiny.
4. The transcript is sent to the Gemini API.
5. AI generates engaging captions.
6. Captions are displayed on the frontend.

## API Endpoint

### Generate Caption

```
POST /upload
```

#### Request

* Content-Type: multipart/form-data
* Parameter:

  * `video` – Video file

#### Response

```json
{
  "transcription": "...",
  "captions": [
    "Caption 1",
    "Caption 2",
    "Caption 3"
  ]
}
```

## Deployment

### Frontend

Vercel

https://caption-generation-two.vercel.app/

### Backend

Render

https://caption-generation-backend.onrender.com

## Screenshots

<img width="1812" height="951" alt="image" src="https://github.com/user-attachments/assets/8e2aa470-b5fa-4c73-b22e-b5ce900c6276" />
<img width="940" height="447" alt="image" src="https://github.com/user-attachments/assets/d7be72e4-17c2-4230-b06a-ac82d015c3e5" />
<img width="940" height="717" alt="image" src="https://github.com/user-attachments/assets/11efaa76-9f22-49e6-9285-a01e4aff11e4" />
<img width="940" height="497" alt="image" src="https://github.com/user-attachments/assets/bed79c97-7e30-4ed5-8dae-7d6e89372b84" />
<img width="940" height="914" alt="image" src="https://github.com/user-attachments/assets/2fdbb65e-f5c7-4c61-aa6c-dac9b5608c36" />


## Future Enhancements

* Caption download feature
* Social media sharing
* User authentication
* Caption history

## GitHub Repository

https://github.com/TSwetha24/Caption_generation

## License

This project is developed for educational and academic purposes.
