# Contributing to Mentora

Thank you for your interest in contributing to Mentora! This guide will help you get started with development and contributing to the project.

## 🚀 Getting Started

### Development Environment
1. Fork and clone the repository
2. Install dependencies: `npm install`
3. Copy environment variables: `cp .env.example .env`
4. Add your Gemini API key to `.env`
5. Start development server: `npm run dev`

### Project Structure
```
mentora/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Route components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── lib/           # Utility libraries
│   │   └── types/         # TypeScript type definitions
├── server/                # Backend Express server
├── shared/                # Shared schemas and types
└── docs/                 # Documentation
```

## 🛠️ Development Guidelines

### Code Style
- Use TypeScript for all new code
- Follow the existing ESLint configuration
- Use Prettier for consistent formatting
- Components should be functional with hooks
- Use descriptive variable and function names

### Component Guidelines
- Use Shadcn/ui components when possible
- Implement responsive design (mobile-first)
- Support both light and dark modes
- Include proper TypeScript interfaces
- Add error handling and loading states

### Backend Guidelines
- Keep routes thin, logic in services
- Use Zod schemas for validation
- Implement proper error handling
- Follow RESTful conventions
- Use the storage interface pattern

## 📝 Commit Guidelines

### Commit Messages
Use conventional commits format:
```
type(scope): description

Examples:
feat(ai): add explain like I'm 5 feature
fix(ui): resolve mobile navigation issue
docs(readme): update installation instructions
refactor(api): improve error handling
```

### Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `test`: Adding tests
- `chore`: Maintenance tasks

## 🔍 Testing

### Before Submitting
- Test on both desktop and mobile
- Verify dark mode compatibility
- Check TypeScript compilation
- Test with and without API keys
- Ensure responsive design works

### Manual Testing Checklist
- [ ] All study modes work correctly
- [ ] PDF upload and processing
- [ ] Note creation and editing
- [ ] Flashcard functionality
- [ ] AI chat responses
- [ ] Mobile navigation
- [ ] Dark/light mode toggle

## 📋 Pull Request Process

### Before Creating PR
1. Create a feature branch from `main`
2. Make your changes with clear commits
3. Test thoroughly across devices
4. Update documentation if needed
5. Ensure no TypeScript errors

### PR Requirements
- Clear description of changes
- Link to related issues
- Screenshots for UI changes
- Confirmation of testing completed
- Updated documentation if applicable

### Review Process
1. Automated checks must pass
2. Code review by maintainers
3. Testing by reviewers
4. Approval and merge

## 🐛 Reporting Issues

### Bug Reports
Include:
- Clear description of the issue
- Steps to reproduce
- Expected vs actual behavior
- Screenshots/videos if applicable
- Browser and device information
- Console errors if any

### Feature Requests
Include:
- Clear description of the feature
- Use case and benefit
- Proposed implementation (if any)
- Mockups or examples (if applicable)

## 🎯 Areas for Contribution

### High Priority
- Performance optimizations
- Accessibility improvements
- Mobile UX enhancements
- Error handling improvements
- Documentation updates

### Feature Ideas
- Additional study modes
- Collaboration features
- Study analytics
- Integration with learning platforms
- Advanced AI interactions

### Technical Improvements
- Test coverage
- Performance monitoring
- Security enhancements
- Code organization
- CI/CD improvements

## 🏗️ Architecture Decisions

### Frontend
- React 18 with TypeScript
- Tailwind CSS for styling
- Radix UI for components
- Wouter for routing
- React Query for data fetching

### Backend
- Express.js with TypeScript
- Drizzle ORM for database
- Memory storage for development
- RESTful API design

### AI Integration
- Google Gemini API
- Contextual prompt engineering
- Mode-specific responses
- Error handling and fallbacks

## 📚 Resources

### Documentation
- [React Documentation](https://react.dev)
- [TypeScript Handbook](https://www.typescriptlang.org/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [Google Gemini API](https://ai.google.dev)

### Tools
- [Shadcn/ui Components](https://ui.shadcn.com)
- [Lucide Icons](https://lucide.dev)
- [Framer Motion](https://www.framer.com/motion)

## 💬 Communication

### Questions and Discussions
- Use GitHub Discussions for general questions
- Create issues for bugs and feature requests
- Join our community discussions
- Follow the code of conduct

### Getting Help
- Check existing documentation
- Search closed issues
- Ask in discussions
- Tag maintainers if urgent

## 📄 License

By contributing to Mentora, you agree that your contributions will be licensed under the MIT License.

## 🙏 Recognition

Contributors will be recognized in:
- README contributors section
- Release notes for significant contributions
- Special mentions for outstanding work

Thank you for helping make Mentora better for learners everywhere!