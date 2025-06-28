# Mentora Setup Guide

## Quick Start

### 1. Clone and Install
```bash
git clone https://github.com/yourusername/mentora.git
cd mentora
npm install
```

### 2. Environment Setup
```bash
cp .env.example .env
```

Edit `.env` and add your Google Gemini API key:
```env
VITE_GEMINI_API_KEY=your_actual_api_key_here
```

### 3. Start Development
```bash
npm run dev
```

Visit `http://localhost:5000` to see Mentora running!

## Getting Your API Key

### Google Gemini API
1. Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Sign in with your Google account
3. Click "Create API Key"
4. Copy the key and add it to your `.env` file

## Development Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run check` - TypeScript type checking
- `npm run lint` - Code linting

## Project Structure

```
mentora/
├── client/           # React frontend
│   ├── src/
│   │   ├── components/   # UI components
│   │   ├── pages/        # Route pages
│   │   ├── hooks/        # Custom hooks
│   │   ├── lib/          # Utilities
│   │   └── types/        # TypeScript types
├── server/           # Express backend
├── shared/           # Shared types/schemas
└── .github/          # GitHub templates
```

## Features Overview

### Study Modes
- **Math**: Equations, problem-solving, statistics
- **Coding**: Programming help, debugging, algorithms
- **Business**: Strategy, finance, marketing
- **Law**: Legal concepts, case analysis
- **Literature**: Writing, analysis, creativity

### Core Tools
- **AI Chat**: Contextual conversations with specialized responses
- **PDF Summarizer**: Extract and analyze document content
- **Smart Notes**: AI-assisted note-taking with export
- **Flashcards**: Spaced repetition learning system
- **Study Planner**: Personalized learning schedules

### Smart Features
- **Contextual Actions**: "Explain like I'm 5" and "Real-Life Analogy"
- **OCR Support**: Text extraction from images
- **Video Search**: Find educational content
- **Dark Mode**: Eye-friendly interface
- **Mobile Responsive**: Works on all devices

## Troubleshooting

### Common Issues

**Server won't start:**
- Check Node.js version (18+ required)
- Verify all dependencies installed: `npm install`
- Check for port conflicts (5000)

**AI features not working:**
- Verify Gemini API key in `.env`
- Check API key has proper permissions
- Ensure internet connection for API calls

**Build errors:**
- Run `npm run check` for TypeScript errors
- Clear node_modules and reinstall if needed
- Check for missing dependencies

### Getting Help
- Check [GitHub Issues](https://github.com/yourusername/mentora/issues)
- Review [Contributing Guide](CONTRIBUTING.md)
- Join [Discussions](https://github.com/yourusername/mentora/discussions)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

## License

MIT License - see [LICENSE](LICENSE) for details.