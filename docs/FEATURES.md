# Features

This document describes Axiom's core product behavior and experience logic.
It focuses on system promises rather than implementation details.

## Experience modes

In Axiom, people don't choose a car — they choose an experience mode.

> _How do I want this trip to feel?_

Experience modes define the interior, behavior, and rules of a journey.
They are modes of mobility, not vehicle models.

Each mode:
- Makes a clear promise
- Influences pricing logic
- Affects vehicle visuals and configuration

Axiom supports five experience modes.

### Focus

Calm environment for concentration and discreet communication.

Characteristics:
- Work-friendly surfaces
- Reduced noise and non-essential activity
- Visual and acoustic shielding from outside and other passengers

### Family

Flexible space for shared moments and stress-free arrivals.

Characteristics:
- Flexible seating and storage that adapts to people and bags
- Easy entry and exit
- Forgiving timing for stops, delays, and real-life interruptions

### Solo

Efficient, personal mobility with minimal overhead.

Characteristics:
- Compact interior optimized for single occupancy
- High availability and short wait times
- Routing and speed tuned for minimal energy consumption

### Private

Privacy and control, without compromise.

Characteristics:
- Maximum privacy and safety
- Priority routing when conditions allow
- Preferred lanes and premium access where available

### Shared

Lower cost through aligned intent, not randomness.

Characteristics:
- Reduced cost compared to other modes
- Co-travelers with compatible destinations
- Clear expectations around behavior and shared space

## Pricing model

Axiom uses experience-based pricing instead of vehicle-based pricing.

### Core pricing factors
- Duration
- Time of day
- Urgency (now vs planned)

Planning ahead reduces cost by:
- Improving AI fleet allocation efficiency
- Reducing peak energy usage of autonomous systems and servers

### Autonomy confidence

Traditional insurance is replaced by autonomy confidence.

- Fully autonomous conditions → lower cost
- Human oversight required → slightly higher cost
- Extreme or uncertain conditions → premium pricing

### Trust level

Pricing also reflects the system's confidence in the user profile.

- Trusted profiles → lower cost
- New or unknown profiles → small safety margin

## User profile

Axiom is guest-first by default.

- Users can proceed without creating an account
- The system generates a friendly alias (e.g. `SkyRider2049`)
- Profiles can be renamed at any time

Renaming a profile transitions its status:
- Recognized → Trusted
- Removes the safety margin
- Slightly lowers pricing