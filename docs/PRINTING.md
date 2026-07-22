# Thorondor 3D Printing Standard

This document defines baseline additive-manufacturing practices for Project Thorondor.

## Printer Envelope

All standard printable parts must fit within a 256 × 256 × 256 mm build volume.

Parts larger than that envelope must be segmented with documented joints, alignment features, and fasteners.

## Preferred Processes

The baseline process is fused-filament fabrication using consumer-grade printers.

Source CAD should remain editable and should not be optimized solely around one printer brand or slicer.

## Default Nozzle and Layer Assumptions

Unless a part specifies otherwise:

- Nozzle diameter: 0.4 or 0.6 mm
- Prototype layer height: 0.20 to 0.30 mm
- Functional wall count: at least 4
- Functional top and bottom layers: at least 5
- Infill: selected by load path, not by habit

Critical parts must define their own print settings.

## Orientation

Part orientation must be chosen around load paths and layer adhesion.

Do not orient safety-critical parts so that primary tensile loads act only across layer bonds when another practical orientation exists.

Every released STL must include a recommended print orientation.

## Tolerances

Printed fits must be validated with calibration coupons before finalizing production parts.

Initial design clearances may use the following as starting points only:

- Sliding fit: 0.20 to 0.40 mm per side
- Captive nut pocket: 0.10 to 0.30 mm oversize
- Bearing pocket: printer- and material-specific; always test
- Shaft clearance hole: nominal diameter plus printer-specific allowance

These are not guaranteed values. Each printer and material combination must be calibrated.

## Fasteners and Inserts

- Prefer through-bolts for safety-critical joints.
- Use heat-set inserts or captive nuts for frequently serviced joints.
- Avoid self-tapping directly into printed plastic where repeated maintenance is expected.
- Do not rely on printed threads for primary rotor retention.

## Segmented Parts

Segment joints should include:

- Positive alignment geometry
- Mechanical fasteners
- Load paths that do not depend on adhesive alone
- Drainage where cavities could collect water
- Replaceable damaged sections

## Supports

Design parts to minimize supports where practical, but do not weaken a part merely to make it support-free.

Support interfaces must not occur on critical bearing, sealing, or alignment surfaces unless post-processing is documented.

## Identification

Released parts should include, where size permits:

- Part number
- Revision letter or number
- Orientation mark when assembly direction matters
- Material or process note when confusion could create a hazard

## Quality Checks

Before assembly, inspect functional parts for:

- Layer separation
- Under-extrusion
- Warping
- Cracks around inserts
- Poor bearing fit
- Dimensional mismatch
- Surface defects at load concentrations

Reject damaged safety-critical parts rather than repairing them cosmetically.

## Outdoor Post-Processing

Outdoor parts may require:

- UV-resistant coating
- Sealing of exposed layer lines
- Drain holes
- Corrosion-resistant hardware
- Heat shielding from dark surfaces in direct sun

Any coating that changes dimensions must be accounted for in fit checks.

## Release Package

Each released printed part should include:

- Source CAD
- STEP export
- STL or 3MF
- Recommended material
- Nozzle and layer guidance
- Orientation image
- Support guidance
- Hardware list
- Known limitations
- Test status
