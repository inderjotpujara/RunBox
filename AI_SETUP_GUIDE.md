# VS Code AI Rules Setup Guide for RunBox

## Overview

This guide configures VS Code for autonomous AI-powered development with settings sync across your account and devices.

## What's Been Configured

### 📁 Project Structure

```
RunBox/
├── .vscode/
│   ├── settings.json          # Main VS Code configuration
│   ├── tasks.json            # Automated tasks for AI development
│   ├── launch.json           # AI-enhanced debugging profiles
│   └── extensions.json       # Recommended extensions
├── .cursorrules              # AI rules compatible with multiple tools
├── project_config.md         # Long-term memory (LTM) - Project standards
├── workflow_state.md         # Short-term memory (STM) - Current context
└── RunBox.code-workspace     # Workspace configuration
```

### 🤖 AI-Powered Features Enabled

#### GitHub Copilot Integration

- ✅ Context-aware code suggestions
- ✅ Inline completions for faster development
- ✅ Chat integration for planning and debugging
- ✅ Language-specific optimization

#### AI Rules Sync

- ✅ Automatic synchronization between Cursor, VS Code, and other AI tools
- ✅ Base rule file: `.cursorrules`
- ✅ Auto-sync on file changes
- ✅ Consistent AI behavior across tools

#### Autonomous Development Workflow

- ✅ Two-file memory system (LTM/STM)
- ✅ Four-phase development cycle: Analyze → Blueprint → Construct → Validate
- ✅ Automated code formatting and linting
- ✅ Context preservation across sessions

## 🔄 Enable Settings Sync

### Step 1: Turn On Settings Sync

1. Open VS Code
2. Press `Cmd+Shift+P` (macOS) or `Ctrl+Shift+P` (Windows/Linux)
3. Type "Settings Sync: Turn On"
4. Select "Settings Sync: Turn On..."
5. Choose what to sync:
   - ✅ Settings
   - ✅ Extensions
   - ✅ UI State
   - ✅ Snippets
   - ✅ Profiles

### Step 2: Sign In

1. Choose your preferred account:
   - **Microsoft Account** (recommended for GitHub Copilot users)
   - **GitHub Account**
2. Authorize VS Code to access your account
3. Your settings will now sync across all devices

### Step 3: Verify Configuration

1. Check that the AI Rules Sync extension is installed
2. Open Command Palette: `Cmd+Shift+P`
3. Run "AI Rules Sync: Sync Rules"
4. Verify sync status in the sidebar

## 🛠 Manual Setup (if needed)

### Install Required Extensions

```bash
# Core AI extensions
code --install-extension github.copilot
code --install-extension github.copilot-chat
code --install-extension zidonglin.ai-rules-sync

# Development essentials
code --install-extension esbenp.prettier-vscode
code --install-extension ms-vscode.vscode-eslint
code --install-extension ms-typescript.typescript
```

### Configure AI Rules Sync

1. Open VS Code settings: `Cmd+,`
2. Search for "AI Rules Sync"
3. Configure these settings:
   - **Base Rule File**: `${workspaceFolder}/.cursorrules`
   - **Auto Sync**: `true`
   - **Watch for Changes**: `true`

## 🚀 How to Use

### For Autonomous AI Development

1. **Open the workspace**: `File → Open Workspace from File → RunBox.code-workspace`
2. **Start a new task**: Edit `workflow_state.md` → Update the Plan section
3. **Let AI work**: The AI will follow the autonomous workflow rules
4. **Monitor progress**: Check `workflow_state.md` for updates

### For Regular Development

1. **Use GitHub Copilot**: Start typing and accept suggestions with `Tab`
2. **Chat with AI**: Open Copilot Chat with `Cmd+Shift+I`
3. **Format code**: Save files for auto-formatting
4. **Run tasks**: `Cmd+Shift+P` → "Tasks: Run Task"

## 📋 Available Commands

### AI Rules Sync

- `AI Rules Sync: Sync Rules` - Manual sync of AI rules
- `AI Rules Sync: Select Base Rule File` - Change base rule file
- `AI Rules Sync: Toggle Auto Sync` - Enable/disable auto-sync

### Development Tasks

- `AI: Initialize Project` - Set up development environment
- `AI: Format Code` - Format all code files
- `AI: Lint Code` - Run linting with auto-fix
- `AI: Full Quality Check` - Comprehensive code quality check

### GitHub Copilot

- `GitHub Copilot: Toggle` - Enable/disable Copilot
- `GitHub Copilot: Open Chat` - Start AI chat session
- `GitHub Copilot: Generate Tests` - Auto-generate test cases

## 🔧 Troubleshooting

### Settings Sync Issues

1. **Check internet connection**
2. **Sign out and sign back in**: `Cmd+Shift+P` → "Settings Sync: Reset"
3. **Force sync**: `Cmd+Shift+P` → "Settings Sync: Sync Now"

### AI Rules Sync Issues

1. **Check file permissions** on `.cursorrules`
2. **Verify extension is active**: Extensions panel → AI Rules Sync
3. **Manual sync**: Command Palette → "AI Rules Sync: Sync Rules"

### GitHub Copilot Issues

1. **Check subscription**: Settings → GitHub Copilot
2. **Restart VS Code** if suggestions stop working
3. **Clear cache**: `Cmd+Shift+P` → "Developer: Clear Cache and Reload"

## 📖 AI Development Workflow

### The Four Phases

1. **Analyze** 📊

   - Read requirements and existing code
   - Search for relevant information
   - Log understanding without coding

2. **Blueprint** 📋

   - Create detailed implementation plan
   - Break down into checklist items
   - Identify dependencies and integration points

3. **Construct** 🔨

   - Execute plan step-by-step
   - Implement complete, tested code
   - No placeholders or TODOs

4. **Validate** ✅
   - Run tests and quality checks
   - Verify against requirements
   - Fix issues or move to next task

### Memory System

- **Long-term Memory**: `project_config.md` - Standards and architecture
- **Short-term Memory**: `workflow_state.md` - Current context and progress

## 🌟 Pro Tips

1. **Use the workspace file**: Always open `RunBox.code-workspace` for full configuration
2. **Trust the AI workflow**: Let the autonomous system handle routine tasks
3. **Monitor the workflow log**: Check `workflow_state.md` for AI decision history
4. **Customize per project**: Modify `.cursorrules` for project-specific needs
5. **Keep rules updated**: Sync improves as you refine your AI rules

## 📚 Additional Resources

- [VS Code Settings Sync Documentation](https://code.visualstudio.com/docs/editor/settings-sync)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [AI Rules Sync Extension](https://marketplace.visualstudio.com/items?itemName=zidonglin.ai-rules-sync)

---

**Ready to start!** 🎉 Your VS Code is now configured for autonomous AI development with settings sync enabled across all your devices.
