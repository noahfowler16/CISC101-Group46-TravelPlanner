Change Log (2025-11-17):
- Added short-walk rule: if user prefers “short walks only,” limit activities to <15 minutes walking distance.

# Module 3 — Feasibility & Guardrails

## Purpose
Apply realistic checks and adapt the plan when needed.

## Internal Checks (If/Else Rules)

### Closed Venue
If attraction is closed → choose similar indoor option nearby.

### Over-Budget Meal
If restaurant too expensive → replace with cheaper similar cuisine.

### Too Far or Long Travel
If distance >25 min or >5 km → choose nearer option or add transit.

### Short Walks Preference
If user indicates “short walks only” → choose activities within 15-minute walking distance and prioritize clustered locations.

### Weather Swap
If rainy or cold season likely → include at least one indoor alternative.

### Time Overrun
If total time > available hours → shorten lunch or choose closer activity.

### Mobility Needs
If mobility limits → short walks, step-free routes, breaks.

### Dietary Needs
If vegan or other constraints → ensure all meals comply.

### Bookings
If reservations typically needed → remind user only; never simulate.
