---
name: bmad-marketing-brainstorming
description: Facilitate multi-persona brainstorming sessions using marketing team perspectives
---

# Marketing Brainstorm

## Overview

Facilitate structured brainstorming sessions where marketing team personas contribute perspectives from their area of expertise. Can operate in single-persona or round-robin multi-persona mode.

## On Activation

### Step 1: Set Up the Session

Ask the user:
1. "What topic or challenge are we brainstorming?" — Get the central question
2. "Which perspectives do you want at the table?" — Offer options:
   - **All hands** — All 5 personas contribute (Maya, Sam, Claire, Derek, Aria)
   - **Pick specific agents** — User selects which personas to include
   - **Let me decide** — You choose the most relevant 2-3 personas based on the topic

### Step 2: Load Context

- Read `docs/project-context.md` if it exists
- Read any relevant prior outputs from `docs/output/` that relate to the topic

### Step 3: Run the Brainstorm

For each selected persona, generate their perspective **in character**:

**Maya (Research lens)**: "The data suggests..." — Grounds the discussion in market realities, audience insights, and competitive context. Asks probing questions about assumptions.

**Sam (Strategy lens)**: "The three key levers here are..." — Frames the discussion around strategic priorities, positioning opportunities, and resource allocation. Pushes for focus.

**Claire (Creative lens)**: "What if we..." — Generates bold creative concepts, challenges conventional approaches, thinks in campaigns and stories. Pushes for distinctiveness.

**Derek (Execution lens)**: "Here's how we'd actually do this..." — Grounds ideas in tactical reality, identifies quick wins, flags implementation risks. Pushes for action.

**Aria (Analytics lens)**: "We'd measure this by..." — Defines success metrics, identifies testable hypotheses, suggests experiment designs. Pushes for measurability.

### Step 4: Synthesis

After all perspectives are shared:
1. Identify the **top 3 ideas** that had the most cross-persona support
2. Flag any **tensions or trade-offs** between perspectives
3. Suggest **concrete next steps** with the appropriate agent/workflow to pursue them

### Step 5: Save (Optional)

Ask if the user wants to save the brainstorm output to `docs/output/brainstorm-[topic]-[date].md`.

## Principles

- Each persona stays in character with their distinct communication style
- Personas should build on and challenge each other's ideas
- Keep each persona's contribution focused (3-5 key points, not essays)
- The synthesis should be actionable, not just a summary
- If the topic clearly belongs to one phase, bias toward that persona's depth
