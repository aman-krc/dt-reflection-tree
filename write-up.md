# Design Rationale — The Daily Reflection Tree

## Why these questions

The hardest constraint wasn't technical — it was tonal. The questions had to be honest without being threatening, and the options had to genuinely discriminate between the two poles of each axis without telegraphing a "right answer."

**Axis 1 (Locus)**: I led with the weather metaphor because it lets people name their day without being asked to evaluate it. "Stormy" is descriptively honest in a way "bad" or "I had no control" isn't — people will say it without defensiveness. The follow-up questions then dig for what specifically happened under that weather. The key design decision was putting the "agency question" *after* the weather routing: the high-agency branch asks "what made things go well?" while the low-agency branch asks "what did you do first?" — subtly different questions that surface the same underlying dimension (did you see yourself as actor or subject?) but feel calibrated to where the person already is.

**Axis 2 (Orientation)**: The entitlement axis is the trickiest to surface without shame. Nobody says "I felt entitled today." So I never used that word. Instead I asked about *interactions* (giving vs. receiving), *unsolicited effort* (what did you do that nobody asked for?), and *recognition* (how did credit feel?). The "I felt like I gave more than I received" option is critical — it captures the entitled person who would never identify as entitled, because their experience feels like victimhood, not greed. If I hadn't included it on the contribution/entitlement routing question, the tree would miss the most common form of workplace entitlement.

**Axis 3 (Radius)**: Maslow's self-transcendence is the hardest to ask about directly, so I asked it spatially — "whose experience comes to mind first?" The options progress literally from narrow to wide radius of concern (Mine → My team → A specific person → The customer), which lets people locate themselves without a judgment frame. I added the `A3_Q_MEANING` node as a reward branch: people who showed genuine concern for others get the deeper question about purpose. This creates a small but meaningful asymmetry between the paths.

## Branching design

The tree has two core branching moments per axis:
1. **Orientation routing** (the opening question of each axis), which routes to either a high or low branch
2. **Confirmation routing** (the second question), which either confirms or softens the initial signal

This double-routing design means a single early answer doesn't lock the conversation. Someone who says "Stormy" can still be routed toward the internal-locus reflection if their second answer shows agency. The signal tallying handles this — reflections are chosen by dominant signal across both questions, not the first answer alone.

The bridge nodes are the most underrated design decision. They don't just announce a transition — they provide a semantic connection between axes: "from how you handled today — to what you gave" explicitly links Axis 1 (agency/locus) to Axis 2 (orientation toward others). This makes the conversation feel like a single arc, not three separate quizzes.

**Trade-off I made**: I kept the tree to 3-4 nodes per axis rather than 5-6. More nodes would allow finer discrimination, but arriving at a reflection tool tired at 7pm and answering 15 questions is a poor experience. Depth was sacrificed for cadence.

## Psychological sources

**Rotter (1954)** — Locus of Control: The foundational framework for Axis 1. I drew on Rotter's original insight that internal LOC isn't about believing you control *outcomes*, but about believing your *actions are connected to outcomes*. This distinction shapes how I wrote the question options — the internal options are about choice and adaptation, not success.

**Dweck (2006)** — Growth Mindset: Informs the "what made it happen?" question on the high-agency branch. Fixed mindset attribution ("I'm good at this") vs. growth mindset attribution ("I prepared / I adapted") is captured in the option structure without naming it.

**Campbell et al. (2004)** — Psychological Entitlement Scale: The recognition questions in Axis 2 draw on PES items. The key insight from that literature is that entitlement is cognitively invisible to the person holding it — they experience it as legitimate expectation, not excess. That's why "I felt like I gave more than I received" is routed to the entitlement branch, not the contribution branch.

**Organ (1988)** — Organizational Citizenship Behavior: The "what did you do that no one asked for?" question is directly measuring OCB. Organ's categories (altruism, conscientiousness, sportsmanship, courtesy) informed the option choices.

**Maslow (1969)** — The Farther Reaches of Human Nature: The self-transcendence concept in Axis 3. Maslow's later work argued that peak experiences and mature development involve orientation beyond the self — not selflessness, but *meaning-through-others*. The `A3_Q_MEANING` node is designed to surface exactly this: not "did you help someone" (behavior) but "does the work feel connected to something larger" (meaning).

## What I'd improve with more time

1. **Longitudinal state**: The most valuable insight would come from comparing today's session to yesterday's. The tree currently has no memory. A minimal weekly view — "last three days: external, internal, external" — would be more actionable than any single session.

2. **Finer axis discrimination**: The 4-option constraint works but flattens nuance. A second-level question distinguishing "internal locus because I trust myself" from "internal locus because I've learned to control my reactions" would be psychologically richer.

3. **The missing A2 branch**: There's currently no branch for the person who is genuinely neutral on orientation — who gave freely *and* felt fairly recognized. The `A2_R_MIXED` reflection handles this adequately, but the routing logic forcing a binary split on the opening question is a real limitation.

4. **Tone testing**: I'd want to test the reflection text with real employees — specifically the "entitlement" and "external locus" reflections, which risk feeling preachy even when I've tried to avoid it. The line "the question worth sitting with is..." is the one I'm most uncertain about.
