# UI Components Reference — UX Movement Corpus

## Buttons

### Button Color
- **Don't use your brand/primary color for CTAs**: The primary color establishes identity (30% of UI). CTAs should use the accent color (10%), which is specifically reserved for directing user action.
- **Bright colors fail accessibility**: High-saturation accent colors often fail WCAG 4.5:1 with white text. Test contrast.
- **Delete buttons should NOT be red**: Red increases motor output (users click faster) and reduces self-control. Use a neutral (black/dark) button with a red warning icon in the dialog header instead.
- "Why You Shouldn't Use Your Brand Color on Buttons"
- "Why Bright Button Colors Fail Accessibility"
- "Why Delete Buttons Should Not Be Red"
- "How to Fix Ugly Interfaces with Better Brand Colors"

### Button States & De-Emphasis
- Use filled > outlined > ghost hierarchy for primary > secondary > tertiary
- Law of De-Emphasis: secondary actions should be less visually prominent
- Avoid giving two competing actions equal visual weight
- "The Law of De-Emphasis for Clean UI Design"
- "How to Make Similar Button Choices Less Confusing"
- "How to Make Similar Buttons Easier to Choose"

### Toggle Buttons
- **Never make active state look like a button**: Selected state ≠ button affordance
- Use color + surface fill + text change to signal selected vs unselected
- Don't use inverted colors (light text on dark) to signal active — it looks like a button you can click again
- "Don't Use Inverted Color Cues on Toggle Buttons"
- "How to Fix the Worst Toggle Button Design Mistakes"
- "How to Signify Toggle Button States Without Color"
- "Google's Big Toggle Button Design Mistake"

### Button Size & Corners
- Minimum touch target: 44×44px
- Max border-radius: avoid full pill shape for primary action buttons (it can signal non-clickable decoration)
- "Why Your Buttons Should Have a Max Border-Radius"
- "How to Optimize Buttons for Task Performance"

### Action Buttons in Tables
- "How to Fit 8 Action Buttons in a Table Row" — icon buttons with tooltips in row actions
- "How to Make Technical Button Actions More Predictable"

### Dangerous Actions
- "How to Make Dangerous Delete Buttons Safer to Click"
- Confirmation dialogs for destructive actions
- Consider requiring the user to type a confirmation string for permanent deletions

## Modals & Dialogs

### When to use modals
- Use for tasks that genuinely require focus isolation
- Don't use for viewing supplementary data users need to compare with the main view
- Don't use for editing inline data (use inline cards instead)

### Modal anatomy
- Header: title + close button (X)
- Body: content (scrollable if needed)
- Footer: primary action (right) + secondary/cancel (left)
- "Anatomy of an Optimally Designed Modal"
- "The Right Way to Design a Modal Confirmation Dialog"

### 4 Modal States
1. Default (form/content visible)
2. Loading (after submit: disable button, show spinner, prevent close)
3. Success (show success message/animation)
4. Error (show error, re-enable submit)
- "Why Modal Dialogs Should Have 4 States"

### Mobile modals
- Use bottom sheets instead of centered dialogs on mobile
- "The Optimal Way to Display Modals on Mobile Screens"

### Modal slideouts (drawers)
- Right-side slideout for detail views and complex forms
- Preserves context (list/page visible behind)
- "Modal Slideouts: The Cure to Back Button Fatigue"
- "Modal Slideouts vs Popups: The Right Choice for Better UX"
- "Why Users View Details Better with Slideovers"

### Confirmation dialogs
- Use for destructive actions
- Red warning icon in header, neutral-colored confirm button (not red)
- Include descriptive warning text about consequences
- Don't offer a Cancel button if closing the dialog is sufficient
- "The Right Way to Design a Modal Confirmation Dialog"
- "When You Should Cancel the Cancel Button"

### Nested modals
- Anti-pattern; causes back-button fatigue
- Flatten into: step-by-step flow, inline cards, or expandable sections
- "How to Simplify 4 Nested Modals into Only 1"

### Inline cards (alternative to modals)
- For editing in-context data: card transitions to edit state in place
- For viewing supplementary info: expand inline below the card
- Preserves spatial context, reduces working memory load
- "Inline Cards: Better Data Display Without Modals"

## Alerts, Toasts & Notifications

### Alert types
- 4 types: info (blue), success (green), warning (yellow), error (red)
- Each has icon + title + message + optional action
- "The 3 Types of UI Alerts and How to Use Them"
- "The 4 Tones of Alert Messages and Notifications"
- "The Proper UI Anatomy for Alert Components"

### Toasts
- Use for brief, non-blocking feedback after user actions
- Position: bottom-center or top-right (not top-center)
- Auto-dismiss after 3–5 seconds for info/success; keep visible for errors
- Don't use toasts as the only feedback for button clicks — also use inline state change
- "Why Toasts Aren't the Best for Button Feedback"
- "Best Practices to Make Your Toasts Usable and Accessible"

### Notifications menu
- "How to Design the Most User-Friendly Notifications Menu"
- Group by time (today, this week, older)
- Mark read/unread clearly

### Button feedback
- Show state change inside the button itself (loading spinner, checkmark)
- "How to Give Visual Feedback After Users Click a Button"
- "How to Speak to Users After They Perform an Action"

## Tooltips

- Show on hover (desktop) and long-press (mobile)
- Dark background tooltip is easier to read (light mode or dark mode)
- Use tooltips for icon-only buttons without labels
- "Why You Should Display Your Tooltips in Dark Mode"
- "Help Text vs Tooltips: Which Is Better for Forms" — tooltips for contextual hints, help text for persistent guidance

## Carousels

- Show partial next item to signal swipability
- Don't rely on dots alone as indicators
- "The Myth of Low Engagement Carousels"
- "Why Dots Are Terrible Indicators for Carousels"
- "Clear Visual Cues for the Perfect Mobile Carousel"
- "Collection Carousel: A Mobile Pattern to End Swipe Errors"

## Icons

- Universal icons (home, search, settings, user, close, etc.) can go label-free
- Non-universal icons need tooltips or labels
- Don't use saturated colors on icons
- Match icon style (outlined vs filled) consistently throughout
- "Best vs Worst Practices for Interface Icons"
- "The 16 Universal Icons to Use on All Interfaces"
- "Why Saturated Colors Are Terrible for Your Icons"
- "UI Design Tips for Better Looking Icons"
- "Which Icon Style Is Most Efficient for Scanning"

## File Uploaders

- Show drag-and-drop zone, not just a button
- Preview uploaded files before submit
- Show file name, size, and remove option
- "Clear Visual Cues for the Perfect File Uploader"
- "Why Your File Uploader Needs a Drag-and-Drop Zone"

## Drag & Drop

- Show visual affordance before interaction (dashed border, "drag here" hint)
- Show active drag state (highlight drop zone, ghost element following cursor)
- "Visual Cues to Help Users Perceive Drag-and-Drop"

## Thank You Pages

- Confirm the action taken
- Tell them what happens next
- Offer a next step (CTA)
- Don't leave users stranded
- "Everything Users Need to See on a Thank You Page"

## Onboarding Patterns

- Lead with value, not data collection
- Use progress indicator
- "Onboarding Patterns to Kickstart Your User Experience"
- "Redesign of a Failed Mobile Onboarding Flow"
- "Why It's Bad to Explain Features on Your Onboarding Screen" — show, don't tell

## Search

- Autocomplete with imagery improves recognition and click confidence
- Show recent searches on focus
- Show results count
- "How to Design a Smart Search Bar Experience"
- "A Faster Way to View Search Results with Fewer Clicks"
- "Why Your Autocomplete Search Field Should Include Imagery"

## Landing Pages

- "The Optimal Design for a Landing Page Hero" — hero structure
- "How to Design the Best Landing Page for Products"
- "The Design Process for Creating a New Ecommerce Feature"
