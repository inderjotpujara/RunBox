# RunBox AI Development Configuration

## Tech Stack

- **Frontend**: React Native (Expo), TypeScript
- **Backend**: Node.js/Express, TypeScript
- **Database**: Firebase (Auth + Firestore), PostgreSQL (Prisma)
- **AI Integration**: OpenAI GPT-4, Anthropic Claude
- **Development**: VS Code, GitHub Copilot, AI Rules Sync

## Architecture Principles

- **Client/Server Separation**: Clear boundaries between frontend and backend
- **MVC Pattern** (Server): Models, Views, Controllers for API structure
- **MVVM Pattern** (Client): Model-View-ViewModel for React Native components
- **Component-Based Design**: Modular, reusable components
- **Type Safety**: Strict TypeScript configuration

## Coding Standards

### Naming Conventions

- **Variables & Functions**: camelCase (`getUserData`, `isAuthenticated`)
- **Components**: PascalCase (`LoginScreen`, `UserProfile`)
- **Constants**: SCREAMING_SNAKE_CASE (`API_BASE_URL`, `MAX_RETRY_COUNT`)
- **Files**: kebab-case for utilities, PascalCase for components
- **Database**: snake_case for tables and columns

### Code Structure

```
src/
├── components/          # Reusable UI components
├── screens/            # Screen components
├── navigation/         # Navigation configuration
├── services/           # API and business logic
├── utils/              # Helper functions
├── types/              # TypeScript type definitions
├── hooks/              # Custom React hooks
└── constants/          # App constants
```

### Frontend Rules

- Use functional components with React Hooks only
- Separate UI, logic, and styles into different files/sections
- Implement proper error boundaries
- Use TypeScript interfaces for all data structures
- No `any` types - use proper typing
- Implement proper loading and error states

### Backend Rules

- Use async/await exclusively, no callbacks
- Implement comprehensive error handling
- Use feature-based folder structure
- Secure coding: no secrets in code, input validation mandatory
- RESTful API design with consistent response formats
- Proper logging and monitoring

### Database Rules

- Use Prisma schema for PostgreSQL operations
- Implement proper migrations
- Use Firebase for real-time features and authentication
- Normalize data structure
- Implement proper indexing

## AI Integration Guidelines

### MCP Tool Usage

- **Search**: Use web search for latest documentation and best practices
- **Code Generation**: Leverage AI for boilerplate and repetitive code
- **Code Review**: AI-assisted code quality checks
- **Documentation**: Auto-generate inline comments and README updates

### AI Workflow Rules

- Always validate AI-generated code before implementation
- Use AI for planning and architecture suggestions
- Implement AI-suggested optimizations after testing
- Document AI-assisted decisions in commit messages

## Development Workflow

### Code Quality

- Format code automatically on save
- Run linters and fix issues before commits
- Write unit tests for critical functions
- Use meaningful commit messages
- No console.log statements in production code

### Error Handling

- Implement try-catch blocks for all async operations
- Use proper error types and messages
- Log errors with context information
- Provide user-friendly error messages

### Performance

- Optimize bundle size and loading times
- Implement proper caching strategies
- Use lazy loading for components and routes
- Monitor and optimize database queries

## Security Guidelines

- Never commit API keys or secrets
- Use environment variables for configuration
- Implement proper authentication and authorization
- Validate all user inputs
- Use HTTPS for all communications
- Regular security audits and dependency updates

## Testing Strategy

- Unit tests for utilities and services
- Integration tests for API endpoints
- E2E tests for critical user flows
- Manual testing on multiple devices
- Performance testing for optimization

## Documentation Requirements

- README files for each major feature
- Inline code comments for complex logic
- API documentation with examples
- Architecture decision records (ADRs)
- Deployment and setup instructions

## Deployment

- Use environment-specific configurations
- Implement CI/CD pipelines
- Monitor application performance
- Automated testing before deployment
- Rollback strategies for production issues

---

_This configuration serves as the long-term memory (LTM) for AI-assisted development in the RunBox project._
