# Mentora Project Documentation

## Overview
Mentora is a comprehensive AI-powered educational assistant featuring multiple specialized study modes (Math, Coding, Business, Law, Literature), smart note-taking, PDF summarization, flashcards with spaced repetition, and contextual AI features.

## Recent Changes
- **2025-01-01**: Created GitHub-friendly repository structure with comprehensive documentation
- **2024-12-30**: Implemented contextual AI features ("Explain like I'm 5" and "Real-Life Analogy") that appear after AI responses
- **2024-12-30**: Enhanced responsive design and dark mode compatibility
- **2024-12-30**: Optimized PDF export system for professional document generation
- **2024-12-30**: Removed duplicate quick action buttons, streamlined UI

## Project Architecture

### Frontend Structure
- **React 18** with TypeScript for type safety
- **Tailwind CSS** for responsive styling with dark mode support
- **Shadcn/ui** components for consistent UI elements
- **Wouter** for client-side routing
- **React Query** for server state management
- **Framer Motion** for smooth animations

### Backend Structure
- **Express.js** server with TypeScript
- **Drizzle ORM** for database operations
- **Memory storage** for development (PostgreSQL support available)
- **RESTful API** design with proper error handling

### Key Features
1. **Multi-Mode AI Chat**: Specialized responses for different academic domains
2. **PDF Processing**: Text extraction and AI summarization
3. **Smart Notes**: AI-assisted note-taking with export capabilities
4. **Flashcard System**: Spaced repetition for optimal learning
5. **Study Planner**: AI-generated personalized learning schedules
6. **Contextual AI**: Post-response simplification and analogy features

### AI Integration
- **Google Gemini API** for intelligent responses
- **Context-aware prompts** based on selected study mode
- **OCR support** for image text extraction
- **Error handling** with graceful degradation

## User Preferences
- **Communication Style**: Professional and educational focus
- **UI Design**: Clean, responsive, accessibility-conscious
- **Features Priority**: AI accuracy, user experience, mobile compatibility
- **Code Style**: TypeScript strict mode, functional components, clear interfaces

## Development Guidelines

### Code Standards
- Use TypeScript interfaces for all components
- Implement responsive design (mobile-first approach)
- Support both light and dark modes
- Include proper error handling and loading states
- Follow existing component patterns

### Git Workflow
- Main branch for production-ready code
- Feature branches for new development
- Comprehensive commit messages using conventional format
- Pull request reviews required

### Deployment
- Optimized for Replit Deployments
- Environment variables configured via .env
- Build process handles frontend/backend integration
- Professional error handling for production

## Technical Decisions

### Why Memory Storage
- Simplifies development and deployment
- Easy migration to PostgreSQL when needed
- Reduces infrastructure complexity
- Faster development iteration

### Why Google Gemini
- Strong educational content generation
- Good context understanding
- Reliable API performance
- Cost-effective for educational use

### Why Shadcn/ui
- Consistent design system
- Accessibility built-in
- Dark mode support
- Customizable components

## GitHub Repository Structure
- Comprehensive README with setup instructions
- Contributing guidelines for open source collaboration
- Issue templates for bugs and feature requests
- CI/CD workflow for automated testing
- MIT license for open source distribution
- Proper .gitignore for clean repository

## Future Considerations
- Enhanced collaboration features
- Advanced analytics and progress tracking
- Integration with learning management systems
- Multi-language support
- Voice interaction capabilities