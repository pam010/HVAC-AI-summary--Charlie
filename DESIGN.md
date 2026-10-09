# DESIGN.md

## Visual direction

**Working title:** Recovery Operations Log

The site should feel like an incident-review runbook used by a small operations team: precise, calm, traceable, and built for returning to the same decision months later. It is not a promotional landing page and not a conventional personal blog.

## Core visual system

- **Canvas:** deep blue-black operational background with a subtle grid and sparse routing lines.
- **Primary surface:** warm off-white log sheets that carry the long-form reading experience.
- **Signals:** HVAC cyan for system/data, safety amber for decisions and attention, restrained green for confirmed states, muted red only for risks.
- **Typography:** a sturdy sans-serif for reading; a compact mono face for dates, statuses, field names, and small operational labels.
- **Geometry:** squared sheets with clipped or stepped corners; thin rules and registration marks rather than rounded floating cards.
- **Density:** compact at the overview level, comfortable in long-form body text.

## First viewport contract

The visitor must immediately understand:

1. What was decided: recover short AI calls with a 30-second SMS path.
2. What counts as success: a successfully handed-off request.
3. Where the work stands: architecture agreed, MVP build next.
4. What happens next: build and test the trigger-to-handoff path in GHL.

The hero should therefore behave like an incident header, with one dominant title, a status strip, a compact decision statement, and an architectural signal flow.

## Information architecture

### Home

- Journal identity and short purpose statement.
- Current system status and primary next action.
- Latest entry presented as a dated log event.
- Compact roadmap and definition of success.
- Link to the reusable entry template and repository documentation.

### Entry

1. Header and executive decision.
2. Why this problem matters.
3. Discussion trail: concern → challenge → refined decision.
4. MVP flow.
5. Form and data model.
6. Owner handoff and integration paths.
7. Scope boundary and KPI definition.
8. Risks and validations.
9. Tools and official references.
10. Immediate action plus the following three steps.

## Interaction rules

- Persistent but quiet return/navigation link on entry pages.
- Expandable implementation details may use native `details` elements.
- Links and controls must have visible keyboard focus.
- Motion is limited to short reveal and hover transitions and must respect reduced-motion settings.
- No carousel, no decorative chart, and no animation that delays reading.

## Responsive behavior

- Wide screens: narrow navigation rail paired with a broad reading sheet.
- Small screens: single column, sticky compact header, architecture flow becomes vertical.
- Tables transform into stacked labeled rows when necessary.
- Minimum body text size remains 16px on mobile.

## Reuse rules

- Every entry reuses the same semantic sections and status vocabulary.
- Statuses: `CONFIRMED`, `TO VALIDATE`, `NEXT`, `RISK`, `REFERENCE`.
- Each entry ends with one immediate action and exactly three continuation steps.
- Future visual additions must reinforce traceability, not add decoration for its own sake.
