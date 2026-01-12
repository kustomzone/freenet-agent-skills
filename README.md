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

Copy the skill directory to your Claude skills folder:

```bash
cp -r dapp-builder ~/.claude/skills/
```

Or symlink it:

```bash
ln -s /path/to/freenet-agent-skills/dapp-builder ~/.claude/skills/
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
