# 🤖 Indic AI Chatbot

A powerful multilingual AI chatbot supporting 10 Indian languages with advanced features including voice interaction, PDF document analysis, web search integration, and real-time screen sharing capabilities.

![Languages](https://img.shields.io/badge/Languages-10-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

### 🌐 Multilingual Support
- **10 Indian Languages**: Hindi, Tamil, Bengali, Gujarati, Marathi, Telugu, Kannada, Malayalam, Punjabi, and English
- Seamless language switching with i18next internationalization
- Native language text-to-speech and speech-to-text support

### 💬 Multiple Chat Modes
1. **Standard Chat**: General conversational AI powered by Google Gemini
2. **File Chat**: Upload and query PDF documents with context-aware responses
3. **Web Search**: Real-time web search integration for up-to-date information
4. **Live Screen**: Screen sharing with real-time AI assistance via WebSocket

### 🎙️ Voice Interaction
- **Speech-to-Text**: Convert voice input to text using Sarvam AI
- **Text-to-Speech**: Natural voice responses in multiple Indian languages
- Real-time audio processing and playback

### 📄 Document Intelligence
- PDF upload and analysis
- Context-aware question answering from documents
- Persistent file storage with UUID-based identification

### 🔍 Web Search Integration
- Real-time information retrieval using Google Search
- Fallback mechanisms for quota management
- Enhanced responses with current web data

## 🛠️ Tech Stack

### Frontend
- **React 19** - Modern UI library
- **Vite** - Fast build tool and dev server
- **TailwindCSS** - Utility-first CSS framework
- **DaisyUI** - Component library for Tailwind
- **i18next** - Internationalization framework
- **marked** - Markdown parser for rich text rendering

### Backend
- **Python 3.x** - Core programming language
- **FastAPI** - High-performance web framework
- **WebSockets** - Real-time bidirectional communication
- **Uvicorn** - ASGI server

### AI/ML Services
- **Google Generative AI (Gemini)** - Advanced language model for conversations and document analysis
- **Sarvam AI** - Indian language TTS/STT services
- **OpenCV** - Computer vision for screen capture
- **PyAudio** - Audio I/O processing

## 📋 Prerequisites

- **Node.js** (v18 or higher)
- **Python** (v3.8 or higher)
- **pip** (Python package manager)
- **Google Generative AI API Key**
- **Sarvam AI API Key**

## 🚀 Installation

### 1. Clone the Repository
```bash
git clone https://github.com/JayDaftardar/indic-chat-bot.git
cd indic-chat-bot
```

### 2. Backend Setup

```bash
# Navigate to backend directory
cd backend

# Install Python dependencies
pip install -r requirements.txt

# Create .env file and add your API keys
# Create a .env file with the following:
# GOOGLE_API_KEY=your_google_api_key_here
# SARVAM_API_KEY=your_sarvam_api_key_here
```

### 3. Frontend Setup

```bash
# Navigate to frontend directory
cd ../frontend

# Install Node dependencies
npm install
```

## 🎯 Running the Application

### Start Backend Server
```bash
cd backend
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

The backend API will be available at `http://localhost:8000`

### Start Frontend Development Server
```bash
cd frontend
npm run dev
```

The frontend will be available at `http://localhost:5173`

## 📁 Project Structure

```
indic-chat-bot-main/
├── backend/
│   ├── main.py                 # FastAPI application entry point
│   ├── requirements.txt        # Python dependencies
│   ├── .env                    # Environment variables (API keys)
│   ├── services/               # Service modules
│   │   ├── llm_service.py     # LLM and AI processing
│   │   ├── tts_service.py     # Text-to-speech service
│   │   ├── stt_service.py     # Speech-to-text service
│   │   └── live_service.py    # WebSocket live chat service
│   ├── utils/                  # Utility functions
│   ├── tools/                  # Additional tools
│   └── uploads/                # PDF file storage
├── frontend/
│   ├── src/
│   │   ├── App.jsx            # Main application component
│   │   ├── components/        # React components
│   │   │   ├── ChatWindow.jsx
│   │   │   ├── ChatInput.jsx
│   │   │   ├── LiveScreenChat.jsx
│   │   │   └── ...
│   │   ├── i18n.js            # Internationalization config
│   │   └── index.css          # Global styles
│   ├── package.json           # Node dependencies
│   └── vite.config.js         # Vite configuration
└── README.md                   # This file
```

## 🔑 Environment Variables

Create a `.env` file in the `backend` directory:

```env
GOOGLE_API_KEY=your_google_generative_ai_api_key
SARVAM_API_KEY=your_sarvam_ai_api_key
```

### Getting API Keys

- **Google Generative AI**: Get your API key from [Google AI Studio](https://makersuite.google.com/app/apikey)
- **Sarvam AI**: Sign up at [Sarvam AI](https://www.sarvam.ai/) for Indian language services

## 📖 Usage

### Standard Chat
1. Select "Standard Chat" mode from the navbar
2. Choose your preferred language from the dropdown
3. Type your message or use voice input
4. Receive AI-generated responses in your selected language

### File Chat (PDF Analysis)
1. Switch to "File Chat" mode
2. Upload a PDF document using the file upload button
3. Ask questions about the document content
4. Get context-aware answers based on the PDF

### Web Search
1. Select "Web Search" mode
2. Ask questions requiring current information
3. Receive responses enhanced with real-time web data

### Live Screen Chat
1. Switch to "Live Screen" mode
2. Share your screen for real-time AI assistance
3. Get contextual help based on what's on your screen

## 🎨 Features in Detail

### Voice Interaction
- Click the microphone icon to start voice input
- Speak in any supported language
- Automatic transcription and response generation
- Text-to-speech playback of bot responses

### PDF Document Analysis
- Supports PDF file uploads
- Context-aware question answering
- Persistent file storage
- Multiple document support

### Multilingual Support
- Automatic language detection
- UI translation for all supported languages
- Native language voice synthesis
- Seamless language switching

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License.

## 👨‍💻 Author

**Jay Daftardar**
- GitHub: [@JayDaftardar](https://github.com/JayDaftardar)

## 🙏 Acknowledgments

- Google Generative AI for powerful language models
- Sarvam AI for Indian language TTS/STT services
- React and FastAPI communities for excellent frameworks

## 📞 Support

For issues, questions, or suggestions, please open an issue on GitHub.

---

Made with ❤️ for Indian language accessibility
