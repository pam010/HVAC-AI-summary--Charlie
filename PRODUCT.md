# PRODUCT.md

## Product definition

**Name:** HVAC AI Build Journal

**Purpose:** A public, evolving build journal for an agency developing an HVAC inbound-call recovery system in GoHighLevel. It records why decisions were made, what is already confirmed, what still needs validation, and the exact next actions.

**Primary mechanism:** Convert short or abandoned AI receptionist calls into traceable service requests through a timed SMS, a compact recovery form, CRM ownership, and reliable notification delivery.

## Audience

- The agency founder, returning later to understand prior decisions and continue execution.
- Future collaborators who need the operating logic without reading the original conversation.
- Prospective HVAC clients who may review the reasoning, scope, and proof behind the service.

## First release goal

Publish one complete entry for 2026-10-09 and establish a reusable journal structure for future entries.

The first entry must document:

- The short-call recovery problem and the proposed 30-second rescue flow.
- Confirmed MVP scope and explicit non-goals.
- The minimal homeowner form and CRM data model.
- Owner handoff and integration options.
- The definition of a successfully handed-off request.
- Required tools, implementation steps, risks, validation plan, and immediate next action.

## Product truth and scope

### Confirmed outcome

The agency is responsible for producing a **Successfully Handed-Off Request**, not a qualified lead or completed booking.

A request counts as successfully handed off when:

1. The call meets the short-call recovery condition.
2. The homeowner submits the recovery form.
3. A service-request record is created in the CRM.
4. A primary owner is assigned.
5. At least one notification channel is successfully delivered.

Downstream outcomes—owner acknowledgment, callback, qualification, booking, won job, and revenue—are optional metrics used to evaluate ROI, not the agency's core delivery promise.

### MVP boundaries

- GoHighLevel is the source of truth for the first 5–10 clients.
- Do not add Supabase until cross-account analytics, a custom portal, advanced media processing, or portability makes it necessary.
- The recovery form collects enough information for a credible callback, not enough for full dispatch.
- Photos are optional supporting evidence.
- The workflow must not promise an immediate human response or a confirmed appointment.
- Existing field-service platforms remain the client's operational system when present.

## Experience requirements

### Journal experience

- Read-first, calm, operational, and highly scannable.
- The first viewport must immediately show the decision, current status, scope boundary, and next action.
- Avoid a generic marketing-site appearance and avoid collections of interchangeable cards.
- Desktop and mobile layouts must both be complete and legible.
- Each future entry should follow the same sequence: context, decision trail, architecture, scope, risks, evidence, and next actions.

### Recovery experience described by the journal

- Trigger: short inbound call, approximately 15 seconds or less, with no valid service need captured.
- Wait: 30 seconds after hangup.
- Action: one concise SMS with one primary link and required opt-out language.
- Form: issue, ZIP, optional photos, editable callback phone, optional callback time.
- Response: immediate acknowledgment and a credible callback window.
- Handoff: assign a primary owner, maintain a backup owner, create a task/request, and notify through configured channels.

## Content and language

- Primary language: Traditional Chinese with necessary English product terms preserved.
- Tone: practical, analytical, transparent about uncertainty, and free of inflated claims.
- Dates use ISO format: YYYY-MM-DD.
- External sources must link to official documentation whenever possible.

## Technical constraints

- Static HTML, CSS, and minimal JavaScript only.
- No build step or paid dependency.
- GitHub Pages compatible from the repository root.
- Relative internal links.
- Semantic HTML and accessible contrast/focus states.
- Repository includes a README and a reusable entry template.

## Success criteria for this delivery

- Public GitHub repository named `hvac-ai-build-journal`.
- GitHub Pages site is accessible.
- The 2026-10-09 entry accurately captures the agreed discussion and actionable next steps.
- A future entry can be added without redesigning the site.
