# Project Thorondor Master Plan

This document is the living program plan for Project Thorondor. It tracks the system vision, workstreams, prototype milestones, major decisions, and release gates.

## Mission

Create an open-source, modular, mostly 3D-printable wind-powered mechanical platform, beginning with pond aeration and designed to support interchangeable modules.

## Program Goals

1. Produce a functional wind-powered pond aeration prototype.
2. Standardize the rotor, shaft, bearings, drive head, tower interface, and module interface.
3. Keep printable parts within a 256 × 256 × 256 mm build volume.
4. Use repairable, readily available hardware wherever practical.
5. Publish reproducible CAD, print files, BOMs, assembly instructions, and test results.
6. Preserve compatibility between modules whenever practical.

## Workstreams

### Governance and Documentation

- Repository structure
- Contribution and conduct policies
- Safety reporting
- Changelog and versioning
- Engineering Decision Records

### Mechanical Platform

- Helical Savonius rotor
- Rotor hub and segmented blades
- Main shaft and bearing supports
- Modular drive head
- Tower and mounting system
- Overspeed and storm protection

### Aeration Module

- Crank and connecting rod
- Diaphragm pump
- Check valves
- Airline and pressure relief
- Pond diffuser

### Fabrication

- Material selection
- Print settings and tolerances
- Fastener and insert standards
- Part numbering and revision marking
- Outdoor durability testing

### Instrumentation and Testing

- Wind speed
- Rotor RPM
- Airflow
- Backpressure
- Vibration
- Bearing temperature
- Runtime and wear

### Future Modules

- Water pump
- Generator
- Fountain
- Weather station
- Battery charging
- Irrigation

## Prototype Milestones

### P0 — Bench Prototype

**Purpose:** Prove the rotor, bearings, drive mechanism, and low-pressure air pumping concept.

Exit criteria:

- Rotor turns freely and self-starts in outdoor testing.
- Drive head operates without binding.
- Pump produces visible bubbles through a shallow test diffuser.
- Major loads and failure points are documented.

### P1 — Functional Outdoor Prototype

**Purpose:** Validate useful airflow and modular assembly outdoors.

Exit criteria:

- Measurable airflow across a practical wind range.
- Replaceable air-pump module.
- Stable tower or test stand.
- At least 25 hours of cumulative operation.

### P2 — Field Prototype

**Purpose:** Validate weather resistance and continuous service.

Exit criteria:

- Weather-resistant construction.
- Defined storm shutdown or overspeed strategy.
- At least 100 hours of outdoor operation.
- Documented maintenance inspection.

### P3 — Valinor Installation

**Purpose:** Operate a full-size system on the pond and validate long-term performance.

Exit criteria:

- Installed bottom diffuser.
- Verified airflow at operating depth.
- Seasonal operation data.
- Complete assembly, operation, and maintenance documentation.

## Sprint Plan

### Sprint 1 — Project Foundation

- Governance documents
- Architecture
- Standards
- BOM structure
- Test framework
- Initial Engineering Decision Records
- Repository folder placeholders

### Sprint 2 — Identity and Documentation System

- Logo and project banner
- Visual style guide
- Part numbering standard
- Engineering drawing template
- README graphics and status badges

### Sprint 3 — Mechanical Standards

- Shaft selection
- Bearing selection
- Fastener standard
- Module interface requirements
- Printing tolerances
- Material rules

### Sprint 4 — P0 CAD and Fabrication

- Bench rotor
- Rotor hub
- Drive-head housing
- Crank mechanism
- Pump fixture
- Test stand

### Sprint 5 — P0 Testing and Review

- Test procedures
- Data collection
- Failure analysis
- Design review
- P1 recommendations

## Decision Process

Major, durable decisions are documented as Engineering Decision Records in `docs/decisions/`. Draft decisions may change. Accepted decisions remain part of the historical record even when later superseded.

## Current Status

- Current phase: P0 planning
- Current sprint: Sprint 1 — Project Foundation
- Development branch: `agent/project-foundation`
- First application: Pond aeration

## Immediate Next Actions

1. Complete Sprint 1 documentation.
2. Define measurable P0 requirements.
3. Record rotor and modular-platform decisions.
4. Select preliminary shaft, bearings, and fasteners for bench testing.
5. Design the smallest useful rotor prototype for the available printers.
