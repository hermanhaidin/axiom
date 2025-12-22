# Technical overview

This document defines the technical scope and constraints of Axiom.
It is not a setup guide and not a production specification.

### Project type

Axiom is a conceptual, front-end–focused demo project.
It explores how a future mobility platform could behave and feel, rather than how such a system would operate at scale.

As such:
- No backend services
- No real-time fleet integration
- No production authentication or identity system

### Intended technology stack

Axiom is intended to be built with a modern, React-based frontend stack:

- React
- TypeScript
- shadcn/ui
- Tailwind CSS

The stack is intentionally frontend-focused to support rapid iteration and speculative exploration.

### Data and persistence

Axiom assumes a local-first approach by default:

- Bookings and user state are stored locally on the user's device
- No server-side persistence is required
- Data can be cleared or reset at any time

### Theming and appearance

Axiom supports light and dark appearance modes.

- By default, the application follows the user's system appearance
- An explicit appearance control allows switching between light and dark modes
- User-selected appearance overrides the system setting and is stored locally

Experience modes do not introduce separate visual themes.

### Experience modes and system behavior

Experience modes influence system behavior rather than vehicle identity or application structure.

They may affect:
- Interior configuration
- Routing and prioritization logic
- Pricing and availability rules

They do not imply separate applications or architectures.

### Constraints and non-goals

Clarity of intent is prioritized over technical completeness.

Axiom does not aim to:
- Simulate real-world autonomous driving
- Model accurate routing, traffic, or pricing algorithms
- Act as a production-ready mobility platform
- Provide backend APIs or integrations