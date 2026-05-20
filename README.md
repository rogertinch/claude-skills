# Claude Skills

Domain-expert skills for [Claude Code](https://claude.ai/code). Each skill loads a focused knowledge base from a specific expert corpus into Claude.

## Skills

### UX Movement Design

A UX design advisor based on Anthony Hobday's framework from UX Movement (319 articles, 2020–2026). Diagnoses UI problems and prescribes specific design patterns. Use for pattern guidance on concrete questions; use Laws of UX Design when you want a formal audit against named principles.

**Triggers on:** form design, navigation, tables, buttons, color, typography, modals, mobile UX, visual hierarchy, accessibility, onboarding, and any "should I use X or Y" or "how should I design X" question.

**Reference material:** `ux-movement-design/references/` — principle summaries for forms, navigation, tables, layout, and components.

**Invoke:** `/ux-movement-design`

---

### Lang Game Design

A tabletop game design consultant built around Eric M. Lang's 28 design tenets. Lang designed *Blood Rage*, *Rising Sun*, *Chaos in the Old World*, *A Game of Thrones CCG*, and 100+ titles. Applies his philosophy to diagnose structural problems and recommend directions.

**Triggers on:** faction design, victory conditions, resource systems, card/ability design, asymmetric balance, complexity budgeting, deckbuilding constraints, and any "what do you think about X mechanic" question.

**Reference material:** `lang-game-design/references/tenets.md` — full quotes and explanations for all 28 tenets.

**Invoke:** `/lang-game-design`

---

### Laws of UX Design

A UX auditor based on all 30 Laws of UX (lawsofux.com). Checks designs against specific laws, surfaces violations with severity ratings, and gives fixes rather than generic advice. Where `ux-movement-design` prescribes patterns, this one audits against named laws.

**Triggers on:** UI screenshots, wireframes, design descriptions, code for UX review, and any question like "what UX laws does this violate?", "is this good UX?", "review my design", or "how can I improve this interface?" Also works for navigation menus, forms, onboarding flows, dashboards, and checkout flows.

**Reference material:** `laws-of-ux-design/references/` — `laws-summary.md` (all 30 laws with taglines and takeaways) and `laws-of-ux.json` (full data, origins, further reading, related laws).

**Invoke:** `/laws-of-ux-design`

---

### Writing Well

A nonfiction prose editor based on William Zinsser's *On Writing Well*. Revises existing drafts or writes from a brief: cuts clutter, strengthens verbs, fixes weak leads and soft endings, enforces unity of pronoun, tense, and mood. Not for fiction, poetry, marketing copy, UI text, or removing AI writing patterns.

**Triggers on:** essays, articles, blog posts, op-eds, criticism, memoir, business writing, science/tech explainers, longform reporting, personal essays — any nonfiction meant for a real reader.

**Reference material:** none; skill is self-contained in `writing-well/SKILL.md`.

**Invoke:** `/writing-well`

---

## Structure

Each skill follows the same layout:

```
<skill-name>/
  SKILL.md          # Skill definition: trigger description + system prompt
  evals/
    evals.json      # Evaluation cases for the skill
  references/       # Optional — domain reference material (markdown or JSON) loaded on demand
    *
```

## License

MIT
