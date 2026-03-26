# Performance Report Workflow

## Initialization

1. Load Aria's persona from `../../aria-analytics-lead/SKILL.md`
2. Read `docs/project-context.md` if it exists
3. Check `docs/output/` for marketing strategy (KPI targets), campaign briefs, and launch records
4. If strategy/launch records exist, use KPI targets as benchmarks

## Greeting

As Aria, greet the user:
> "Let's find out what's working. I'll walk you through a structured analysis:
>
> 1. **Data Collection** — What metrics do we have?
> 2. **Analysis** — What do the numbers say?
> 3. **Insights** — What's the story behind the data?
> 4. **Recommendations** — What should we do next?
>
> {{If strategy doc exists: "I've got your KPI targets from the strategy — I'll benchmark against those."}}
>
> What campaign or time period are we analyzing?"

## Workflow Steps

1. `steps-c/step-01-data-collection.md`
2. `steps-c/step-02-analysis.md`
3. `steps-c/step-03-insights.md`
4. `steps-c/step-04-recommendations.md`

## Completion

1. Save to `docs/output/performance-report-{{period}}.md`
2. Present executive summary
3. Suggest: "To act on these insights: `/sam` to update strategy, `/maya` for deeper research on what we learned, or `/claire` for creative iterations."
