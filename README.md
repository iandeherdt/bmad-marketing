# BMAD Marketing Team

A marketing team framework powered by the [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD), designed for use with Claude CLI. Five specialist AI agents guide you through the full marketing lifecycle — from market research to performance analytics.

## Prerequisites

- [Claude CLI](https://docs.anthropic.com/en/docs/claude-code) installed and authenticated

## Getting Started

1. Clone the repository:
   ```bash
   git clone git@github.com:iandeherdt/bmad-marketing.git
   cd bmad-marketing
   ```

2. Start Claude CLI:
   ```bash
   claude
   ```

3. Initialize your project:
   ```
   /marketing-init
   ```
   This creates `docs/project-context.md` with your product, audience, and goals. All agents reference this context automatically.

4. Start working with any agent or workflow:
   ```
   /maya
   /marketing-strategy
   ```

## The Team

Five specialist agents, each owning a phase of the marketing lifecycle:

| Phase | Agent | Command | What They Do |
|-------|-------|---------|-------------|
| 1. Research | **Maya** | `/maya` | Market research, audience personas, competitive intelligence |
| 2. Strategy | **Sam** | `/sam` | Marketing strategy, positioning, messaging, content calendars |
| 3. Creative | **Claire** | `/claire` | Campaign briefs, brand guidelines, copywriting |
| 4. Execution | **Derek** | `/derek` | Campaign launches, email sequences, ad setup |
| 5. Analytics | **Aria** | `/aria` | Performance reports, A/B tests, ROI analysis |

Each agent has a distinct personality and communication style. They stay in character throughout the conversation and suggest the next agent when their phase is complete.

## Workflows

Guided step-by-step processes that walk you through creating specific deliverables:

| Workflow | Agent | Command | Steps |
|----------|-------|---------|-------|
| Market Research | Maya | `/market-research` | Define Scope → Audience Analysis → Competitive Intel → Synthesis |
| Marketing Strategy | Sam | `/marketing-strategy` | Situation Analysis → Positioning → Channel Strategy → Campaign Plan |
| Content Calendar | Sam | `/content-calendar` | Content Pillars → Channel Mapping → Calendar Build |
| Campaign Brief | Claire | `/campaign-brief` | Brief Intake → Creative Direction → Deliverable Specs |
| Brand Guidelines | Claire | `/brand-guidelines` | Brand Audit → Voice & Tone → Visual Identity |
| Launch Campaign | Derek | `/launch-campaign` | Pre-Launch Checklist → Channel Setup → Deployment → Go-Live |
| Performance Report | Aria | `/performance-report` | Data Collection → Analysis → Insights → Recommendations |

Each workflow step includes an interactive menu:
- **[P] Proceed** — Move to the next step
- **[R] Revise** — Adjust the current step
- **[S] Save & Exit** — Save progress and exit
- **[B] Back** — Return to the previous step

## Utilities

| Command | Description |
|---------|-------------|
| `/help` | List all agents, workflows, and commands |
| `/marketing-init` | Set up or update project context |
| `/brainstorm` | Multi-persona brainstorming session (pick which agents contribute) |

## Recommended Flow

The phases are designed to flow naturally into each other:

```
/marketing-init → /maya → /sam → /claire → /derek → /aria
                                                          ↓
                                    Feed insights back into /sam or /maya
```

1. **`/marketing-init`** — Set up your product, audience, and goals
2. **`/maya`** or **`/market-research`** — Research your market and audience
3. **`/sam`** or **`/marketing-strategy`** — Build your strategy and messaging
4. **`/claire`** or **`/campaign-brief`** — Create campaign briefs and brand guidelines
5. **`/derek`** or **`/launch-campaign`** — Launch and deploy campaigns
6. **`/aria`** or **`/performance-report`** — Measure results and get recommendations
7. Feed Aria's insights back into Sam (strategy updates) or Maya (new research)

You don't have to follow this order. Each agent works independently — jump to whichever phase you need.

## Output

All generated deliverables are saved to `docs/output/`:

- Market research briefs and competitive landscapes
- Marketing strategy documents and messaging frameworks
- Content calendars
- Campaign briefs and design briefs
- Brand guidelines
- Launch checklists and email sequences
- Performance dashboards and A/B test reports

## Project Structure

```
bmad-marketing/
├── .claude/commands/            # Claude CLI slash commands (registered skills)
├── CLAUDE.md                    # Agent routing and project conventions
├── module.yaml                  # Project configuration
├── docs/output/                 # Generated deliverables
└── src/
    ├── core-skills/             # Utilities (help, init, brainstorming)
    └── bmm-skills/
        ├── phase-1-research/    # Maya + market research workflow
        ├── phase-2-strategy/    # Sam + strategy & content calendar workflows
        ├── phase-3-creative/    # Claire + campaign brief & brand guidelines workflows
        ├── phase-4-execution/   # Derek + launch campaign workflow
        └── phase-5-analytics/   # Aria + performance report workflow
```

Each workflow follows the BMAD pattern:
- `SKILL.md` — Agent persona with capabilities table
- `workflow.md` — Workflow initialization and step routing
- `steps-c/` — Sequential step files with execution protocols
- `templates/` — Output document templates

## Customization

- **Edit agent personas** in `src/bmm-skills/phase-*/agent-name/SKILL.md` to adjust personality, expertise, or capabilities
- **Modify workflows** by editing step files in `steps-c/` or adding new steps
- **Update templates** in `templates/` to match your preferred output format
- **Add new workflows** by creating a new directory with SKILL.md, workflow.md, steps, and templates, then add a command file in `.claude/commands/` and register it in `CLAUDE.md`
