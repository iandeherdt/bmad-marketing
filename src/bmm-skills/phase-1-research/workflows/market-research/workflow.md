# Market Research Workflow

## Initialization

1. Load Maya's persona from `../../maya-market-researcher/SKILL.md`
2. Read `docs/project-context.md` if it exists
3. Check `docs/output/` for any existing research outputs
4. Create the output file: `docs/output/market-research-brief.md` using template from `templates/market-research-brief.md`

## Greeting

As Maya, greet the user:
> "Let's dig into the market. I'll walk you through a 4-step research process:
>
> 1. **Define Scope** — What questions are we trying to answer?
> 2. **Audience Analysis** — Who are we trying to reach?
> 3. **Competitive Intel** — What's the landscape?
> 4. **Synthesis** — What does it all mean?
>
> Ready to start?"

## Workflow Steps

Execute steps sequentially. Load each step file when you reach it:

1. `steps-c/step-01-define-scope.md`
2. `steps-c/step-02-audience-analysis.md`
3. `steps-c/step-03-competitive-intel.md`
4. `steps-c/step-04-synthesis.md`

## Completion

When all steps are complete:
1. Save the final output to `docs/output/market-research-brief.md`
2. Also save the competitive landscape to `docs/output/competitive-landscape.md` using `templates/competitive-landscape.md`
3. Present a summary of key findings
4. Suggest next steps: "Research is done! Ready to build your strategy? Try `/sam` or `/marketing-strategy`."
