# ORCHESTRATOR.md - BrandForge Intelligent Routing System

Intelligent routing system for BrandForge brand strategy framework.

## 🧠 Detection Engine

Advanced brand context analysis to understand intent, complexity, and strategic requirements.

### Pre-Operation Validation Checks

**Brand Resource Validation**:
- Market data accuracy prediction based on research scope and demographics
- Creative asset requirements estimation for brand deliverables
- Brand guideline complexity and stakeholder coordination needs
- MCP server availability for brand-specific integrations
- Cultural context depth assessment for global brand projects

**Brand Compatibility Validation**:
- Flag combination conflict detection (e.g., `--cultural-context` with `--global-scope`)
- Persona + brand command compatibility verification
- Brand tool availability for requested creative operations
- Project structure requirements for brand asset management
- Stakeholder alignment validation for enterprise projects

**Brand Risk Assessment**:
- Brand complexity scoring (0.0-1.0 scale) for strategic challenges
- Market risk probability based on competitive landscape
- Cultural sensitivity risk for global brand positioning
- Creative execution risk based on technical requirements
- Stakeholder misalignment risk for multi-party projects

**Validation Logic**: Brand resource availability, demographic targeting accuracy, cultural context completeness, competitive intelligence quality, and strategic recommendation safety.

**Brand Resource Management Thresholds**:
- **Green Zone** (0-60%): Standard brand projects, predictive monitoring active
- **Yellow Zone** (60-75%): Complex brand projects, cultural optimization, suggest `--uc` mode
- **Orange Zone** (75-85%): Enterprise brand projects, stakeholder coordination warnings
- **Red Zone** (85-95%): Multi-market brands, force efficiency modes, block resource-intensive operations
- **Critical Zone** (95%+): Global brand launches, emergency protocols, essential operations only

### Brand Pattern Recognition Rules

#### Brand Complexity Detection
```yaml
simple:
  indicators:
    - single market brand development
    - basic visual identity creation
    - straightforward positioning statements
    - < 3 stakeholder groups
    - local market focus
  token_budget: 5K
  time_estimate: < 5 min

moderate:
  indicators:
    - multi-market brand development
    - comprehensive design system creation
    - competitive analysis projects
    - 3-10 stakeholder groups
    - regional market focus
  token_budget: 15K
  time_estimate: 5-30 min

complex:
  indicators:
    - global brand architecture
    - enterprise rebrand projects
    - multi-stakeholder coordination
    - cultural localization requirements
    - > 10 stakeholder groups
  token_budget: 30K+
  time_estimate: > 30 min
```

#### Brand Domain Identification
```yaml
brand-strategy:
  keywords: [positioning, strategy, competitive, market, differentiation, value-proposition]
  typical_operations: [strategy development, competitive analysis, positioning]
  auto_personas: [strategist, market-analyst, architect]

creative-development:
  keywords: [identity, design, creative, visual, guidelines, design-system]
  typical_operations: [visual identity, design system, creative concepts]
  auto_personas: [creative-director, brand-qa, brand-scribe]

user-research:
  keywords: [user, research, ethnographic, persona, demographic, validation]
  typical_operations: [user research, validation, market research]
  auto_personas: [ux-researcher, cultural-strategist, market-analyst]

business-design:
  keywords: [business, model, pricing, go-to-market, scaling, growth]
  typical_operations: [business model, pricing strategy, market entry]
  auto_personas: [business-designer, strategist, launch-manager]

content-strategy:
  keywords: [content, messaging, voice, storytelling, brand-voice]
  typical_operations: [content strategy, messaging, brand voice]
  auto_personas: [content-strategist, brand-scribe, strategist]

synthetic-research:
  keywords: [synthetic, persona-generation, demographic-targeting, user-validation]
  typical_operations: [synthetic user research, persona creation, validation]
  auto_personas: [ux-researcher, cultural-strategist, brand-analyzer]

enterprise-brand:
  keywords: [enterprise, rebrand, transformation, stakeholder, global]
  typical_operations: [enterprise strategy, stakeholder alignment, global rollout]
  auto_personas: [architect, launch-manager, brand-qa]

wave_eligible:
  keywords: [comprehensive, global, enterprise, transformation, systematic]
  complexity_indicators: [multi-market, cultural-adaptation, stakeholder-coordination]
  operation_indicators: [complete-rebrand, global-launch, enterprise-transformation]
  scale_indicators: [global, enterprise, multi-stakeholder, cross-cultural]
  typical_operations: [comprehensive-brand-development, global-brand-strategy, enterprise-transformation]
```

#### Brand Operation Classification
```yaml
strategic-analysis:
  verbs: [analyze, strategize, position, differentiate, compete]
  outputs: [brand strategy, competitive analysis, positioning frameworks]
  typical_tools: [Context7, Sequential, brand-analyzer]

creative-development:
  verbs: [design, create, develop, visualize, conceptualize]
  outputs: [visual identity, design systems, creative concepts]
  typical_tools: [Magic, Sequential, creative-director]

research-execution:
  verbs: [research, validate, test, interview, survey]
  outputs: [user insights, market research, validation reports]
  typical_tools: [Sequential, Playwright, ux-researcher]

launch-orchestration:
  verbs: [launch, rollout, deploy, implement, coordinate]
  outputs: [launch strategies, rollout plans, implementation guides]
  typical_tools: [Sequential, launch-manager, stakeholder-coordination]

iterative-brand-improvement:
  verbs: [improve, refine, optimize, enhance, polish]
  outputs: [brand refinements, optimization strategies, enhancement plans]
  typical_tools: [Sequential, brand-analyzer, brand-qa]
```

## 🚦 Brand Routing Intelligence

Dynamic decision trees mapping brand patterns to optimal persona combinations and orchestration strategies.

### Brand Wave Orchestration Engine
**Multi-stage brand development with compound intelligence. Automatic complexity assessment or explicit flag control.**

**Brand Wave Control Matrix**:
```yaml
wave-activation:
  automatic: "brand complexity >= 0.7 AND stakeholders > 5 AND markets > 1"
  explicit: "--wave-mode, --force-waves"
  override: "--single-wave, --wave-dry-run"
  
wave-strategies:
  progressive: "Iterative brand enhancement and refinement"
  systematic: "Methodical phased brand development"
  adaptive: "Dynamic brand configuration based on market feedback"
  enterprise: "Large-scale brand orchestration for global projects"
```

**Brand Wave-Enabled Commands**:
- **Tier 1**: `/brandforge forge`, `/brandforge strategy`, `/brandforge launch`, `/brandforge validate`
- **Tier 2**: `/brandforge creative`, `/brandforge research`, `/brandforge improve`

### Master Brand Routing Table

| Brand Pattern | Complexity | Domain | Auto-Activates | Confidence |
|---------------|------------|---------|----------------|------------|
| "develop global brand" | complex | enterprise | architect + strategist + cultural-strategist + --ultrathink | 95% |
| "create brand identity" | moderate | creative | creative-director + brand-qa + --uc | 90% |
| "position against competitors" | moderate | strategy | strategist + market-analyst + --seq | 88% |
| "validate with synthetic users" | moderate | research | ux-researcher + cultural-strategist + --seq | 92% |
| "enterprise rebrand" | complex | enterprise | architect + launch-manager + --wave-mode | 94% |
| "cultural brand adaptation" | complex | cultural | cultural-strategist + strategist + --think-hard | 90% |
| "complete brand strategy" | complex | strategy | all personas + --wave-mode + --validate | 95% |
| "startup brand development" | simple | startup | strategist + creative-director + --uc | 85% |
| "competitive analysis" | moderate | market | market-analyst + strategist + --think | 85% |
| "design system creation" | moderate | creative | creative-director + brand-qa + --magic | 90% |
| "user research validation" | moderate | research | ux-researcher + brand-analyzer + --play | 90% |
| "business model innovation" | complex | business | business-designer + strategist + --think-hard | 95% |
| "global brand analysis" | complex | enterprise | brand-analyzer + architect + --delegate --parallel-markets | 95% |
| "comprehensive rebrand" | complex | enterprise | --wave-mode --enterprise-waves --wave-validation | 92% |
| "cultural brand audit" | complex | cultural | --wave-mode --wave-validation --systematic-waves | 94% |

### Brand Decision Trees

#### Tool Selection Logic for Brands

**Base Brand Tool Selection**:
- **Market Research**: Context7 (industry data) or Sequential (strategic analysis)
- **Creative Development**: Magic (design systems) or Sequential (concept development)
- **User Research**: Sequential (methodology) or Playwright (experience testing)
- **Brand Testing**: Playwright (consistency) or Sequential (strategic validation)

#### Brand Delegation & Wave Evaluation

**Brand Delegation Scoring Factors**:
- **Brand Complexity >0.6**: +0.3 score for strategic challenges
- **Multi-market Operations**: +0.4 for global brand projects
- **High Stakeholder Count >5**: +0.2 score for coordination complexity
- **Cultural Adaptation Requirements**: +0.1 per culture/market
- **Creative Asset Volume >50**: +0.2 for design system complexity

**Brand Wave Opportunity Scoring**:
- **High Brand Complexity >0.8**: +0.4 score for strategic challenges
- **Multiple Operation Types >2**: +0.3 score for comprehensive projects
- **Global Market Requirements**: +0.2 score for cultural adaptation
- **Enterprise Stakeholder Count >10**: +0.1 score for coordination complexity
- **Cross-cultural Indicators**: +0.2 for cultural sensitivity requirements
- **Brand Transformation Scale**: +0.15 score for enterprise impact

**Brand Strategy Recommendations**:
- **Wave Score >0.7**: Use brand wave strategies for complex projects
- **Markets >3**: `parallel_markets` delegation for global brands
- **Cultural Contexts >2**: `parallel_cultures` for multicultural brands
- **High Complexity**: `adaptive_delegation` for strategic challenges
- **Default**: `single_brand_strategy` for focused projects

**Brand Wave Strategy Selection**:
- **Cultural Focus**: `wave_validation` for cultural brand projects
- **Creative Focus**: `progressive_waves` for design system development
- **Strategic Focus**: `systematic_waves` for brand architecture projects
- **Enterprise Scale**: `enterprise_waves` for global brand transformations
- **Multi-stakeholder**: `adaptive_waves` for complex stakeholder coordination

## Brand-Specific Auto-Delegation Triggers

### Cultural Brand Projects
```yaml
cultural_threshold:
  condition: cultural_contexts > 2 AND brand_complexity > 0.6
  action: auto_enable --delegate --parallel-cultures
  confidence: 95%
  personas: [cultural-strategist, strategist, ux-researcher]

global_brand:
  condition: markets > 5 OR stakeholders > 15
  action: auto_enable --wave-mode --enterprise-waves
  confidence: 90%
  personas: [architect, launch-manager, cultural-strategist]

multi_stakeholder:
  condition: stakeholder_groups > 7 AND complexity > 0.7
  action: auto_enable --delegate --stakeholder-coordination
  confidence: 85%
  personas: [launch-manager, strategist, brand-qa]

enterprise_rebrand:
  condition: enterprise_context AND structural_changes AND complexity > 0.8
  action: auto_enable --wave-mode --systematic-waves --wave-validation
  confidence: 93%
  personas: [architect, strategist, launch-manager]

```

### Brand-Specific Delegation Routing

| Brand Operation | Complexity | Auto-Delegates | Performance Gain |
|-----------------|------------|----------------|------------------|
| `/brandforge global-analysis` | high | --delegate --parallel-markets | 70% |
| `/brandforge cultural-adaptation` | high | --multi-agent --parallel-cultures | 75% |
| `/brandforge enterprise-rebrand` | high | --wave-mode --progressive-waves | 80% |
| `/brandforge multi-stakeholder-launch` | high | --wave-mode --wave-validation | 85% |
| `/brandforge systematic-brand-improvement` | high | --wave-mode --systematic-waves | 75% |

### Brand Persona Specialization Matrix

**Brand Strategy**: strategist persona, positioning/market-focus, Context7/Sequential tools
**Cultural Analysis**: cultural-strategist persona, demographics/cultural-focus, Context7/Sequential tools
**Creative Development**: creative-director persona, visual/systems-focus, Magic/Sequential tools
**User Research**: ux-researcher persona, insights/validation-focus, Sequential/Playwright tools
**Business Integration**: business-designer persona, models/value-focus, Sequential/Context7 tools
**Quality Assurance**: brand-qa persona, consistency/standards-focus, Sequential/All tools
**Launch Coordination**: launch-manager persona, implementation/stakeholder-focus, Sequential/Context7 tools
**Performance Analysis**: brand-analyzer persona, metrics/optimization-focus, Sequential/Context7 tools
**Knowledge Transfer**: brand-mentor persona, education/guidance-focus, Context7/Sequential tools
**Documentation**: brand-scribe persona, guidelines/process-focus, Scribe/Context7 tools

### Brand Wave-Specific Specialization

**Research Phase**: ux-researcher + cultural-strategist + market-analyst for comprehensive insights
**Strategy Phase**: strategist + architect + business-designer for strategic alignment
**Creative Phase**: creative-director + content-strategist + brand-qa for creative excellence
**Validation Phase**: brand-qa + ux-researcher + brand-analyzer for comprehensive validation
**Launch Phase**: launch-manager + architect + stakeholder-coordination for successful rollout
**Optimization Phase**: brand-analyzer + strategist + performance-specialist for continuous improvement

## Brand Quality Gates & Validation

### 10-Step Brand Validation Cycle
```yaml
brand_quality_gates:
  step_1_strategy: "Strategic alignment validation with Context7 market data"
  step_2_cultural: "Cultural sensitivity validation with cultural context analysis"
  step_3_creative: "Creative consistency validation with brand guideline compliance"
  step_4_research: "User research validation with methodological rigor"
  step_5_competitive: "Competitive positioning validation with market intelligence"
  step_6_stakeholder: "Stakeholder alignment validation with expectation management"
  step_7_accessibility: "Brand accessibility validation with WCAG compliance"
  step_8_implementation: "Technical feasibility validation across all touchpoints"
  step_9_performance: "Brand performance validation with measurable KPIs"
  step_10_sustainability: "Long-term brand sustainability validation"

brand_validation_automation:
  cultural_integration: "Cultural context validation at every step"
  stakeholder_coordination: "Multi-stakeholder validation throughout process"
  market_alignment: "Market opportunity validation at strategic checkpoints"
  creative_consistency: "Cross-platform brand consistency validation"

wave_integration:
  validation_across_waves: "Brand validation at wave boundaries with rollback capability"
  compound_validation: "AI orchestration with brand-specific quality gates"
  cultural_checkpoint: "Cultural sensitivity validation at every wave transition"
```

### Brand Task Completion Criteria
```yaml
completion_requirements:
  strategic_validation: "All 10 brand validation steps passed with cultural context"
  stakeholder_alignment: "All key stakeholders validated and aligned"
  cultural_appropriateness: "Cultural sensitivity validated across all markets"
  market_fit: "Positioning validated against actual competitive landscape"
  creative_excellence: "Creative assets meet brand quality standards"
  implementation_readiness: "Technical implementation validated across all touchpoints"

evidence_requirements:
  strategic: "Market analysis, competitive positioning, strategic frameworks"
  cultural: "Cultural context analysis, demographic insights, sensitivity review"
  creative: "Design system validation, brand guideline compliance, asset optimization"
  performance: "Brand metrics, user feedback, market response data"
  stakeholder: "Alignment documentation, approval records, change management"
```

## ⚡ Brand Performance Optimization

**Intelligent Brand Resource Management**: Real-time monitoring with <100ms brand decisions

**Brand Token Management**: Intelligent allocation based on cultural complexity and stakeholder coordination needs

**Brand Operation Batching**:
- **Cultural Coordination**: Parallel cultural context analysis across markets
- **Stakeholder Synchronization**: Batch stakeholder communication and validation
- **Creative Asset Optimization**: Parallel brand asset generation and optimization
- **Market Research**: Simultaneous competitive analysis across markets

**Brand Resource Distribution**: Dynamic allocation across cultural contexts and stakeholder groups

## 🔗 Brand Integration Intelligence

### Brand-Specific Server Selection Matrix
- **Market Context**: Context7 for competitive intelligence and market data
- **Strategic Analysis**: Sequential for brand strategy and stakeholder coordination
- **Creative Development**: Magic for design systems and brand asset creation
- **User Experience**: Playwright for brand testing and validation
- **Cultural Intelligence**: Context7 for cultural insights and demographic analysis
- **Synthetic Research**: Sequential for synthetic user coordination and validation

### Brand Crisis and Issue Handling
**Brand Crisis Protocols**:
- **Cultural Misalignment**: Immediate cultural consultation and adjustment
- **Stakeholder Disagreement**: Facilitated alignment sessions and compromise solutions
- **Market Positioning Issues**: Rapid competitive reanalysis and repositioning
- **Creative Consistency Problems**: Systematic brand audit and correction
- **Technical Implementation Failures**: Technical review and remediation planning

BrandForge's orchestrator provides intelligent routing for complex brand development projects, ensuring optimal persona activation, cultural sensitivity, and stakeholder coordination for world-class brand strategy outcomes."}