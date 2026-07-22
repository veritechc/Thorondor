# Thorondor System Architecture

This document describes the initial system architecture for Project Thorondor.

## System Overview

Thorondor converts wind energy into useful mechanical work through a modular platform.

```text
Wind
  ↓
Helical Savonius Rotor
  ↓
Main Shaft
  ↓
Drive Head
  ↓
Standard Module Interface
  ↓
Interchangeable Module
  ↓
Useful Output
```

The first output module is a diaphragm air pump for pond aeration.

## Architectural Goals

- Separate the wind-capture system from the application module.
- Allow modules to be removed without dismantling the rotor or tower.
- Keep bearings, shafts, fasteners, and wear components replaceable.
- Support prototype scaling without invalidating the overall architecture.
- Make each subsystem independently testable.

## Primary Subsystems

### 1. Rotor

The rotor captures wind from any direction and produces low-speed, high-torque rotary motion.

Initial concept:
- Vertical-axis helical Savonius geometry
- Segmented printed blade sections
- Metallic central shaft
- Replaceable top and bottom hubs
- Balanced modular assembly

### 2. Main Shaft

The main shaft transfers rotor torque to the drive head.

Requirements:
- Metallic construction
- Positive axial retention
- Replaceable bearings
- Defined rotational direction
- Documented torque and speed limits

### 3. Drive Head

The drive head supports the rotor shaft and converts or transfers motion to the attached module.

Responsibilities:
- Upper and lower bearing support
- Weather shielding and drainage
- Rotor-to-module alignment
- Crank or direct-drive attachment
- Guarding around moving parts
- Standardized module mounting

### 4. Module Interface

The module interface is the core platform boundary.

It must define:
- Mounting bolt pattern
- Alignment features
- Input shaft or crank geometry
- Rotation direction
- Speed and torque envelope
- Axial and radial load limits
- Service clearance
- Retention and locking method

The interface will remain provisional until accepted through an Engineering Decision Record.

### 5. Aeration Module

The first module converts rotary motion into reciprocating diaphragm motion.

Components:
- Eccentric crank
- Connecting rod
- Diaphragm assembly
- Inlet and outlet check valves
- Pressure-relief path
- Air outlet fitting
- Guarding and service cover

### 6. Tower and Base

The tower places the rotor in usable wind and supports all structural loads.

Initial philosophy:
- Do not 3D print primary tower members.
- Use wood, aluminum, or steel structural members.
- Print brackets, covers, guides, and non-critical fixtures where appropriate.
- Design for inspection, anchoring, and controlled lowering or service.

### 7. Air Delivery System

The aeration system downstream of the pump includes:
- Pressure relief
- Check valve against water backflow
- Airline
- Weighted or protected routing
- Bottom diffuser

The airline and diffuser are application components, not part of the universal mechanical interface.

## Cross-Cutting Concerns

### Safety

The architecture must account for:
- Rotor overspeed
- Gust and storm loading
- Pinch points
- Ejected parts
- Tower stability
- Backpressure
- Water backflow
- Maintenance lockout

### Modularity

Subsystems should be replaceable at clear boundaries. A failed pump should not require rebuilding the rotor. A revised rotor should not require redesigning every module.

### Instrumentation

Prototype architecture should support temporary sensors for:
- Wind speed
- Rotor RPM
- Shaft torque where practical
- Airflow
- Backpressure
- Vibration
- Bearing temperature

### Weather Resistance

Housings must drain, ventilate where needed, and avoid trapping condensation. Bearings and fasteners must remain inspectable.

## Future Modules

Potential modules include:
- Water pump
- Electrical generator
- Fountain mechanism
- Weather station power unit
- Irrigation pump
- Educational mechanical loads

Future modules must conform to the accepted interface or clearly declare incompatibility.

## Architecture Status

This architecture is provisional for the P0 phase. Dimensions, interfaces, and component selections are not yet frozen.
