# COMMANDS.md - BrandForge Command Execution Framework

Command execution framework for BrandForge brand strategy ecosystem.

## Command System Architecture

### Core Command Structure
```yaml
---
command: "/brandforge-{command-name}"
category: "Brand Development Classification"
purpose: "Brand Strategy Objective"
wave-enabled: true|false
performance-profile: "optimization|standard|complex"
---
```

### Command Processing Pipeline
1. **Input Parsing**: `$ARGUMENTS` with `@<path>`, `!<command>`, `--<flags>`
2. **Context Resolution**: Auto-persona activation and MCP server selection
3. **Wave Eligibility**: Complexity assessment and wave mode determination
4. **Execution Strategy**: Tool orchestration and resource allocation
5. **Quality Gates**: Validation checkpoints and error handling

### Integration Layers
- **BrandForge Commands**: Native slash command compatibility
- **Persona System**: Auto-activation based on command context
- **MCP Servers**: Market research, creative tools, synthetic user integration
- **Wave System**: Multi-stage orchestration for complex brand projects

## Core Commands

### `/brandforge init [project-name] [flags]`
```yaml
---
command: "/brandforge init"
category: "Project Setup"
purpose: "Initialize brand development project"
wave-enabled: false
performance-profile: "standard"
---
```
- **Auto-Persona**: Architect, Project Manager
- **MCP Integration**: Context7 for industry patterns, Sequential for project planning
- **Arguments**: `[project-name]`, `--type [startup|enterprise|rebrand|product]`
- **Flags**: `--industry <sector>`, `--budget <range>`, `--timeline <duration>`

### `/brandforge forge [target] [flags]`
```yaml
---
command: "/brandforge forge"
category: "Complete Brand Development"
purpose: "Orchestrate end-to-end brand development"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: Architect, Strategist, Creative Director, Researcher
- **MCP Integration**: All servers for comprehensive orchestration
- **Arguments**: `[target]`, `@<path>`, `!<command>`
- **Flags**: `--complete-workflow`, `--from-strategy-to-launch`, `--phase [discovery|strategy|creative|validation|launch]`

### `/brandforge strategy [operation] [scope]`
```yaml
---
command: "/brandforge strategy"
category: "Strategic Planning"
purpose: "Brand strategy and market positioning"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: Brand Strategist, Business Designer, Analyst
- **MCP Integration**: Context7 for market data, Sequential for strategic analysis
- **Operations:**
  - `position`: Brand positioning and differentiation
  - `competitive`: Competitive analysis and market mapping
  - `architecture`: Brand architecture and hierarchy
  - `innovation`: Business model innovation
  - `growth`: Growth strategy and market expansion
- **Scopes:**
  - `market`: Industry-wide analysis
  - `segment`: Target market segment
  - `product`: Product-level positioning
  - `enterprise`: Corporate brand strategy

### `/brandforge creative [operation] [medium]`
```yaml
---
command: "/brandforge creative"
category: "Creative Development"
purpose: "Visual identity and creative concept development"
wave-enabled: true
performance-profile: "optimization"
---
```
- **Auto-Persona**: Creative Director, Visual Designer, Content Strategist
- **MCP Integration**: Magic for design generation, Context7 for design patterns
- **Operations:**
  - `concept`: Creative concept development
  - `identity`: Visual identity and brand systems
  - `design`: Design system creation
  - `campaign`: Creative campaign development
  - `guidelines`: Brand guidelines documentation
- **Mediums:**
  - `digital`: Digital experiences and interfaces
  - `print`: Print and physical materials
  - `identity`: Brand identity systems
  - `campaign`: Marketing campaigns
  - `experience`: Brand experiences

### `/brandforge research [type] [methodology]`
```yaml
---
command: "/brandforge research"
category: "User & Market Research"
purpose: "Comprehensive research and validation"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: UX Researcher, Market Analyst, Ethnographer
- **MCP Integration**: Sequential for research methodology, Playwright for user testing
- **Types:**
  - `synthetic`: Synthetic user research and persona generation
  - `traditional`: Real user research coordination
  - `market`: Market analysis and competitive intelligence
  - `ethnographic`: Deep user behavior research
  - `validation`: Concept and assumption validation
- **Methodologies:**
  - `interviews`: One-on-one user interviews
  - `focus-groups`: Moderated group discussions
  - `surveys`: Quantitative user research
  - `usability`: Usability testing and validation
  - `journey-mapping`: Customer journey analysis

### `/brandforge market [operation] [scope]`
```yaml
---
command: "/brandforge market"
category: "Market Intelligence"
purpose: "Market analysis and competitive intelligence"
wave-enabled: true
performance-profile: "standard"
---
```
- **Auto-Persona**: Market Analyst, Strategist, Business Designer
- **MCP Integration**: Context7 for market data, Sequential for analysis
- **Operations:**
  - `analysis`: Comprehensive market analysis
  - `competitive`: Competitor analysis and positioning
  - `trends`: Market trend identification
  - `opportunity`: Market opportunity assessment
  - `segmentation`: Market segmentation
- **Scopes:**
  - `industry`: Industry-wide analysis
  - `regional`: Geographic market analysis
  - `demographic`: Target demographic analysis
  - `competitive`: Competitive landscape

### `/brandforge content [operation] [channel]`
```yaml
---
command: "/brandforge content"
category: "Content Strategy"
purpose: "Brand voice and content development"
wave-enabled: true
performance-profile: "standard"
---
```
- **Auto-Persona**: Content Strategist, Brand Voice Specialist, Copywriter
- **MCP Integration**: Context7 for content patterns, Scribe for content creation
- **Operations:**
  - `strategy`: Content strategy development
  - `voice`: Brand voice and tone definition
  - `messaging`: Core messaging framework
  - `storytelling`: Brand narrative development
  - `calendar`: Editorial calendar creation
- **Channels:**
  - `digital`: Digital content and web
  - `social`: Social media content
  - `marketing`: Marketing communications
  - `internal`: Internal brand communications

### `/brandforge business [operation] [model-type]`
```yaml
---
command: "/brandforge business"
category: "Business Design"
purpose: "Business model and value proposition design"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: Business Designer, Strategist, Innovation Specialist
- **MCP Integration**: Sequential for business modeling, Context7 for patterns
- **Operations:**
  - `model`: Business model design
  - `value-prop`: Value proposition development
  - `pricing`: Pricing strategy
  - `go-to-market`: Go-to-market strategy
  - `scaling`: Growth and scaling strategy
- **Model Types:**
  - `startup`: New venture business models
  - `enterprise`: Corporate business models
  - `subscription`: Subscription-based models
  - `marketplace`: Platform and marketplace models
  - `saas`: Software-as-a-service models

### `/brandforge validate [target] [method]`
```yaml
---
command: "/brandforge validate"
category: "Validation & Testing"
purpose: "Validate brand concepts and assumptions"
wave-enabled: true
performance-profile: "standard"
---
```
- **Auto-Persona**: QA Specialist, Researcher, Analyst
- **MCP Integration**: All servers for comprehensive validation
- **Targets:**
  - `concept`: Brand concept validation
  - `positioning`: Positioning validation
  - `messaging`: Message testing
  - `creative`: Creative concept testing
  - `business-model`: Business model validation
- **Methods:**
  - `synthetic`: Synthetic user validation
  - `traditional`: Real user testing
  - `market`: Market validation
  - `stakeholder`: Stakeholder feedback
  - `data`: Data-driven validation

### `/brandforge launch [phase] [strategy]`
```yaml
---
command: "/brandforge launch"
category: "Launch & Deployment"
purpose: "Brand rollout and launch orchestration"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: Project Manager, Launch Specialist, DevOps
- **MCP Integration**: Sequential for planning, Context7 for best practices
- **Phases:**
  - `pre-launch`: Launch preparation and testing
  - `soft-launch`: Controlled rollout
  - `full-launch`: Complete market launch
  - `scale`: Growth and expansion
- **Strategies:**
  - `digital-first`: Digital-first launch
  - `omnichannel`: Multi-channel rollout
  - `phased`: Staged deployment
  - `surprise`: Surprise and delight launch

## Development Commands

### `/brandforge build [target] [framework]`
```yaml
---
command: "/brandforge build"
category: "Development & Deployment"
purpose: "Build brand assets and deliverables"
wave-enabled: true
performance-profile: "optimization"
---
```
- **Auto-Persona**: Developer, Designer, Asset Manager
- **MCP Integration**: Magic for asset generation, Sequential for build process
- **Targets:**
  - `assets`: Brand asset creation
  - `website`: Brand website development
  - `guidelines`: Brand guidelines compilation
  - `templates`: Brand template creation
- **Frameworks:**
  - `design-system`: Comprehensive design system
  - `style-guide`: Brand style guide
  - `component-library`: Reusable brand components
  - `documentation`: Complete brand documentation

### `/brandforge improve [target] [focus]`
```yaml
---
command: "/brandforge improve"
category: "Quality & Enhancement"
purpose: "Evidence-based brand enhancement"
wave-enabled: true
performance-profile: "optimization"
---
```
- **Auto-Persona**: Refactorer, Performance Specialist, QA
- **MCP Integration**: Sequential for analysis, Context7 for improvement patterns
- **Targets:**
  - `strategy`: Strategic refinement
  - `creative`: Creative enhancement
  - `positioning`: Positioning optimization
  - `performance`: Brand performance improvement
- **Focus Areas:**
  - `market-fit`: Market fit optimization
  - `user-experience`: User experience enhancement
  - `competitive`: Competitive positioning
  - `growth`: Growth optimization

### `/brandforge analyze [target] [dimension]`
```yaml
---
command: "/brandforge analyze"
category: "Analysis & Investigation"
purpose: "Multi-dimensional brand analysis"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: Analyzer, Strategist, Researcher
- **MCP Integration**: Sequential for deep analysis, Context7 for benchmarks
- **Targets:**
  - `brand-health`: Overall brand health assessment
  - `competitive`: Competitive landscape analysis
  - `user-perception`: User perception and sentiment
  - `market-position`: Market position analysis
- **Dimensions:**
  - `performance`: Brand performance metrics
  - `sentiment`: Brand sentiment analysis
  - `awareness`: Brand awareness measurement
  - `loyalty`: Customer loyalty assessment

## Meta Commands

### `/brandforge index [query] [flags]`
```yaml
---
command: "/brandforge index"
category: "Navigation & Discovery"
purpose: "Command catalog browsing and discovery"
wave-enabled: false
performance-profile: "standard"
---
```
- **Auto-Persona**: Mentor, Navigator
- **Purpose**: Help users discover and understand BrandForge capabilities

### `/brandforge task [operation] [scope]`
```yaml
---
command: "/brandforge task"
category: "Project Management"
purpose: "Long-term brand project management"
wave-enabled: true
performance-profile: "complex"
---
```
- **Auto-Persona**: Project Manager, Architect
- **Purpose**: Manage complex multi-phase brand projects

## Command Categories

### Development Commands
- **Tier 1**: `/brandforge forge`, `/brandforge build`, `/brandforge improve`
- **Tier 2**: `/brandforge strategy`, `/brandforge creative`, `/brandforge validate`

### Research Commands
- **Tier 1**: `/brandforge research`, `/brandforge market`, `/brandforge analyze`
- **Tier 2**: `/brandforge validate`, `/brandforge launch`

### Planning Commands
- **Tier 1**: `/brandforge strategy`, `/brandforge task`, `/brandforge business`

### Quality Commands
- **Tier 1**: `/brandforge improve`, `/brandforge validate`, `/brandforge analyze`

### Meta Commands
- **Navigation**: `/brandforge index`, `/brandforge task`

## Command Integration Matrix

| Command | Primary Persona | Secondary Persona | MCP Servers | Complexity |
|---------|-----------------|-------------------|-------------|------------|
| init | Architect | Project Manager | Context7, Sequential | Low |
| forge | Architect | All Personas | All Servers | High |
| strategy | Strategist | Business Designer | Context7, Sequential | High |
| creative | Creative Director | Visual Designer | Magic, Context7 | Medium |
| research | UX Researcher | Market Analyst | Sequential, Playwright | High |
| market | Market Analyst | Strategist | Context7, Sequential | Medium |
| content | Content Strategist | Copywriter | Context7, Scribe | Medium |
| business | Business Designer | Strategist | Sequential, Context7 | High |
| validate | QA Specialist | Researcher | All Servers | Medium |
| launch | Project Manager | Launch Specialist | Sequential, Context7 | High |
| build | Developer | Designer | Magic, Sequential | Medium |
| improve | Refactorer | Performance Specialist | Sequential, Context7 | Medium |
| analyze | Analyst | Strategist | Sequential, Context7 | High |

## Wave-Enabled Commands

**Wave System Integration**:
- **Complexity Threshold**: ≥0.7 complexity + >20 files + >2 operation types
- **Auto-Activation**: Enterprise projects, multi-phase brand development
- **Persona Orchestration**: Dynamic team assembly based on project needs
- **Resource Scaling**: Automatic resource allocation for complex projects

## Usage Examples

### Complete Brand Development
```bash
# Initialize project
/brandforge init "StartupXYZ" --type startup --industry fintech

# Complete workflow
/brandforge forge --complete-workflow --market-research --user-validation

# Strategic analysis
/brandforge strategy competitive --scope industry --depth comprehensive
```

### Synthetic User Research
```bash
# Generate synthetic users
/brandforge research synthetic --demographic "millennial-parents" --count 50

# Validate concepts
/brandforge validate concept --method synthetic --target "new-parents-app"
```

### Creative Development
```bash
# Design system creation
/brandforge creative design-system --scope comprehensive --format figma-ready

# Brand guidelines
/brandforge creative guidelines --format web-and-print --scalability enterprise
```

BrandForge commands provide complete orchestration for brand development from initial strategy through market launch, with specialized support for synthetic user research and design thinking methodologies.