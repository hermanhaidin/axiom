# Technical Overview

This document defines the technical scope and constraints of Axiom.

For the design vision, see [VISION.md](VISION.md).

---

## Project type

Axiom is a conceptual, front-end–focused demo. It explores how a future mobility platform could behave and feel, not how such a system would operate at scale.

As such:
- No backend services or real-time fleet integration
- No production authentication or identity system
- Mocked data and responses throughout

---

## Technology stack

Axiom is built with a modern React-based frontend stack:

- React
- TypeScript
- shadcn/ui
- Tailwind CSS

The stack is intentionally frontend-focused to support rapid iteration and speculative exploration.

---

## Implementation approach

The demo follows a mock-first pattern:

1. **Home page** — Single input field for natural language intent
2. **API route** — Returns mocked `TripPlan` JSON (hardcoded responses)
3. **Trip plan component** — Renders structured understanding, options, and confirmation flow

Once the UI feels right, the mock can be swapped for a real model call. Only the prompt and response parsing need to change—the UI remains stable.

### Data shape (TripPlan)

The API route returns a `TripPlan` object containing:

- Structured understanding (trip type, party, constraints, inferred mode)
- Clarifying question (optional, one at a time)
- Movement story options (2–4), each with:
  - Title and description
  - Price range
  - Composition details
  - Interior preview reference
  - "Why this fits" rationale

Exact schema to be defined during implementation.

---

## Data and persistence

Axiom uses a local-first approach:

- Bookings and user state stored in browser (localStorage or similar)
- No server-side persistence required
- Data can be cleared or reset at any time

### User profile

- Default: Guest with generated alias (e.g., `SkyRider2049`) and "Recognized" trust level
- Upgrade: User provides name → "Trusted" level, slightly reduced pricing
- Profile stored locally, not synced

---

## Theming and appearance

Axiom supports light and dark modes.

- Default: Follows system appearance
- Override: Manual toggle, preference stored locally
- Experience modes do not introduce separate visual themes

---

## Constraints and non-goals

Clarity of intent is prioritized over technical completeness.

Axiom does not aim to:
- Simulate real-world autonomous driving or routing
- Model accurate traffic or pricing algorithms
- Act as a production-ready mobility platform
- Provide backend APIs or external integrations
