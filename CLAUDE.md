# BMAD Marketing Team

This is a marketing team powered by the BMAD method. Each marketing function is handled by a specialist agent with structured workflows that guide you through research, strategy, creative, execution, and analytics.

## Quick Start

1. Run `/marketing-init` to set up your project context (product, audience, goals)
2. Start with `/maya` for market research, then progress through the phases
3. Use `/help` to see all available agents and workflows at any time

All slash commands are registered as Claude Code custom commands in `.claude/commands/`. They are invoked directly as `/command-name` in the CLI.

## Agents

| Agent | Phase | Command | Domain |
|-------|-------|---------|--------|
| Maya | 1 - Research | `/maya` | Market research, audience analysis, competitive intelligence |
| Sam | 2 - Strategy | `/sam` | Marketing strategy, messaging frameworks, content calendars |
| Claire | 3 - Creative | `/claire` | Campaign briefs, brand guidelines, copywriting |
| Derek | 4 - Execution | `/derek` | Campaign launch, email sequences, ad management |
| Aria | 5 - Analytics | `/aria` | Performance reports, A/B test analysis, ROI analysis |

When the user invokes an agent by name (e.g., `/maya`), read and activate the corresponding SKILL.md file:

- `/maya` → `src/bmm-skills/phase-1-research/maya-market-researcher/SKILL.md`
- `/sam` → `src/bmm-skills/phase-2-strategy/sam-marketing-strategist/SKILL.md`
- `/claire` → `src/bmm-skills/phase-3-creative/claire-creative-director/SKILL.md`
- `/derek` → `src/bmm-skills/phase-4-execution/derek-growth-marketer/SKILL.md`
- `/aria` → `src/bmm-skills/phase-5-analytics/aria-analytics-lead/SKILL.md`

## Workflows

| Workflow | Agent | Command | Description |
|----------|-------|---------|-------------|
| Market Research | Maya | `/market-research` | Guided 4-step research process |
| Marketing Strategy | Sam | `/marketing-strategy` | 4-step strategy creation |
| Content Calendar | Sam | `/content-calendar` | 3-step content planning |
| Campaign Brief | Claire | `/campaign-brief` | 3-step creative brief |
| Brand Guidelines | Claire | `/brand-guidelines` | 3-step brand identity guide |
| Launch Campaign | Derek | `/launch-campaign` | 4-step campaign launch |
| Performance Report | Aria | `/performance-report` | 4-step analytics report |

When the user invokes a workflow, read and activate the workflow's SKILL.md, then follow the workflow.md:

- `/market-research` → `src/bmm-skills/phase-1-research/workflows/market-research/SKILL.md`
- `/marketing-strategy` → `src/bmm-skills/phase-2-strategy/workflows/create-marketing-strategy/SKILL.md`
- `/content-calendar` → `src/bmm-skills/phase-2-strategy/workflows/create-content-calendar/SKILL.md`
- `/campaign-brief` → `src/bmm-skills/phase-3-creative/workflows/create-campaign-brief/SKILL.md`
- `/brand-guidelines` → `src/bmm-skills/phase-3-creative/workflows/create-brand-guidelines/SKILL.md`
- `/launch-campaign` → `src/bmm-skills/phase-4-execution/workflows/launch-campaign/SKILL.md`
- `/performance-report` → `src/bmm-skills/phase-5-analytics/workflows/create-performance-report/SKILL.md`

## Utilities

- `/help` → `src/core-skills/help/SKILL.md` — List all agents and workflows
- `/marketing-init` → `src/core-skills/init/SKILL.md` — Set up project context (named `marketing-init` to avoid conflict with Claude Code's built-in `/init`)
- `/brainstorm` → `src/core-skills/brainstorming/SKILL.md` — Multi-persona brainstorming

## Conventions

- All generated output goes to `docs/output/`
- Agents load `docs/project-context.md` on activation if it exists
- Agents reference prior phase outputs when available (e.g., Sam reads Maya's research brief)
- Each workflow is interactive: the agent guides you through steps with menus
- Cross-phase handoffs: agents suggest the next phase agent when their work is complete
