# NyayaSulabh - Accessible Justice Platform

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![n8n](https://img.shields.io/badge/n8n-FF6B35?style=flat&logo=n8n&logoColor=white)](https://n8n.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white)](https://www.postgresql.org/)

> **Democratizing Justice Through AI** 🚀

NyayaSulabh is an AI-powered legal document analysis platform designed to democratize access to justice by simplifying complex legal documents. Using cutting-edge AI and natural language processing, it transforms dense legal jargon into clear, understandable summaries and provides multilingual support for users worldwide.

## 📋 Table of Contents

- [🚀 Features](#-features)
- [🛠️ Technologies Used](#️-technologies-used)
- [📋 Prerequisites](#-prerequisites)
- [🔧 Installation & Setup](#-installation--setup)
- [📖 Usage](#-usage)
- [🔌 API/Webhook Details](#-apiwebhook-details)
- [🤝 Contributing](#-contributing)
- [📞 Contact & Support](#-contact--support)
- [🙏 Acknowledgments](#-acknowledgments)

## 🚀 Features

### Core Functionality
- 🤖 **AI-Powered Document Analysis**: Leverages Google Gemini AI to analyze legal documents and extract key information
- 🌍 **Multilingual Support**: Supports English, Hindi, and Marathi for document translation and summaries
- 📄 **Document Upload & Processing**: Upload PDF, DOC, DOCX, and TXT files for instant analysis
- 💬 **Interactive Q&A**: Ask context-aware questions about uploaded documents
- ⚡ **Real-time Summarization**: Generate concise summaries of legal texts in multiple languages
- 🎤 **Voice Input Support**: Record and process voice queries for accessibility

### User Management
- 🔐 **Secure Authentication**: JWT-based user authentication with session management
- 📝 **User Registration & Login**: Multi-step signup process with password strength validation
- 👤 **Profile Management**: User dashboard with session tracking

### Technical Features
- 🔍 **RAG-Based Validation**: Retrieval-Augmented Generation for accurate legal information grounding
- 📱 **Responsive Design**: Mobile-first design that works across all devices
- 💬 **Real-time Chat Interface**: Interactive AI assistant with typing indicators
- 🖱️ **Drag & Drop Upload**: Intuitive file upload with progress feedback
- ⚠️ **Error Handling**: Comprehensive error handling and user feedback

## 🛠️ Technologies Used

| Category | Technologies |
|----------|--------------|
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) HTML5, ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) CSS3, ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) JavaScript (ES6+), Font Awesome |
| **Backend & Infrastructure** | ![n8n](https://img.shields.io/badge/n8n-FF6B35?style=flat&logo=n8n&logoColor=white) n8n, ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white) PostgreSQL, 
| **AI & APIs** | Google Gemini API, Webhook APIs |

## 📋 Prerequisites

Before running this project, ensure you have the following installed:

- 🔄 **n8n** (latest version)
- 🗄️ **PostgreSQL** database
- 📦 **Git** for version control

## 🔧 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/nyayasulabh.git
cd nyayasulabh
```

### 2. Set Up n8n Workflows
- Install n8n globally:
  ```bash
  npm install -g n8n
  ```
- Start n8n:
  ```bash
  n8n
  ```
- Import the workflow file:
  - Open n8n in your browser (usually http://localhost:5678)
  - Import the `User Authentication` and `Summarization_n8n.json` file
  - Configure the following credentials:
    - PostgreSQL: Set up connection to your Postgres database
    - Google Gemini API: Add your API key

### 3. Database Setup
- Create a PostgreSQL database named `nyayasulabh`
- Run the following SQL to create the users table:

### 4. Configure Environment Variables
- Create a `.env` file in your n8n directory with:

### 5. Start the Application
- Open the HTML files in a web browser, or serve them using a local server:
  - Access the application at http://localhost:8000/index.html

## 📖 Usage
### Getting Started
- Visit the Landing Page: Open `index.html` to explore the platform features
- Sign Up: Create a new account using the multi-step registration form
- Login: Authenticate using your credentials

### Using the AI Assistant
- Upload Documents: Click the upload button or drag & drop legal documents
- Ask Questions: Type questions about the document or use voice input
- Get Summaries: Request document summaries in your preferred language
- Multilingual Support: Switch between English, Hindi, and Marathi

### Example Queries
- "Summarize this rental agreement"
- "What are the key clauses in this contract?"
- "Translate this document to Hindi"
- "Explain the legal terms in simple language"

## 🔌 API/Webhook Details
### Authentication Endpoints
- `POST /auth`: Handles signup, login, validation, and logout
  - Operations: signup, login, validate, logout
  - Requires: email, password (for signup/login), token (for validation/logout)

### Document Processing Endpoints
- `POST /query`: Main query processing with AI analysis
  - Accepts: Text queries, voice audio, language preferences
- `POST /webhook/rag-upload`: Document upload for RAG processing
- `POST /webhook/summary-upload`: Document upload for summarization

### Response Formats
- All endpoints return JSON responses with:

## 🤝 Contributing
We welcome contributions to NyayaSulabh! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Commit your changes: `git commit -am 'Add new feature'`
5. Push to the branch: `git push origin feature-name`
6. Submit a pull request

### Development Guidelines
- Follow HTML/CSS/JS best practices
- Ensure responsive design across all devices
- Test authentication flows thoroughly
- Add comments for complex logic
- Update documentation for new features

## 📞 Contact & Support
- Email: contact@nyayasulabh.com
- Website: [[Your website URL](https://nyay-sulabh.vercel.app/)]
- GitHub Issues: For bug reports and feature requests

## 🙏 Acknowledgments
- Google Gemini AI for powering the document analysis
- n8n for workflow automation
- Font Awesome for icons
- Unsplash for hero images

> **Note**: This platform provides informational responses only and does not constitute legal advice. Always consult with qualified legal professionals for legal matters.

Built with ❤️ for accessible justice worldwide
