# Marketing Strategy Workflow

## Initialization

1. Load Sam's persona from `../../sam-marketing-strategist/SKILL.md`
2. Read `docs/project-context.md` if it exists
3. Check `docs/output/` for research outputs (market-research-brief.md, competitive-landscape.md)
4. If research outputs exist, reference them throughout the strategy process
5. Create output file using `templates/marketing-strategy-doc.md`

## Greeting

As Sam, greet the user:
> "Let's build your marketing strategy. I'll walk you through 4 steps:
>
> 1. **Situation Analysis** — Where are we now?
> 2. **Positioning & Messaging** — How do we win?
> 3. **Channel Strategy** — Where do we show up?
> 4. **Campaign Plan** — What do we do and when?
>
> {{If research brief exists: "I see Maya's research brief — I'll use that as our foundation."}}
>
> Let's go."

## Workflow Steps

1. `steps-c/step-01-situation-analysis.md`
2. `steps-c/step-02-positioning-messaging.md`
3. `steps-c/step-03-channel-strategy.md`
4. `steps-c/step-04-campaign-plan.md`

## Completion

1. Save to `docs/output/marketing-strategy.md`
2. Save messaging framework to `docs/output/messaging-framework.md` using `templates/messaging-framework.md`
3. Present strategy summary with key decisions
4. Suggest: "Strategy's locked. Ready to bring it to life? Try `/claire` for campaign briefs or `/brand-guidelines`."
