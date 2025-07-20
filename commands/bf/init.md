# /brandforge init - Project Initialization & Discovery

## Command Structure
```yaml
---
command: "/brandforge init"
category: "Brand Strategy Foundation"
purpose: "Comprehensive brand project initialization and discovery"
wave-enabled: true
performance-profile: "standard"
---
```

## Purpose
Complete brand project initialization that establishes foundation, discovers context, and creates strategic roadmap. Combines market analysis, competitive intelligence, and brand positioning discovery.

## Usage Patterns
```bash
/brandforge init [project-name] [flags]
/brandforge init [brand-concept] --market [industry] --audience [target]
/brandforge init --discovery --analysis --strategy
```

## Arguments
- **project-name**: Brand project identifier (optional)
- **brand-concept**: Core brand idea or hypothesis (optional)

## Flags
- `--market [industry]`: Specify target industry/market
- `--audience [persona]`: Define primary target audience
- `--discovery`: Enable comprehensive discovery phase
- `--analysis`: Activate market and competitive analysis
- `--strategy`: Generate initial strategic framework
- `--mvp`: Focus on minimum viable brand
- `--enterprise`: Scale for enterprise requirements
- `--validate`: Include validation checkpoints
- `--uc`: Ultra-compressed output mode

## Auto-Persona Activation
- **architect**: System-wide brand architecture planning
- **analyst**: Market and competitive intelligence
- **mentor**: Strategic guidance and education
- **scribe**: Documentation and brand guidelines

## MCP Server Integration
- **Context7**: Brand strategy patterns and frameworks
- **Sequential**: Multi-step discovery and planning
- **Magic**: Visual brand elements and mood boards

## Workflow Process
1. **Discovery Phase**: Market research, competitive analysis, audience profiling
2. **Foundation Setting**: Brand architecture, positioning framework
3. **Strategic Planning**: Roadmap development, milestone definition
4. **Documentation**: Brand guidelines, asset inventory
5. **Validation**: Checkpoint reviews and quality gates

## Quality Gates
- ✅ Market analysis completeness
- ✅ Competitive differentiation identified
- ✅ Target audience clearly defined
- ✅ Strategic positioning validated
- ✅ Documentation standards met

## Examples
```bash
# Basic project initialization
/brandforge init "EcoTech Solutions"

# Comprehensive brand discovery
/brandforge init --discovery --analysis --strategy

# Targeted market entry
/brandforge init "Sustainable Fashion" --market fashion --audience millennials

# Enterprise-scale brand development
/brandforge init --enterprise --validate --uc
```

## Output Structure
```
brand-forge/
├── discovery/
│   ├── market-analysis.md
│   ├── competitive-landscape.md
│   └── audience-personas.md
├── strategy/
│   ├── positioning-framework.md
│   ├── brand-architecture.md
│   └── strategic-roadmap.md
└── guidelines/
    ├── brand-guidelines.md
    └── asset-inventory.md
```