# Forms Reference — UX Movement Corpus

## Label Patterns

**Top-aligned labels** (preferred default):
- Best for accessibility; screen readers always find them
- Labels above fields are easier to scan when filling out
- Use when form length is a concern

**Floating labels**:
- Label lives inside field, floats above on focus/input
- Saves vertical space vs top-aligned
- "8 Rules for Switching to Infield Top-Aligned Form Labels" covers when to use
- Don't use if you also need persistent hint text (floating label competes with hint)

**Infield placeholder-only** (anti-pattern):
- Label disappears on input → user forgets what field they're in
- Fails WCAG 1.3.5 (identify purpose) for assistive tech
- Never use placeholder as the only label

## Required vs Optional Fields

- Mark optional fields with "(Optional)" text, not asterisks
- Asterisks on required fields increase form anxiety; they signal the form is demanding
- The goal is reducing perceived effort, not flagging demands
- If a field is truly optional, ask: can you remove it entirely?
- "Stop Putting Asterisks on Required Fields" — anti-asterisk argument
- "Optional Fields You Should Remove On Your Form" — when to cut fields
- "Required Data Fields That Shouldn't Be Required" — which common fields are over-required

## Input Splitting (Anti-Patterns)

- Never split first name / last name → one "Full Name" field is faster and culturally flexible
- Never split email + confirm email → use live validation with a checkmark instead
- Never split phone into area code + number → one masked field is faster
- "Why You Should Never Split First and Last Name Fields"
- "Why Confirm Password Is the Slowest Field to Fill Out" — apply same logic to email confirm

## Selection Controls

**Checkboxes**:
- Add full-row click target (padding around label)
- Group related checkboxes with a visible group label
- Use chips when you have ≤8 options and space allows
- "10 Usability Mistakes Most Designers Make on Checkboxes"

**Radio buttons**:
- Always add border + surface around each option
- The border creates whitespace between options (readability)
- The surface makes the entire row the click target
- Use highlight border for selected state (not just filled circle)
- "Why Radio Buttons Should Always Have Borders"

**Select menus (dropdowns)**:
- Anti-pattern for small option sets (≤10): replace with chips
- Anti-pattern for large option sets (>50): use an autocomplete/searchable field
- "1 Select Field vs 12 Select Chips" — chips vs dropdown comparison
- "Stop Using Listboxes for Multiselecting Items"

**Chips / Select Chips**:
- Best for ≤10 options where all are visible at once
- Reduce interaction from 3 clicks to 1
- Can be used inline within form fields or as standalone option groups
- "Lower Cognitive Load on Forms with Input Chips"
- "Why Chips Should Replace Checkboxes and Radio Buttons"

## Date & Time Fields

**Date input mask** (recommended):
- Single field with MM/DD/YYYY mask
- Auto-advances cursor from MM → DD → YYYY
- Format hint is always visible (not placeholder that disappears)
- Faster than free-text; more accessible than 3 separate fields

**What to avoid**:
- 3 separate fields (month/day/year) — extra clicks, unclear error placement
- 3 select menus — 9+ interactions for one date
- Unconstrained text field — parsing inconsistency

**Calendar picker**:
- Use alongside mask for "schedule in near future" use cases
- Calendar icon right-aligned in field opens picker on click
- "The Best UX Pattern for Date Fields on Forms"
- "The Best Mobile UI for Picking Date and Time"

## Validation

**When to validate**:
- Best: validate on blur (when user leaves the field)
- Avoid: validate on keypress (too aggressive, feels like being watched)
- Never: validate only on submit (user has to scroll back to find errors)
- "A Better Form Field Validation Than OnBlur" — real-time + blur hybrid approach

**Error message style**:
- Inline, next to the field (not summary at top)
- Positive voice: "Enter a valid email" not "Invalid email"
- Tell them what to do, not just what's wrong
- "How to Write User-Friendly Error Messages"

**Sibling fields**:
- When two fields are interdependent (start/end date), validate their relationship
- "Sibling Fields: Better Input Validation for Related Data"

## Long Forms

**Multi-page vs single-page**:
- Single page: short forms (≤5 fields), simple data, same cognitive context
- Multi-page: long forms (>8 fields), unrelated field groups, complex decisions
- "Single-Page vs. Multi-Page Forms: When to Use Which"

**Conversational / question format**:
- Display one question per page/screen
- Works well for onboarding, qualification flows, surveys
- More empathetic tone, feels less like interrogation
- "Why Long Page Forms Need to Be Conversational"
- "Why a Mad Libs Form Gets You More Leads"

**Making long forms look shorter**:
- Group fields under clear section headings
- Collapse optional sections behind toggle switches
- Show progress bar for multi-page
- "How to Make a Long Mobile Form Look Shorter"
- "How to Simplify 6 Optional Fields with Toggle Switches"

## Signup & Login

- Signup and login should be the same form (auto-detect account existence)
- Don't open in a new page — use a modal drawer
- Remember Me should default to ON
- "Why Sign-Up and Login Should Be the Same Form"
- "Why Signups & Logins Should Open in a Modal Drawer"
- "Why Remember Me on Logins Should Be the Default"

## Onboarding Flows (replacing signup forms)

Structure:
1. Goal/focus question first (builds trust, personalizes)
2. Identity fields (name, email) — less friction after goal question
3. Role + company (chips, not dropdowns)
4. Username with live preview
5. Confirmation + workspace ready screen

Key rules:
- Always show progress indicator with step count
- Use empathetic, second-person copy ("We'll set up your workspace based on this")
- Remove all optional fields
- End with a reward (confirmation + direct path to app)
- "Why Onboarding Flow Is the New Signup Form"

## Accessibility

- All fields need programmatic labels (not just visual)
- Placeholder text ≠ label
- Error messages need `role="alert"` or `aria-live`
- Form groups need `<fieldset>` + `<legend>`
- "The Ultimate Guide to Signup Form Accessibility"
- "How to Make Form Fields Accessible with Proper Contrast"
