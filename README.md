# The Daily Reflection Tree

A deterministic end-of-day reflection tool. No LLM at runtime — the intelligence is in the structure.

## Structure

```
/tree/
  reflection-tree.json     ← the full tree (42 nodes)
/agent/
  index.html               ← runnable web agent (single file, no dependencies)
/transcripts/
  persona-1-external-entitled-selfcentric.md
  persona-2-internal-contributing-altrocentric.md
write-up.md                ← design rationale
README.md
```

## Running the agent

Open `agent/index.html` in any browser. No server required.

The agent loads the tree data embedded in the HTML (for portability), walks it deterministically, and produces a reflection summary without any API calls.

## Reading the tree

`tree/reflection-tree.json` is the canonical data file. Any developer can load it and build a different agent from the same structure. Key fields:

| Field | Purpose |
|-------|---------|
| `id` | Unique node identifier |
| `parentId` | Parent node (builds hierarchy) |
| `type` | `start`, `question`, `decision`, `reflection`, `bridge`, `summary`, `end` |
| `text` | What the employee sees. `{NODE_ID.answer}` interpolates earlier answers |
| `options` | For questions: array of chooseable strings. For decisions: routing rules |
| `target` | Override next-node (for bridges/reflections that jump across subtrees) |
| `signal` | What this node records: `axis1:internal`, `axis2:contribution`, etc. |

Decision node routing syntax:

```
answer=Option A|Option B:NodeX;answer=Option C:NodeY
```

Reads: "If prior answer was 'Option A' or 'Option B', go to NodeX. If it was 'Option C', go to NodeY."

## Tree statistics

- Total nodes: 42
- Question nodes: 13
- Decision nodes: 11
- Reflection nodes: 9 (3+ per axis)
- Bridge nodes: 2
- Summary node: 1
- Start/End: 2
- Options per question: 4
- Possible conversation paths: 16 distinct paths to summary
- All 3 axes covered in sequence

## Axes

1. **Locus** — Victim ↔ Victor (Rotter 1954, Dweck 2006)
2. **Orientation** — Entitlement ↔ Contribution (Campbell 2004, Organ 1988)
3. **Radius** — Self-centric ↔ Altrocentric (Maslow 1969, Batson 2011)

## Summary logic

At the end of the session, the tree tallies signals accumulated across all nodes and picks the dominant pole per axis. The 8 possible combinations (`internal/external × contribution/entitlement × altrocentric/selfcentric`) each map to a distinct closing reflection in `summaryTemplates.closingReflections`.
