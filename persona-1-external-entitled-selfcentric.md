# Transcript: Persona 1 — External / Entitled / Self-Centric

**Profile**: Senior analyst. Long day. A key presentation was rescheduled last-minute, a colleague got credit for her work, and a technical issue blocked her deliverable. She arrives at this tool tired and frustrated.

---

**[START]**
> Good evening. Let's take five minutes to look at your day — not to judge it, just to see it clearly.

*[Employee clicks Begin →]*

---

**[A1_OPEN]** Axis I — Locus
> If today had a weather forecast, what would it be?

**Selected**: *"Stormy — things felt out of control"*

*→ Routed to: A1_Q_AGENCY_LOW (external locus branch)*

---

**[A1_Q_AGENCY_LOW]** Axis I — Locus
> You described today as "Stormy — things felt out of control". When things got hard, what did you do first?

**Selected**: *"Got frustrated with the situation"*

*→ Signal recorded: axis1:external*
*→ Routed to: A1_D2_LOW → A1_Q_CHOICE_EXT*

---

**[A1_Q_CHOICE_EXT]** Axis I — Locus
> Think of one specific moment today that didn't go to plan. Looking back, was there anything in your control?

**Selected**: *"Not really — external factors drove it"*

*→ Routed to: A1_D3B → A1_R_EXT*

---

**[A1_R_EXT]** Reflection
> Tough days pull attention outward — to what others did, to what went wrong, to what wasn't in your hands. That's real. But somewhere in there, even small, you made a call. Tomorrow, see if you can catch it while it's happening.

*→ Signal recorded: axis1:external*
*→ Auto-advances to BRIDGE_1_2*

---

**[BRIDGE_1_2]** Bridge
> Now let's shift from how you handled today — to what you gave.

*→ Auto-advances to A2_OPEN*

---

**[A2_OPEN]** Axis II — Orientation
> Think of someone you interacted with today — a colleague, a teammate, anyone. Which of these felt most true?

**Selected**: *"I felt like I gave more than I received"*

*→ Routed to: A2_D1 → A2_Q_ENTITLE (entitlement branch)*

---

**[A2_Q_ENTITLE]** Axis II — Orientation
> When you think about recognition today — credit for work done, appreciation from others — how did it feel?

**Selected**: *"I felt others got credit that should have been shared"*

*→ Signal recorded: axis2:entitlement*
*→ Routed to: A2_D2_E → A2_R_ENTITLE*

---

**[A2_R_ENTITLE]** Reflection
> When we focus on what we deserve — recognition, fairness, credit — it's usually because something real feels unacknowledged. That matters. And: the question worth sitting with is whether your energy today was mostly pointed outward or inward.

*→ Signal recorded: axis2:entitlement*
*→ Auto-advances to BRIDGE_2_3*

---

**[BRIDGE_2_3]** Bridge
> Last shift. From what you gave — to who you were thinking about when you gave it.

*→ Auto-advances to A3_OPEN*

---

**[A3_OPEN]** Axis III — Radius
> When you think about today's biggest challenge, whose experience comes to mind first?

**Selected**: *"Mine — it was my problem to navigate"*

*→ Routed to: A3_D1 → A3_Q_SELF (self-centric branch)*

---

**[A3_Q_SELF]** Axis III — Radius
> That makes sense — your own experience is real and immediate. At any point today, did you catch yourself wondering how someone else was doing?

**Selected**: *"Not really — I was in survival mode"*

*→ Signal recorded: axis3:selfcentric*
*→ Routed to: A3_D2_S → A3_R_SELF*

---

**[A3_R_SELF]** Reflection
> Today was about getting through. That's valid — some days require all of your attention just to survive them. Tomorrow, try to find one moment where you look up and notice someone else in the room. Not to help them. Just to see them.

*→ Signal recorded: axis3:selfcentric*
*→ Auto-advances to SUMMARY*

---

**[SUMMARY]**

**Axis state at summary:**
- axis1: internal=0, external=2 → dominant: **external**
- axis2: contribution=0, entitlement=2 → dominant: **entitlement**
- axis3: altrocentric=0, selfcentric=2 → dominant: **selfcentric**

**Summary key**: `external+entitlement+selfcentric`

> **Today's reflection**
>
> Here's what today looked like.
>
> **Axis I · Locus** — You felt pulled by circumstances
> **Axis II · Orientation** — You were paying attention to what you received
> **Axis III · Radius** — You were focused on your own lane
>
> *A difficult day, and you felt it in every direction. That's real. Rest. Tomorrow, try one thing: find one moment you could choose differently, and take it.*

---

**[END]**
> See you tomorrow.

---

## Path analysis

The tree routed this persona through the lowest-agency, most entitlement-oriented, most self-focused branches consistently. The reflections acknowledged the difficulty without moralizing ("That's valid", "That's real"), and the closing summary offered a single, concrete, actionable nudge — not a lecture. The tone is a wise colleague, not a manager.

**Nodes visited**: START → A1_OPEN → A1_D1 → A1_Q_AGENCY_LOW → A1_D2_LOW → A1_Q_CHOICE_EXT → A1_D3B → A1_R_EXT → BRIDGE_1_2 → A2_OPEN → A2_D1 → A2_Q_ENTITLE → A2_D2_E → A2_R_ENTITLE → BRIDGE_2_3 → A3_OPEN → A3_D1 → A3_Q_SELF → A3_D2_S → A3_R_SELF → SUMMARY → END
