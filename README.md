# Freenet Agent Skills

AI coding agent skills for building applications on Freenet.

## Available Skills

### [dapp-builder](./dapp-builder/)

Build decentralized applications on Freenet. Guides through:
1. Designing contracts (shared, replicated state)
2. Implementing delegates (private, local state)
3. Building the UI (WebSocket connection to Freenet)

Based on [River](https://github.com/freenet/river), a decentralized chat application.

## Installation

### Claude Code

**Option 1: Clone and copy**
```bash
git clone https://github.com/freenet/freenet-agent-skills.git
cp -r freenet-agent-skills/dapp-builder ~/.claude/skills/
```

**Option 2: Clone and symlink** (easier to update)
```bash
git clone https://github.com/freenet/freenet-agent-skills.git ~/freenet-agent-skills
ln -s ~/freenet-agent-skills/dapp-builder ~/.claude/skills/
```

To update a symlinked skill:
```bash
cd ~/freenet-agent-skills && git pull
```

**Verify installation:**
Ask Claude: "What skills are available?" - it should list `freenet-dapp-builder`.

### Project-specific installation

To include a skill in a specific project (shared with team):
```bash
mkdir -p .claude/skills
cp -r freenet-agent-skills/dapp-builder .claude/skills/
git add .claude/skills
```

## Contributing

Skills follow the structure:

```
skill-name/
├── SKILL.md           # Main instructions (required)
└── references/        # Detailed documentation loaded on-demand
```

See [Claude Code documentation](https://docs.anthropic.com/en/docs/claude-code) for skill format details.

## License

LGPL-3.0
