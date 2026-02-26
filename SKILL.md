---
name: explain-code
description: Explains code with visual diagrams and analogies. Use when explaining how code works, teaching about a codebase, or when the user asks "how does this work?", "explain this code", "what does this code do", "walk me through this", "explain this file", "explain this function", "explain this class", "break down this code", or wants to understand code logic, architecture, or behavior. Includes Spring Boot equivalent mappings for non-Java code.
allowed-tools: Bash(*), Glob(*), Grep(*), Read(*)
argument-hint: "[file, function, class, or directory to explain]"
---

# Code Explanation Skill

When explaining code, always include these four elements:

1. **Start with an analogy**: Compare the code to something from everyday life to build intuition before diving into details.
2. **Draw a diagram**: Use ASCII art or Mermaid diagrams to show the flow, structure, or relationships between components. Prefer Mermaid for complex flows and class relationships; use ASCII art for simple, quick illustrations.
3. **Walk through the code**: Explain step-by-step what happens.
4. **Highlight a gotcha**: Call out a common mistake or misconception related to the code.

For complex concepts, use multiple analogies.

## Output Templates

Structure explanations using these sections as appropriate:

- **File/Class:** Purpose, Key Concepts, Structure, How It Works, Dependencies & Interactions, Notable Details
- **Function/Method:** Purpose, Parameters & Return Value, How It Works, Edge Cases & Error Handling, Usage
- **Directory/Module:** Purpose, Architecture, Key Files, External Interfaces, Data Flow

## Spring Boot Equivalents

When the code is not Java/Kotlin + Spring Boot, read `references/spring-boot-mapping.md` and include equivalent mappings in the explanation.

## Explanation Guidelines

- **Reference specific line numbers** using `file_path:line_number` format.
- **Call out design patterns** by name (e.g., "This uses the Strategy pattern to...").
