# Thorondor Bill of Materials Standard

This document defines how bills of materials are created and maintained for Project Thorondor.

## Purpose

A BOM must allow another builder to identify, source, fabricate, and assemble the documented configuration without relying on undocumented knowledge.

## Required Fields

Each BOM line should include:

- Item number
- Thorondor part number, when applicable
- Description
- Quantity
- Material or specification
- Manufacturer
- Manufacturer part number
- Approved alternate
- Source or vendor
- Unit cost when known
- Revision
- Notes

## Categories

Use these categories where practical:

- Printed parts
- Machined or fabricated parts
- Bearings and motion hardware
- Fasteners
- Shafting and structural members
- Elastomers and seals
- Pneumatic components
- Electronics and sensors
- Consumables
- Tools required but not included

## Sourcing Rules

- Prefer components available from multiple suppliers.
- Do not define a generic marketplace listing as the sole specification.
- Record dimensions, materials, ratings, and standards independently of the vendor link.
- Vendor links are conveniences and may become obsolete.
- Safety-critical substitutions require documented equivalence.

## Part Numbering

Until the final numbering standard is accepted, use this preliminary format:

`THR-<SYSTEM>-<NUMBER>-<REV>`

Examples:

- `THR-ROT-001-A` — rotor hub
- `THR-DRV-001-A` — drive-head housing
- `THR-PMP-001-A` — diaphragm pump body
- `THR-TWR-001-A` — tower bracket

Preliminary system codes:

- `ROT` — rotor
- `DRV` — drive head and transmission
- `PMP` — pump modules
- `TWR` — tower and mounting
- `AIR` — airline and diffuser system
- `ELE` — electronics
- `TST` — test fixtures
- `GEN` — general or shared parts

## Prototype BOMs

Each prototype stage should have its own BOM under its prototype directory.

Example:

```text
prototypes/P0/BOM.md
prototypes/P1/BOM.md
```

A prototype BOM must identify the exact configuration tested.

## Released BOMs

A release BOM must:

- Match a tagged release
- Reference exact part revisions
- Identify required tools and consumables
- State known unavailable or region-specific items
- Include estimated total cost when practical

## Change Control

Any substitution that changes fit, function, durability, safety, or performance must be documented and may require retesting.
