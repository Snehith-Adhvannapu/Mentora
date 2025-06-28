# Mentora - AI Educational Assistant

> Your intelligent AI companion for personalized learning across multiple domains

![Mentora Logo](https://img.shields.io/badge/Mentora-AI%20Education-blue?style=for-the-badge&logo=brain)

## 🚀 Features

### Multi-Modal AI Learning
- **Specialized Study Modes**: Math, Coding, Business, Law, and Literature
- **Contextual AI Responses**: Get explanations tailored to your chosen domain
- **Smart Simplification**: "Explain like I'm 5" for complex concepts
- **Real-World Analogies**: Connect abstract ideas to everyday experiences

### Study Tools
- **📚 PDF Summarizer**: Extract key insights from documents with AI analysis
- **🗒️ Smart Notes**: AI-powered note-taking with automatic organization
- **🃏 Flashcards**: Spaced repetition system for optimal memory retention
- **📋 Study Planner**: Personalized learning schedules with topic breakdown
- **💭 Doubt Resolution**: Ask questions and get detailed explanations

### Advanced Features
- **🎨 OCR Support**: Extract text from images for instant AI analysis
- **🔍 Video Search**: Find relevant educational videos for any topic
- **📱 Responsive Design**: Works seamlessly on desktop and mobile
- **🌙 Dark Mode**: Eye-friendly interface for extended study sessions
- **📄 PDF Export**: Professional document generation for notes and summaries

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS
- **Backend**: Express.js, Node.js
- **AI Integration**: Google Gemini API
- **Database**: PostgreSQL with Drizzle ORM
- **Build Tool**: Vite
- **UI Components**: Radix UI, Shadcn/ui
- **Animations**: Framer Motion

## 📦 Installation

### Prerequisites
- Node.js 18+ 
- npm or yarn
- PostgreSQL (optional, uses memory storage by default)

### Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/mentora.git
cd mentora
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
cp .env.example .env
```

4. **Configure your API keys**
Add your Google Gemini API key to the `.env` file:
```env
VITE_GEMINI_API_KEY=your_gemini_api_key_here
```

5. **Start the development server**
```bash
npm run dev
```

Visit `http://localhost:5000` to see your application running!

## 🚀 Deployment

### Replit Deployment (Recommended)
This project is optimized for Replit Deployments:

1. Import this repository to Replit
2. Configure your environment variables in Replit Secrets
3. Click "Deploy" to launch your application

### Manual Deployment
For other platforms:

```bash
npm run build
npm start
```

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `VITE_GEMINI_API_KEY` | Google Gemini API key for AI features | Yes |
| `DATABASE_URL` | PostgreSQL connection string | No (uses memory storage) |
| `NODE_ENV` | Environment mode (development/production) | No |

### Getting API Keys

#### Google Gemini API
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Add it to your environment variables

## 📚 Usage Guide

### Getting Started
1. **Choose Your Mode**: Select from Math, Coding, Business, Law, or Literature
2. **Start Learning**: Ask questions, upload PDFs, or create study materials
3. **Use Smart Features**: Try "Explain like I'm 5" or "Real-Life Analogy" buttons
4. **Organize Knowledge**: Save notes, create flashcards, and track progress

### Study Modes
- **📊 Math**: Equations, problem-solving, statistical analysis
- **💻 Coding**: Programming concepts, debugging, algorithm explanations
- **💼 Business**: Strategy, finance, marketing, management
- **⚖️ Law**: Legal concepts, case analysis, regulatory guidance
- **📖 Literature**: Analysis, writing, creative expression

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Setup
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes and test thoroughly
4. Commit your changes: `git commit -m 'Add amazing feature'`
5. Push to the branch: `git push origin feature/amazing-feature`
6. Open a Pull Request

### Code Style
- Use TypeScript for type safety
- Follow ESLint configuration
- Use Prettier for code formatting
- Write descriptive commit messages

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

- **Documentation**: Check our [Wiki](https://github.com/yourusername/mentora/wiki)
- **Issues**: [Report bugs or request features](https://github.com/yourusername/mentora/issues)
- **Discussions**: [Join our community](https://github.com/yourusername/mentora/discussions)

## 🙏 Acknowledgments

- Google Gemini for AI capabilities
- Shadcn/ui for beautiful components
- The open-source community for amazing tools

## 📊 Project Status

![GitHub release](https://img.shields.io/github/v/release/yourusername/mentora)
![GitHub issues](https://img.shields.io/github/issues/yourusername/mentora)
![GitHub stars](https://img.shields.io/github/stars/yourusername/mentora)
![GitHub license](https://img.shields.io/github/license/yourusername/mentora)

---

<div align="center">
  <strong>Built with ❤️ for learners everywhere</strong>
  <br>
  <br>
  <a href="https://mentora.replit.app">Live Demo</a> •
  <a href="#installation">Quick Start</a> •
  <a href="https://github.com/yourusername/mentora/wiki">Documentation</a>
</div>