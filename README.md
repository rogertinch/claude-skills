# claude-skills

A collection of domain-expert skills for [Claude Code](https://claude.ai/code). Each skill loads a specialized knowledge base and reasoning framework into Claude, grounding its answers in a specific expert corpus rather than general training data.

## Skills

### `ux-movement-design`

A UX design advisor powered by the full UX Movement corpus — 319 articles by Anthony Hobday (2020–2026). Applies his research-backed framework to diagnose UI problems and prescribe specific design patterns.

**Triggers on:** form design, navigation, tables, buttons, color, typography, modals, mobile UX, visual hierarchy, accessibility, onboarding, and any "should I use X or Y" design question.

**Reference material:** `ux-movement-design/references/` — curated principle summaries for forms, navigation, tables, layout, and components.

---

### `lang-game-design`

A tabletop game design consultant built around Eric M. Lang's 28 design tenets. Lang designed *Blood Rage*, *Rising Sun*, *Chaos in the Old World*, *A Game of Thrones CCG*, and 100+ titles. The skill applies his philosophy to diagnose structural design problems and recommend concrete directions.

**Triggers on:** faction design, victory conditions, resource systems, card/ability design, asymmetric balance, complexity budgeting, deckbuilding constraints, and any "what do you think about X mechanic" question.

**Reference material:** `lang-game-design/references/tenets.md` — full quotes and explanations for all 28 tenets.

---

## Structure

Each skill follows the same layout:

```
<skill-name>/
  SKILL.md          # Skill definition: trigger description + system prompt
  evals/
    evals.json      # Evaluation cases for the skill
  references/
    *.md            # Domain reference material loaded on demand
```

## License

MIT
