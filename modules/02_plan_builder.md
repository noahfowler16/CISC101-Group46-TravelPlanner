# Module 2 — Plan Builder (Options → Days)

## Purpose
Generate activity options and assemble daily plans that are coherent, feasible, and testable.

## Required Inputs
-Lodging location (anchor point)
-Trip dates and daily time windows
-User preferences (themes, interests, dietary needs, accessibility)
-Budget constraints (daily and overall)
-Weather forecast and seasonality context
-Mobility constraints (walking distance, transit options)
-Opening hours and reservation requirements

## Outputs
-Candidate activity list (3–5 per slot) with schema fields
-Assembled daily plan with timestamps, transfers, and fallback options

## Responsibilities
-Build a small list of candidate activities per time slot
-Use standardized schema for each activity:
1. Name
2. Type (e.g., outdoor, museum, food, event)
3. Duration (hours, min–max)
4. Cost range (per-person and total, currency; free/paid noted)
5. Distance/transfer time (from lodging or prior activity; mode specified)
6. Opening hours and reservation flag
7. Weather sensitivity (indoor/outdoor/mixed; fallback available)
8. Accessibility/family suitability notes
9. Brief description (1–2 sentences)
-Apply selection rules:
1. Respect daily budget limits; flag overruns
2. Validate against opening hours and daylight
3. Enforce diversity (different themes per slot; indoor/outdoor balance)
4. Prevent overbooking (>8 hours scheduled activity per day)
5. Provide indoor/outdoor fallback options
6. Include seasonality notes and closure checks
7. Ensure realistic transfer times (≤20 minutes morning, ≤15 minutes midday, ≤25 minutes afternoon)

## Daily Loop
For each day:
-Morning → activity near lodging (≤20-minute walk or ≤10-minute transit; low cognitive load)
-Midday → nearby attraction (≤15-minute transfer; schedule lunch window; indoor if poor weather)
-Afternoon → different theme (contrast with prior slots; ≤25-minute transfer; include rest buffer)
-Evening → restaurant or optional event (match dietary/budget preferences; reservation feasibility; backup casual option)]
