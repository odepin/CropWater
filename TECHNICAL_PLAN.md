# CropWater - technical plan

**Planning document, not an implementation report.**

## Product objective

An offline, transparent soil-water balance for one crop workflow at a time.

## Intended system boundary

- **Input:** Invented field labels and sample weather files with documented origin.
- **Processing stages:** Crop, soil, and weather data contracts; Water-balance calculation core; Scenario runner and chart UI; Sample datasets and validation tests.
- **Output:** A documented synthetic scenario yields reproducible daily soil-water estimates.
- **Runtime / build stack (tentative):** Python 3.12+, Pandas, NumPy, Streamlit, pytest
- **Explicitly excluded:** Autonomous irrigation control, farm customer databases, real precise field positions, or guaranteed agronomic advice.

## Functional modules

- Represent crop stage, root zone, and available soil-water parameters
- Import public historical daily weather in a validated table format
- Estimate reference evapotranspiration with documented method inputs
- Simulate daily water balance and scenario-based irrigation
- Plot assumptions, uncertainty, and synthetic irrigation schedules

## Demonstration and acceptance cases

**Test 1:** Model a fictional orchard over a dry two-week period

**Test 2:** Show sensitivity to soil water-holding capacity

**Test 3:** Reproduce a known public training worked example

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

Weather input quality and crop coefficients dominate errors; make uncertainty visible.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
