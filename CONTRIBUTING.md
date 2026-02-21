# Contributing to Electrobun Skills

Thank you for your interest in contributing to Electrobun Skills! This guide will help you create high-quality skills following best practices.

## Skill Creation Guidelines

### Follow Anthropic's Skill-Creator Guidelines

All skills must follow the patterns outlined in [Anthropic's skill-creator](https://skills.sh/anthropics/skills/skill-creator):

1. **Concise SKILL.md** - Keep the main skill file under 500 lines
2. **Comprehensive descriptions** - Write detailed frontmatter descriptions (200-300 words) for proper triggering
3. **Progressive disclosure** - Move detailed content to `references/` folder
4. **Real-world examples** - Include practical, tested code examples
5. **Reusable scripts** - Add helper scripts to `scripts/` folder when appropriate

### Skill Structure

```
skill-name/
├── SKILL.md              # Main skill file (required)
├── references/           # Detailed documentation (optional)
│   ├── api-reference.md
│   └── advanced-patterns.md
├── scripts/              # Reusable code (optional)
│   └── helper.ts
└── assets/               # Output resources (optional)
    └── template.html
```

### SKILL.md Format

```markdown
---
name: skill-name
description: Comprehensive description that helps AI agents know when to trigger this skill. Include what the skill does, when to use it, and common trigger phrases. 200-300 words recommended.
license: MIT
metadata:
  author: Your Name
  version: "1.0.0"
---

# Skill Name

Brief introduction (2-3 sentences).

## Core Concepts

Essential patterns and workflows.

## Code Examples

Real-world, tested code examples.

## Resources

Links to related skills and documentation.
```

### Description Best Practices

The frontmatter `description` is critical for skill triggering. Include:

- **What the skill does**: Clear statement of capabilities
- **When to use it**: Specific scenarios and use cases
- **Trigger phrases**: Common words/phrases users might say
- **Scope**: What's covered and what's not

Example:
```yaml
description: Build and configure Docker containers for development and production. Covers Dockerfile creation, multi-stage builds, docker-compose orchestration, volume management, networking, and optimization. Use when containerizing applications, setting up development environments, deploying with Docker, troubleshooting container issues, or implementing CI/CD with Docker. Triggers include "Docker", "container", "Dockerfile", "docker-compose", "containerize", "image build", or discussions about container-based deployment.
```

## Submission Process

### 1. Create Your Skill

```bash
# Create skill directory
mkdir -p skills/your-skill-name

# Create SKILL.md
# Follow the structure above
```

### 2. Test Your Skill

- Test the skill with GitHub Copilot CLI or Claude
- Verify it triggers appropriately
- Ensure code examples work correctly
- Check for typos and formatting

### 3. Submit Pull Request

1. Fork the repository
2. Create a feature branch: `git checkout -b add-skill-name`
3. Add your skill
4. Commit: `git commit -m "Add [skill-name] skill"`
5. Push: `git push origin add-skill-name`
6. Open a Pull Request

### PR Checklist

- [ ] SKILL.md follows the required format
- [ ] Frontmatter description is comprehensive (200-300 words)
- [ ] SKILL.md body is concise (<500 lines)
- [ ] Code examples are tested and working
- [ ] No typos or formatting issues
- [ ] Skill is focused and has clear scope
- [ ] Related skills are cross-referenced

## Quality Standards

### Code Examples

- **Complete**: Examples should be copy-paste ready
- **Tested**: Verify all code actually works
- **Commented**: Add comments for complex logic
- **Realistic**: Use real-world scenarios

### Writing Style

- **Clear**: Use simple, direct language
- **Concise**: Remove unnecessary words
- **Active voice**: "Use X to do Y" not "X can be used to do Y"
- **Imperative form**: "Create a window" not "Creating a window"

### Progressive Disclosure

If your SKILL.md is approaching 500 lines:

1. Move detailed API docs to `references/api.md`
2. Move advanced patterns to `references/advanced.md`
3. Move troubleshooting to `references/troubleshooting.md`
4. Keep only essential workflows in SKILL.md

Reference files from SKILL.md:
```markdown
For complete API reference, see [API Documentation](references/api.md).
For advanced patterns, see [Advanced Patterns](references/advanced.md).
```

## Examples

Study existing skills for inspiration:

- **electrobun** - Core skill structure
- **electrobun-window-management** - Multi-window patterns
- **electrobun-rpc-patterns** - Advanced communication
- **electrobun-native-ui** - Native integration
- **electrobun-distribution** - Build and deploy
- **electrobun-debugging** - Troubleshooting

## Questions?

- Open an issue for discussion
- Join [Electrobun Discord](https://discord.gg/ueKE4tjaCE)
- Review [Anthropic's skill-creator guide](https://skills.sh/anthropics/skills/skill-creator)

## License

All skills must be MIT licensed to maintain compatibility with the repository.
