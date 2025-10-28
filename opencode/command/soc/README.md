<SuperOpenCode>

# OpenCode Custom Commands (oc)

This directory contains OpenCode-optimized custom commands converted from Claude Code format.

## Overview

These commands provide enhanced workflows for development tasks including analysis, implementation, testing, documentation, and more. All commands have been adapted to work with OpenCode's command system and agent architecture.

## Available Commands

### Analysis & Planning
- `/oc:analyze [target]` - Comprehensive code analysis (quality, security, performance, architecture)
- `/oc:brainstorm <idea>` - Interactive requirements discovery through Socratic dialogue
- `/oc:estimate <feature>` - Development time/effort estimation with complexity analysis
- `/oc:explain <target>` - Clear explanations of code, concepts, and system behavior

### Implementation
- `/oc:implement <feature>` - Feature and code implementation with best practices
- `/oc:design <target>` - System architecture, API, and component design specifications
- `/oc:workflow <prd>` - Generate structured implementation workflows from PRDs

### Code Quality
- `/oc:improve [target]` - Systematic code quality, performance, and maintainability improvements
- `/oc:cleanup [target]` - Remove dead code and optimize project structure
- `/oc:troubleshoot <issue>` - Diagnose and resolve bugs, build failures, and system issues

### Testing & Building
- `/oc:test [target]` - Execute tests with coverage analysis and quality reporting
- `/oc:build [target]` - Build, compile, and package with error handling

### Documentation
- `/oc:document <target>` - Generate focused documentation for components, APIs, and features
- `/oc:index [target]` - Create comprehensive project documentation and knowledge base

### Git Operations
- `/oc:git <operation>` - Intelligent Git operations with smart commit messages

### Session Management
- `/oc:load` - Load project context and initialize development session
- `/oc:save` - Save session context and preserve discoveries
- `/oc:reflect` - Analyze task progress and validate work quality

### Advanced Orchestration
- `/oc:task <description>` - Execute complex tasks with workflow management
- `/oc:spawn <operation>` - Break down complex tasks into coordinated subtasks
- `/oc:select-tool <operation>` - Intelligent tool selection strategy analysis

## Usage

Commands can be invoked using the `/oc:` prefix followed by the command name:

```
/oc:analyze src/
/oc:implement user authentication
/oc:test --coverage
```

### Arguments

Most commands accept arguments using the `$ARGUMENTS` placeholder:

```
/oc:explain authentication.js
/oc:document src/api
/oc:troubleshoot "null pointer exception"
```

If no argument is provided, commands typically operate on the entire project or use sensible defaults.

## Agent Configuration

Some commands specify an `agent` in their frontmatter:

- `agent: build` - Uses the build agent for compilation and testing tasks
- `agent: plan` - Uses the planning agent for analysis and explanation tasks
- `subtask: true` - Forces execution as a subagent invocation

## Command Categories

Commands are organized by category based on their primary purpose:

- **utility** - Basic analysis, testing, and build operations
- **workflow** - Implementation and improvement workflows
- **orchestration** - Complex multi-step coordination (brainstorm, workflow)
- **special** - Advanced operations (task, index, estimate)
- **session** - Session management (load, save, reflect)

## Conversion Notes

These commands were converted from Claude Code format with the following changes:

1. **Removed**: `personas:` and `mcp-servers:` fields (Claude Code specific)
2. **Added**: `agent:` field where appropriate (OpenCode agents)
3. **Updated**: Command descriptions to use OpenCode terminology
4. **Enhanced**: Argument handling with `$ARGUMENTS` placeholder
5. **Simplified**: Removed Claude Code-specific behavioral instructions

## Differences from Claude Code

### Persona System
Claude Code uses explicit persona coordination (architect, frontend, backend, security, etc.). OpenCode handles domain expertise through its agent system and doesn't require explicit persona declarations.

### MCP Server Integration
Claude Code declares MCP servers (sequential, context7, magic, playwright, serena, morphllm) in command frontmatter. OpenCode manages MCP servers globally through configuration files.

### Agent Specification
OpenCode uses the `agent:` field to specify which agent should execute the command:
- `agent: build` - Build and testing operations
- `agent: plan` - Planning and analysis operations
- No agent specified - Uses current/default agent

## Examples

### Analyze code quality
```
/oc:analyze src/components
```

### Brainstorm a feature
```
/oc:brainstorm real-time collaboration system
```

### Implement a feature
```
/oc:implement user dashboard with analytics
```

### Run tests with coverage
```
/oc:test src/ --coverage
```

### Generate documentation
```
/oc:document src/api
```

### Troubleshoot an issue
```
/oc:troubleshoot "build fails with TypeScript errors"
```

## Tips

1. **Use specific targets**: Commands work better with specific targets than broad requests
2. **Provide context**: Include relevant context in your command arguments
3. **Combine with @ references**: Use `@filename` to reference specific files
4. **Use shell output**: Commands support `!`command`` syntax for dynamic input
5. **Chain commands**: Use multiple commands in sequence for complex workflows

## Contributing

To add or modify commands:

1. Edit the corresponding `.md` file in this directory
2. Follow the OpenCode command format with frontmatter
3. Use `$ARGUMENTS` for command parameters
4. Test the command in OpenCode
5. Update this README if adding new commands

## Related Documentation

- [OpenCode Commands Documentation](https://opencode.ai/docs/commands)
- [OpenCode Agents](https://opencode.ai/docs/agents)
- [OpenCode Configuration](https://opencode.ai/docs/config)

</SuperOpenCode>
