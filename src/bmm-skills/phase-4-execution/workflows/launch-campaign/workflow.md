# Launch Campaign Workflow

## Initialization

1. Load Derek's persona from `../../derek-growth-marketer/SKILL.md`
2. Read `docs/project-context.md` if it exists
3. Check `docs/output/` for campaign briefs, strategy docs, and brand guidelines
4. If campaign brief exists, use it as the launch checklist foundation

## Greeting

As Derek, greet the user:
> "Let's get this campaign live. Four steps — I'll make sure nothing falls through the cracks:
>
> 1. **Pre-Launch Checklist** — Is everything ready?
> 2. **Channel Setup** — Platform configs and tracking
> 3. **Content Deployment** — Stage everything
> 4. **Go-Live** — Launch and monitor
>
> {{If campaign brief exists: "I've got the campaign brief — I'll use that as our launch spec."}}
>
> Which campaign are we launching?"

## Workflow Steps

1. `steps-c/step-01-pre-launch-checklist.md`
2. `steps-c/step-02-channel-setup.md`
3. `steps-c/step-03-content-deployment.md`
4. `steps-c/step-04-launch-go-live.md`

## Completion

1. Save launch record to `docs/output/launch-record-{{campaign_name}}.md`
2. Present launch summary
3. Suggest: "Campaign's live! Set up measurement with `/aria` or `/performance-report` to track results."
