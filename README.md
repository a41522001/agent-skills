# Agent Skills

A collection of [Agent Skills](https://agentskills.io) for AI coding agents such as Claude Code and Codex.

## Skills

| Skill | Description |
| --- | --- |
| [`nestjs-testing`](skills/nestjs-testing/SKILL.md) | Write, review, repair, and extend NestJS unit, integration-style, and HTTP E2E tests (Jest / Vitest, Supertest, Prisma, PostgreSQL, Redis). |
| [`figma-plugin-native-design`](skills/figma-plugin-native-design/SKILL.md) | Build a Figma Development Plugin that turns references, screenshots, SVGs, code, or specs into native, editable Figma design systems (variables, components, variants, Auto Layout). |

## Installation

### Claude Code (plugin marketplace)

```
/plugin marketplace add a41522001/agent-skills
/plugin install jeffery-skills@jeffery-skills
```

### Any agent (`skills` CLI)

```bash
npx skills add a41522001/agent-skills
```

### Manual

Copy the skill folder you want from `skills/` into your agent's skills directory, for example:

```bash
git clone https://github.com/a41522001/agent-skills.git
cp -R agent-skills/skills/nestjs-testing ~/.claude/skills/
```

## Structure

```
skills/
├── <skill-name>/
│   ├── SKILL.md          # Entry point: name, description, instructions
│   ├── references/       # Detailed docs loaded on demand
│   ├── scripts/          # Optional helper scripts
│   └── agents/           # Agent-specific metadata (e.g. openai.yaml)
```

## License

[MIT](LICENSE)
