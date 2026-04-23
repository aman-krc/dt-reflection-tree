# Transcript: Persona 2 — Internal / Contributing / Altrocentric

**Profile**: Product manager. A deployment went sideways midday — he had to replan the afternoon and support a junior engineer who was panicking. The outcome was imperfect but the team held together. He arrives reflective and moderately tired.

---

**[START]**
> Good evening. Let's take five minutes to look at your day — not to judge it, just to see it clearly.

*[Employee clicks Begin →]*

---

**[A1_OPEN]** Axis I — Locus
> If today had a weather forecast, what would it be?

**Selected**: *"Partly cloudy — mixed bag"*

*→ Routed to: A1_D1 → A1_Q_AGENCY_HIGH (high agency branch)*

---

**[A1_Q_AGENCY_HIGH]** Axis I — Locus
> You described today as "Partly cloudy — mixed bag". When something went well, what was the main reason?

**Selected**: *"I stayed flexible and adapted"*

*→ Routed to: A1_D2_HIGH → A1_Q_CHOICE_INT (internal locus branch)*

---

**[A1_Q_CHOICE_INT]** Axis I — Locus
> Think of one specific moment today that didn't go to plan. What choice did you make — even a small one?

**Selected**: *"I asked someone for help"*

*→ Signal recorded: axis1:internal*
*→ Routed to: A1_D3 → A1_R_INT*

---

**[A1_R_INT]** Reflection
> You stayed in the driver's seat today — even when the road got rough. That's agency. It doesn't mean everything went your way. It means you kept choosing. Notice that.

*→ Signal recorded: axis1:internal*
*→ Auto-advances to BRIDGE_1_2*

---

**[BRIDGE_1_2]** Bridge
> Now let's shift from how you handled today — to what you gave.

*→ Auto-advances to A2_OPEN*

---

**[A2_OPEN]** Axis II — Orientation
> Think of someone you interacted with today — a colleague, a teammate, anyone. Which of these felt most true?

**Selected**: *"I gave them something — time, help, attention"*

*→ Routed to: A2_D1 → A2_Q_CONTRIB (contribution branch)*

---

**[A2_Q_CONTRIB]** Axis II — Orientation
> What's one thing you did today that no one asked you to do?

**Selected**: *"Helped someone who was stuck"*

*→ Signal recorded: axis2:contribution*
*→ Routed to: A2_D2_C → A2_R_CONTRIB*

---

**[A2_R_CONTRIB]** Reflection
> You were giving today. That's not small. The work that gets done without anyone asking for it — the help that shows up before someone has to ask — that's what holds teams together. You did some of that.

*→ Signal recorded: axis2:contribution*
*→ Auto-advances to BRIDGE_2_3*

---

**[BRIDGE_2_3]** Bridge
> Last shift. From what you gave — to who you were thinking about when you gave it.

*→ Auto-advances to A3_OPEN*

---

**[A3_OPEN]** Axis III — Radius
> When you think about today's biggest challenge, whose experience comes to mind first?

**Selected**: *"A specific person who had it harder than me"*

*→ Routed to: A3_D1 → A3_Q_ALTO (altrocentric branch)*

---

**[A3_Q_ALTO]** Axis III — Radius
> You thought about others in that challenge. Did that shift how you approached it?

**Selected**: *"Yes — it made me more patient or careful"*

*→ Signal recorded: axis3:altrocentric*
*→ Routed to: A3_D2_A → A3_Q_MEANING*

---

**[A3_Q_MEANING]** Axis III — Radius
> When you think about the work you did today — the effort, the stress, even the frustration — does it feel like it was in service of something beyond yourself?

**Selected**: *"Somewhat — I believe in the work even when it's hard"*

*→ Routed to: A3_D3 → A3_R_ALTO*

---

**[A3_R_ALTO]** Reflection
> You're carrying others with you — not as a burden, but as a compass. That's what makes hard days tolerable: knowing they're not just about you. The meaning lives in the gap between you and the person your work reaches.

*→ Signal recorded: axis3:altrocentric*
*→ Auto-advances to SUMMARY*

---

**[SUMMARY]**

**Axis state at summary:**
- axis1: internal=2, external=0 → dominant: **internal**
- axis2: contribution=2, entitlement=0 → dominant: **contribution**
- axis3: altrocentric=2, selfcentric=0 → dominant: **altrocentric**

**Summary key**: `internal+contribution+altrocentric`

> **Today's reflection**
>
> Here's what today looked like.
>
> **Axis I · Locus** — You owned your choices
> **Axis II · Orientation** — You gave more than you counted
> **Axis III · Radius** — You thought beyond yourself
>
> *That's a day worth building on. Agency, generosity, and perspective — when all three line up, the work means something.*

---

**[END]**
> See you tomorrow.

---

## Path analysis

This persona traveled the highest-agency, most contribution-oriented, most outward-focused branches. Notice that the tree still asked him hard questions — it didn't assume the positive answers. The question "Did that shift how you approached it?" required a genuine choice, and he gave an honest answer rather than an obviously virtuous one. The closing reflection affirms without inflating — "a day worth building on" not "you're a hero."

The `A3_Q_MEANING` node added an extra step here (versus persona 1 who hit `A3_R_SELF` directly) — because he checked in on someone, he got the deeper question about purpose. That's a small but meaningful branching reward for genuine engagement.

**Nodes visited**: START → A1_OPEN → A1_D1 → A1_Q_AGENCY_HIGH → A1_D2_HIGH → A1_Q_CHOICE_INT → A1_D3 → A1_R_INT → BRIDGE_1_2 → A2_OPEN → A2_D1 → A2_Q_CONTRIB → A2_D2_C → A2_R_CONTRIB → BRIDGE_2_3 → A3_OPEN → A3_D1 → A3_Q_ALTO → A3_D2_A → A3_Q_MEANING → A3_D3 → A3_R_ALTO → SUMMARY → END
