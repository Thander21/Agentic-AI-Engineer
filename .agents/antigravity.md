# Synkra AIOX Development Rules for AntiGravity

You are working with Synkra AIOX, an AI-Orchestrated System for Full Stack Development.

## Core Development Rules

### Agent Integration
- Recognize AIOX agent activations: @editorial, @dev, @qa, @architect, @pm, @po, @sm, @analyst
- Agent commands use * prefix: *help, *brief, *write, *review, *refine, *proof, *develop, *exit
- Follow agent-specific workflows and patterns

### Dual-Track Development (Code & Editorial)
1. **Always work from a story file** in docs/stories/ or the initiative task
2. **For Software Engineering:** @dev implements code, @qa executes test/quality gates
3. **For Editorial & Content:** @editorial (Scribe) researches, writes, applies 4-pillar quality gates, and refines
4. **Update story checkboxes** as tasks are completed: [ ] → [x]
5. **Maintain the File List** section with all created/modified files
6. **Follow acceptance criteria** exactly as written (ACs can be technical or editorial)

### Code Quality Standards
- Write clean, maintainable code following project conventions
- Include comprehensive error handling
- Add unit tests for all new functionality
- Follow existing patterns in the codebase

### Testing Protocol
- Run all tests before marking tasks complete
- Ensure linting passes: `npm run lint`
- Verify type checking: `npm run typecheck`
- Add tests for new features

## AIOX Framework Structure

```
aiox-core/
├── agents/       # Agent persona definitions
├── tasks/        # Executable task workflows
├── workflows/    # Multi-step workflows
├── templates/    # Document templates
└── checklists/   # Validation checklists

docs/
├── stories/      # Development stories
├── prd/          # Sharded PRD sections
└── architecture/ # Sharded architecture
```

## Development Workflow

1. **Read the story** - Understand requirements fully
2. **Implement sequentially** - Follow task order
3. **Test thoroughly** - Validate each step
4. **Update story** - Mark completed items
5. **Document changes** - Update File List

## Best Practices

### When implementing:
- Check existing patterns first
- Reuse components and utilities
- Follow naming conventions
- Keep functions focused and small

### When testing:
- Write tests alongside implementation
- Test edge cases
- Verify error handling
- Run full test suite

### When documenting:
- Update README for new features
- Document API changes
- Add inline comments for complex logic
- Keep story File List current

## Git & GitHub

- Use conventional commits: `feat:`, `fix:`, `docs:`, etc.
- Reference story ID in commits: `feat: implement IDE detection [Story 2.1]`
- Ensure GitHub CLI is configured: `gh auth status`
- Push regularly to avoid conflicts

## Common Patterns

### Error Handling
```javascript
try {
  // Operation
} catch (error) {
  console.error(`Error in ${operation}:`, error);
  throw new Error(`Failed to ${operation}: ${error.message}`);
}
```

### File Operations
```javascript
const fs = require('fs-extra');
const path = require('path');

// Always use absolute paths
const filePath = path.join(__dirname, 'relative/path');
```

### Async/Await
```javascript
async function operation() {
  try {
    const result = await asyncOperation();
    return result;
  } catch (error) {
    // Handle error appropriately
  }
}
```

---
*Synkra AIOX AntiGravity Configuration v1.0*
