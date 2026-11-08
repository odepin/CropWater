# CropWater

> Crop-specific soil-water balance scenarios with public weather inputs.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, used. Update this status to reflect real work.

## What it is

CropWater is a proposed specialist software tool for Specialty crop growers, agricultural training centers, and vineyard advisors. Irrigation guidance is often too broad and does not explain local crop assumptions. The intended differentiation is: An offline, transparent soil-water balance for one crop workflow at a time.

## Intended users and use cases

- Model a fictional orchard over a dry two-week period
- Show sensitivity to soil water-holding capacity
- Reproduce a known public training worked example

## Planned features

- Represent crop stage, root zone, and available soil-water parameters
- Import public historical daily weather in a validated table format
- Estimate reference evapotranspiration with documented method inputs
- Simulate daily water balance and scenario-based irrigation
- Plot assumptions, uncertainty, and synthetic irrigation schedules

## Proposed technology

Python 3.12+, Pandas, NumPy, Streamlit, pytest

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- Crop, soil, and weather data contracts
- Water-balance calculation core
- Scenario runner and chart UI
- Sample datasets and validation tests

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Invented field labels and sample weather files with documented origin.`

## Data boundaries and exclusions

Autonomous irrigation control, farm customer databases, real precise field positions, or guaranteed agronomic advice. All public examples should use Invented field labels and sample weather files with documented origin.

## Known limitations / validation risks

Weather input quality and crop coefficients dominate errors; make uncertainty visible.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Specialty crop modules, agronomic report templates, and sensor import adapters. 

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

