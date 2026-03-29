# BrandForge

AI prompt framework for comprehensive brand strategy development. BrandForge transforms an AI assistant into a full-service brand strategy team with 12 specialized personas, structured workflows, and synthetic user research.

## What This Is

BrandForge is not a software application — it's a structured collection of markdown prompts designed for use with AI coding assistants (Claude Code). When loaded as a plugin, it provides slash commands, expert personas, and orchestrated workflows for end-to-end brand development.

## Features

- **12 specialized personas** — architect, strategist, creative director, UX researcher, market analyst, content strategist, business designer, cultural strategist, QA, launch manager, analyzer, and mentor
- **16 slash commands** — `/brandforge init`, `/brandforge forge`, `/brandforge strategy`, `/brandforge creative`, and more
- **Intelligent orchestration** — automatic persona routing based on task complexity scoring
- **Synthetic user research** — generate realistic personas for design thinking interviews without recruiting real participants
- **Flag system** — precision targeting for demographic, research depth, creative scope, and quality control

## Usage

```bash
# Initialize a brand project
/brandforge init "MyBrand" --type startup --industry fintech

# Run research
/brandforge research --user-personas --market-analysis

# Develop strategy
/brandforge strategy competitive --scope industry

# Create visual identity
/brandforge creative design-system --scope comprehensive

# Validate with synthetic users
/brandforge validate concept --method synthetic

# Or run the full workflow
/brandforge forge --complete-workflow
```

## Structure

```
├── BRANDFORGE.md              # Entry point
├── PERSONAS.md                # 12 expert personas
├── COMMANDS.md                # Command reference
├── ORCHESTRATOR.md            # Intelligent task routing
├── DYNAMIC_PERSONA_SYSTEM.md  # Synthetic user research
├── PRINCIPLES.md              # Core philosophy and ethics
├── FLAGS.md                   # Precision targeting flags
├── MODES.md                   # Operational modes
├── RULES.md                   # Safety protocols
└── commands/bf/               # Individual command definitions
```

## License

Licensed under either of [Apache License, Version 2.0](LICENSE-APACHE) or [MIT License](LICENSE-MIT) at your option.
