# Thorondor Engineering Standards

This document defines the baseline engineering rules for Project Thorondor. These standards are intentionally conservative during prototype development and may be revised through Engineering Decision Records.

## 1. Design Priorities

Design decisions should prioritize, in order:

1. Safety
2. Reliability
3. Repairability
4. Modularity
5. Reproducibility
6. Outdoor durability
7. Efficiency
8. Appearance

Efficiency matters, but not at the expense of unsafe, fragile, or difficult-to-repair designs.

## 2. Print Envelope

Every printed part should fit within a 256 × 256 × 256 mm build volume unless an Engineering Decision Record approves an exception.

Large parts should be segmented using mechanical joints, alignment features, and replaceable fasteners rather than permanent adhesive alone.

## 3. Units and Drawings

- Use SI units.
- Dimensions are in millimeters unless otherwise stated.
- Mass is in grams or kilograms.
- Force is in newtons.
- Torque is in newton-meters.
- Pressure is in kilopascals or bar.
- Airflow is in liters per minute, with CFM permitted as a secondary unit.
- Wind speed is in meters per second, with mph permitted as a secondary unit.

CAD models and drawings must state units explicitly.

## 4. Hardware

- Prefer metric fasteners.
- Use the smallest practical set of recurring fastener sizes.
- Use stainless steel hardware for exposed outdoor service where galling and strength requirements permit.
- Use locknuts, thread-locking methods, safety wire, retaining rings, or other positive retention where loosening could create a hazard.
- Do not rely on printed threads for frequently serviced or safety-critical joints.
- Use heat-set inserts, captive nuts, through-bolts, or threaded metal components for repeated assembly.

Preliminary preferred sizes are M3, M5, and M8. Final standards require an accepted Engineering Decision Record.

## 5. Rotating Assemblies

- Rotating parts must be balanced before extended testing.
- Shaft connections must include positive axial retention.
- Safety-critical hubs must not rely solely on friction from a printed bore.
- Exposed pinch points should be guarded.
- Rotor-plane access must be restricted during testing.
- Designs must consider overspeed, gusts, fatigue, and loss of load.

## 6. Bearings and Shafts

- Use commercially available bearings with published dimensions and load ratings.
- Bearing fits must account for print material, printer variation, moisture, and temperature.
- Shafts should be metallic for primary rotating structures unless testing justifies another material.
- Bearings should be replaceable without destroying major printed parts.
- Outdoor bearing locations should include drainage, shielding, or seals.

## 7. Modular Interface

Every module interface should define:

- Mechanical mounting geometry
- Shaft or motion input
- Rotation direction
- Permitted torque and speed range
- Alignment method
- Retention method
- Guarding requirements
- Service access

Modules should be removable without disassembling the rotor or tower whenever practical.

## 8. Environmental Design

Outdoor parts must account for:

- Ultraviolet exposure
- Heat
- Rain and condensation
- Dust and insects
- Corrosion
- Freeze and temperature cycling where applicable
- Wind gusts and storms
- Wildlife interaction

Water must not be trapped inside printed cavities without drainage.

## 9. Safety Factors

Prototype parts must use conservative safety factors appropriate to uncertainty in printed material properties, layer adhesion, fatigue, and wind loading.

No general safety factor is declared yet. Each critical component must document its assumptions and test evidence.

## 10. Documentation Required for Released Parts

A release-ready part should include:

- Part name and number
- Revision
- Source CAD
- STEP export
- STL or other manufacturing file
- Material recommendation
- Print orientation
- Print settings
- Required hardware
- Assembly notes
- Known limitations
- Test status

## 11. Revision Control

Changes that affect fit, function, safety, compatibility, or manufacturing require a revision change and changelog entry.

Cosmetic changes that do not affect function may retain compatibility but must still be documented.

## 12. Verification

Claims such as weatherproof, balanced, rated, safe, continuous-duty, or compatible must be supported by documented testing or clearly marked as unverified.
