# FLAGS.md - BrandForge Flag Reference

Flag system for BrandForge brand strategy framework with auto-activation and conflict resolution.

## Flag System Architecture

**Priority Order**:
1. Safety flags (--safe-mode) > optimization flags
2. Explicit flags > auto-activation
3. Brand-specific > general flags
4. Complexity-based > resource-based
5. Persona flags > command flags
6. Research rigor > speed optimization
7. Last specified takes precedence

## Brand Strategy Flags

### Demographic Targeting

#### `--demographic-profile [profile]`
**Purpose**: Target specific audience demographics for research and strategy
**Format**: `"age=25-40,gender=mixed,income=50k-120k,location=urban,tech=early-adopter,culture=western"
**Auto-activates**: UX Researcher persona, Context7 for demographic data
**Examples**:
```bash
--demographic-profile "millennial-parents,age=28-40,income=75k-150k,location=suburban,values=family-focused"
--demographic-profile "gen-z-professionals,age=22-28,income=40k-80k,location=urban,tech=digital-native"
```

#### `--market-segment [segment]`
**Purpose**: Target specific market segments for analysis
**Options**: `b2b`, `b2c`, `enterprise`, `smb`, `consumer`, `startup`, `scaleup`
**Auto-activates**: Market Analyst persona, Sequential for segmentation

#### `--cultural-context [context]`
**Purpose**: Specify cultural and regional targeting
**Options**: `western`, `asian`, `hispanic`, `african`, `global`, `regional`, `local`
**Auto-activates**: Cultural Strategist persona, Context7 for cultural patterns

### Research Depth Flags

#### `--research-depth [level]`
**Purpose**: Control research comprehensiveness
**Levels**:
- `surface`: Quick market scan and basic positioning
- `standard`: Competitive analysis + user insights
- `comprehensive`: Full market research + user validation
- `ethnographic`: Deep behavioral research + cultural analysis

#### `--validation-method [method]`
**Purpose**: Specify validation approach
**Methods**:
- `synthetic`: Synthetic user research (fast, scalable)
- `traditional`: Real user recruitment (authentic, slower)
- `hybrid`: Combined synthetic + traditional
- `stakeholder`: Internal stakeholder validation
- `market`: Market testing and feedback

#### `--sample-size [size]`
**Purpose**: Control research sample size
**Range**: `1-1000` for synthetic users, `5-100` for traditional research
**Auto-scales**: Based on complexity and resource availability

### Creative Development Flags

#### `--creative-scope [scope]`
**Purpose**: Define creative development boundaries
**Scopes**:
- `identity`: Logo, colors, typography only
- `system`: Complete design system
- `campaign`: Marketing campaign materials
- `experience`: Full brand experience
- `omnichannel`: All touchpoints and channels

#### `--design-system [level]`
**Purpose**: Specify design system comprehensiveness
**Levels**:
- `basic`: Core components and guidelines
- `standard`: Comprehensive component library
- `enterprise`: Scalable system with governance
- `platform`: Multi-brand design system

#### `--brand-guidelines [format]`
**Purpose**: Specify brand guidelines output format
**Formats**:
- `web`: Interactive web guidelines
- `pdf`: Comprehensive PDF document
- `figma`: Figma-ready design system
- `notion`: Collaborative Notion workspace
- `website`: Public brand guidelines website

### Business Strategy Flags

#### `--business-model [type]`
**Purpose**: Specify business model focus
**Types**:
- `startup`: New venture validation
- `enterprise`: Corporate transformation
- `subscription`: SaaS/subscription models
- `marketplace`: Platform business models
- `freemium`: Freemium conversion strategies
- `direct-sales`: DTC business models

#### `--pricing-strategy [strategy]`
**Purpose**: Define pricing approach
**Strategies**:
- `value-based`: Value-based pricing
- `competitive`: Competitive pricing
- `premium`: Premium positioning
- `penetration`: Market penetration
- `skimming`: Price skimming

#### `--go-to-market [approach]`
**Purpose**: Specify launch strategy
**Approaches**:
- `digital-first`: Online-first rollout
- `omnichannel`: Multi-channel launch
- `phased`: Staged deployment
- `surprise`: Surprise launch strategy
- `soft-launch`: Controlled soft launch

### Research & Validation Flags

#### `--synthetic-research [config]`
**Purpose**: Configure synthetic user research
**Config Options**:
- `--persona-count [n]`: Number of synthetic personas (1-1000)
- `--variation-level [level]`: Individual variation within demographic (low/medium/high)
- `--realism-validation`: Cross-validate against real demographic data
- `--follow-up-enabled`: Allow multiple interview sessions
- `--persona-persistence`: Maintain persona memory across sessions

#### `--traditional-research [spec]`
**Purpose**: Configure traditional user research
**Spec Options**:
- `--recruitment-method [method]`: Online, in-person, hybrid
- `--incentive-level [amount]`: Participant compensation
- `--screening-criteria [criteria]`: Participant selection criteria
- `--timeline [duration]`: Research timeline

#### `--validation-depth [depth]`
**Purpose**: Control validation comprehensiveness
**Depths**:
- `concept`: Basic concept validation
- `positioning`: Positioning and messaging validation
- `creative`: Creative concept testing
- `usability`: User experience validation
- `market`: Full market validation

### Market Analysis Flags

#### `--competitive-intelligence [level]`
**Purpose**: Specify competitive analysis depth
**Levels**:
- `basic`: Top 3-5 competitors
- `standard`: Industry landscape analysis
- `comprehensive`: Deep competitive intelligence
- `enterprise`: Global competitive analysis

#### `--market-trends [timeframe]`
**Purpose**: Specify trend analysis timeframe
**Timeframes**:
- `current`: Current market conditions
- `1-year`: 12-month trend analysis
- `3-year`: Medium-term trend analysis
- `5-year`: Long-term strategic trends

#### `--geographic-scope [scope]`
**Purpose**: Define geographic analysis scope
**Scopes**:
- `local`: City/region level
- `national`: Country-wide analysis
- `regional`: Multi-country regions
- `global`: Worldwide market analysis

### Quality & Optimization Flags

#### `--quality-gates [level]`
**Purpose**: Specify quality assurance level
**Levels**:
- `essential`: Basic quality checks
- `standard`: Comprehensive validation
- `enterprise`: Full quality assurance
- `premium`: Premium quality standards

#### `--validation-criteria [criteria]`
**Purpose**: Define validation success criteria
**Criteria**:
- `market-fit`: Product-market fit validation
- `user-satisfaction`: User satisfaction metrics
- `business-impact`: Business outcome validation
- `competitive-advantage`: Competitive differentiation

#### `--performance-metrics [metrics]`
**Purpose**: Specify performance measurement
**Metrics**:
- `awareness`: Brand awareness measurement
- `engagement`: User engagement metrics
- `conversion`: Conversion rate optimization
- `loyalty`: Customer loyalty measurement

### Resource & Timeline Flags

#### `--project-scope [scope]`
**Purpose**: Define project complexity level
**Scopes**:
- `startup`: MVP brand development
- `scaleup`: Growth stage branding
- `enterprise`: Corporate rebrand/transformation
- `product`: Product-specific branding

#### `--timeline [duration]`
**Purpose**: Specify project timeline
**Durations**:
- `rapid`: 1-2 week sprint
- `standard`: 4-6 week project
- `comprehensive`: 8-12 week project
- `enterprise`: 3-6 month transformation

#### `--resource-allocation [level]`
**Purpose**: Specify resource commitment
**Levels**:
- `minimal`: Lean team approach
- `standard`: Balanced team and tools
- `comprehensive`: Full team engagement
- `enterprise`: Dedicated team and premium tools

### Advanced Orchestration Flags

#### `--wave-mode [mode]`
**Purpose**: Control wave orchestration
**Modes**:
- `auto`: Automatic complexity detection
- `force`: Force wave mode
- `off`: Disable wave mode
- `enterprise`: Enterprise-level orchestration

#### `--wave-strategy [strategy]`
**Purpose**: Specify wave orchestration approach
**Strategies**:
- `progressive`: Iterative enhancement
- `systematic`: Methodical phased approach
- `adaptive`: Dynamic configuration
- `enterprise`: Large-scale orchestration

#### `--delegate [strategy]`
**Purpose**: Control task delegation
**Strategies**:
- `files`: File-level delegation
- `folders`: Directory-level delegation
- `personas`: Persona-based delegation
- `auto`: Automatic delegation detection

### Brand-Specific Flags

#### `--brand-personality [personality]`
**Purpose**: Define brand personality archetype
**Personalities**:
- `innovative`: Cutting-edge and forward-thinking
- `trustworthy`: Reliable and established
- `playful`: Fun and approachable
- `premium`: Luxury and exclusivity
- `accessible`: Friendly and inclusive

#### `--brand-voice [voice]`
**Purpose**: Specify brand communication style
**Voices**:
- `professional`: Corporate and authoritative
- `conversational`: Friendly and approachable
- `technical`: Expert and detailed
- `inspiring`: Motivational and aspirational
- `playful`: Fun and engaging

#### `--target-emotion [emotion]`
**Purpose**: Define emotional brand connection
**Emotions**:
- `trust`: Building confidence and reliability
- `excitement`: Creating energy and enthusiasm
- `belonging`: Fostering community and connection
- `security`: Providing safety and stability
- `aspiration**: Inspiring growth and achievement

## Flag Integration Matrix

| Flag Category | Primary Persona | Secondary Persona | MCP Integration | Auto-Triggers |
|---------------|-----------------|-------------------|-----------------|---------------|
| Demographic | UX Researcher | Market Analyst | Context7, Sequential | research commands |
| Research Depth | Researcher | Strategist | Sequential | research commands |
| Creative Scope | Creative Director | Designer | Magic, Context7 | creative commands |
| Business Model | Business Designer | Strategist | Sequential | strategy commands |
| Validation | QA Specialist | Researcher | Sequential, Playwright | validate commands |
| Market Analysis | Market Analyst | Strategist | Context7 | market commands |

## Flag Precedence Rules

### Conflict Resolution
1. **Brand-specific flags** override general flags
2. **Research rigor** overrides speed optimization
3. **Quality gates** override resource constraints
4. **Demographic accuracy** overrides sample size
5. **Ethical considerations** override convenience

### Auto-Activation Patterns

#### Research Commands
```bash
# Auto-activates demographic targeting and research depth
/brandforge research synthetic --persona-count 50
# → Auto-activates: UX Researcher, Sequential, Context7

# Auto-activates market analysis flags
/brandforge strategy competitive --scope industry
# → Auto-activates: Market Analyst, Context7, Sequential
```

#### Creative Commands
```bash
# Auto-activates creative scope and design system
/brandforge creative design-system --scope comprehensive
# → Auto-activates: Creative Director, Magic, Context7
```

#### Validation Commands
```bash
# Auto-activates validation method and quality gates
/brandforge validate concept --method synthetic --validation-depth comprehensive
# → Auto-activates: QA Specialist, Sequential, Playwright
```

## Usage Examples

### Complete Brand Project
```bash
/brandforge forge --from-strategy-to-launch \
  --demographic-profile "millennial-parents,age=28-40,income=75k-150k" \
  --research-depth comprehensive \
  --creative-scope system \
  --business-model subscription \
  --validation-method hybrid \
  --timeline standard \
  --quality-gates enterprise
```

### Synthetic User Research
```bash
/brandforge research synthetic \
  --demographic-profile "gen-z-professionals,age=22-28,income=40k-80k" \
  --persona-count 100 \
  --variation-level high \
  --validation-method synthetic \
  --realism-validation
```

### Creative Development
```bash
/brandforge creative design-system \
  --creative-scope enterprise \
  --design-system comprehensive \
  --brand-guidelines web-and-print \
  --performance-metrics all
```

### Market Analysis
```bash
/brandforge market competitive \
  --competitive-intelligence comprehensive \
  --market-trends 3-year \
  --geographic-scope national \
  --validation-criteria market-fit
```

BrandForge flags provide precise control over every aspect of brand development, from demographic targeting to quality assurance, ensuring optimal outcomes for any brand project scale or complexity."}