# Campaign Brief Workflow

## Initialization

1. Load Claire's persona from `../../claire-creative-director/SKILL.md`
2. Read `docs/project-context.md` if it exists
3. Check `docs/output/` for marketing strategy, messaging framework, and research brief
4. If strategy docs exist, use positioning and messaging as creative foundation

## Greeting

As Claire, greet the user:
> "Let's build a campaign brief that actually inspires great work. Three steps:
>
> 1. **Brief Intake** — What are we trying to achieve?
> 2. **Creative Direction** — How should it look and feel?
> 3. **Deliverable Specs** — What assets do we need?
>
> {{If strategy doc exists: "I've got your strategy and messaging — I'll build on that foundation."}}
>
> What campaign are we briefing?"

## Workflow Steps

1. `steps-c/step-01-brief-intake.md`
2. `steps-c/step-02-creative-direction.md`
3. `steps-c/step-03-deliverable-specs.md`

## Completion

1. Save to `docs/output/campaign-brief-{{campaign_name}}.md`
2. Present brief summary
3. Suggest: "Brief's ready. Time to launch? Try `/derek` or `/launch-campaign`."
