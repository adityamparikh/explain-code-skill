# Explain Code Skill

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill that explains code using visual diagrams, analogies, and structured walkthroughs.

## What It Does

- Explains files, functions, classes, or entire directories
- Starts with an everyday analogy to build intuition
- Draws ASCII art or Mermaid diagrams to visualize flow and structure
- Walks through the code step-by-step with line number references
- Highlights common gotchas and misconceptions
- Maps non-Java code to Spring Boot equivalents for Java developers
- Verifies library/framework behavior against live documentation

## Usage

Install as a Claude Code skill, then:

```
Explain this file
```

```
How does the authentication middleware work?
```

```
Walk me through src/services/payment.ts
```

## Installation

Add this skill to your Claude Code configuration:

```bash
claude mcp add-skill explain-code https://github.com/adityamparikh/explain-code-skill
```

Or clone into your skills directory:

```bash
git clone https://github.com/adityamparikh/explain-code-skill.git ~/.claude/skills/explain-code
```

## License

MIT
