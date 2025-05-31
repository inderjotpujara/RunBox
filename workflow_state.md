# AI Workflow State - RunBox Project

## State

- **Phase**: Initialize
- **Status**: READY
- **Current Task**: Project setup and configuration
- **Last Updated**: 2025-05-31

## Plan

### Project Initialization Checklist

- [x] Create project structure
- [x] Configure VS Code settings for AI development
- [x] Set up project configuration (LTM)
- [x] Initialize workflow state (STM)
- [ ] Configure package.json and dependencies
- [ ] Set up development environment
- [ ] Create initial component structure
- [ ] Configure build and deployment scripts
- [ ] Set up testing framework
- [ ] Implement CI/CD pipeline

## Rules

### Phase Entry Rules

- **Analyze**: Read and understand requirements, search for relevant information, log understanding without coding
- **Blueprint**: Create detailed implementation plan in checklist format, no code implementation
- **Construct**: Execute plan step-by-step, implement code, fix errors (max 3 retries per issue)
- **Validate**: Test implementation, run validation checks, proceed to next task or re-enter Construct if issues found

### Logging Rules

- Use concise, past-tense, one-line entries
- Format: "Action: Description of what was accomplished"
- Never modify existing log entries, only append new ones
- Include error resolutions and important decisions

### Coding Best Practices

- Follow conventions defined in project_config.md
- No placeholder code or TODOs in final implementations
- Format and lint all code before completion
- Add clear comments for AI integration logic
- Implement proper error handling for all async operations

### Tool Usage Rules

- Prefer VS Code tools over manual code writing
- Use search tools when facing unknown requirements
- Chain operations: edit → test → fix in single iterations
- Never ask user for guidance unless absolutely blocked (Status: BLOCKED)

### Quality Assurance

- Validate all changes with appropriate tests
- Ensure code follows TypeScript strict mode
- Check for security vulnerabilities
- Verify performance implications
- Confirm accessibility standards

## Log

- 2025-05-31 10:00: Initialized project structure and AI configuration
- 2025-05-31 10:15: Created VS Code settings with AI rules sync configuration
- 2025-05-31 10:20: Established project_config.md as long-term memory reference
- 2025-05-31 10:25: Set up workflow_state.md for autonomous AI development tracking

## Items

### Repetitive Tasks Queue

1. Component creation workflow
2. API endpoint implementation
3. Database schema updates
4. Test case generation
5. Documentation updates

## TokenizationResults

_This section will be used for log summarization when the log becomes too long_

---

### AI Instructions

**You are operating in autonomous mode. Follow this workflow:**

1. **Read** this workflow_state.md to understand current context
2. **Check** project_config.md for technical requirements and standards
3. **Execute** current task according to phase rules
4. **Update** this file with progress and next steps
5. **Continue** until task completion or BLOCKED status

**Current Priority**: Follow the Plan checklist sequentially. Update Status and Log after each major action. Never ask for user input unless Status = BLOCKED.

**Context Sources**:

- Long-term Memory: `project_config.md`
- Short-term Memory: `workflow_state.md` (this file)
- Technical Standards: `.vscode/settings.json`
