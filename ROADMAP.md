# CropWater - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A documented synthetic scenario yields reproducible daily soil-water estimates.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Specify soil, crop, and weather inputs | 8 | Validated models with clear units |
| 2 | Implement daily water balance | 12 | Reference-backed calculation tests |
| 3 | Add ET calculation module | 10 | Synthetic and published-example cross checks |
| 4 | Create scenario viewer | 9 | Users can compare irrigation assumptions |
| 5 | Build reports and CSV export | 7 | Audit-friendly daily outputs |
| 6 | Test numerical limits and document | 10 | Boundary tests and method citations |
| | **Total estimated** | **56** | |

## Detailed milestones

### 1. Specify soil, crop, and weather inputs (8 estimated hours)

- [ ] Deliverable: Validated models with clear units.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Implement daily water balance (12 estimated hours)

- [ ] Deliverable: Reference-backed calculation tests.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Add ET calculation module (10 estimated hours)

- [ ] Deliverable: Synthetic and published-example cross checks.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Create scenario viewer (9 estimated hours)

- [ ] Deliverable: Users can compare irrigation assumptions.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Build reports and CSV export (7 estimated hours)

- [ ] Deliverable: Audit-friendly daily outputs.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Test numerical limits and document (10 estimated hours)

- [ ] Deliverable: Boundary tests and method citations.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: Weather input quality and crop coefficients dominate errors; make uncertainty visible.
- Commercial hypothesis (not validated): Specialty crop modules, agronomic report templates, and sensor import adapters.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
