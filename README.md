# My Template

A project template for AI-assisted development with specialized agents for linting, documentation, and more.

## Overview

This template provides a structured setup for projects that leverage AI agents to automate code quality, documentation, and development tasks. It includes pre-configured agents for Go and Node.js linting, as well as a documentation agent.

## Features

- **Go Lint Agent** (`@go-lint`): Fixes Go code quality issues using `golangci-lint`, `gofmt`, and `goimports`.
- **Node Lint Agent** (`@node-lint`): Handles JavaScript/TypeScript linting with ESLint, Prettier, and TypeScript checks.
- **Docs Agent** (`@docs`): Creates and maintains project documentation, including READMEs, API docs, and code comments.
- **Extensible**: Add custom agents in `.github/agents/` and instructions in `.github/instructions/`.

## Quick Start

1. **Clone the template**:

   ```bash
   git clone https://github.com/your-repo/my-template.git
   cd my-template
   ```

2. **Customize agents**: Edit `.github/agents/` files to fit your project needs.

3. **Invoke agents**: In your development environment (e.g., VS Code with Copilot), use commands like:
   - `@go-lint` to fix Go code issues
   - `@node-lint` to lint Node.js code
   - `@docs` to generate or update documentation

## Project Structure

- `.github/agents/`: Agent configuration files (YAML frontmatter + Markdown body)
- `.github/instructions/`: Detailed instructions for each agent (e.g., commands, workflows)
- `README.md`: This file
- `my-template-x/`: Example sub-project (ignored for documentation purposes)

## Adding New Agents

1. Create a new `.md` file in `.github/agents/` with the required frontmatter (name, description, tools, etc.).
2. Add corresponding instructions in `.github/instructions/`.
3. Ensure the agent name is unique and follows conventions.

## Requirements

- VS Code or compatible IDE with AI agent support
- For Go agents: `golangci-lint`, `go`, etc.
- For Node agents: `npm`, ESLint, Prettier, TypeScript

## Contributing

Contributions are welcome! Please update documentation and test agents thoroughly.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
