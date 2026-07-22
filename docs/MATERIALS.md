# Thorondor Materials Guide

This guide defines preliminary material choices for Project Thorondor. Final selections for safety-critical parts require testing and may be revised through Engineering Decision Records.

## Printed Polymers

### ASA — Preferred Outdoor Default

Use ASA for long-term outdoor printed parts when the printer can handle it safely.

Advantages:
- Strong ultraviolet resistance
- Better heat resistance than PLA
- Good weather resistance
- Suitable for housings, blade segments, guards, and brackets

Considerations:
- Requires enclosure and ventilation
- Can warp
- Layer adhesion and print settings must be validated

### PETG — Prototype and Moderate Outdoor Use

PETG is acceptable for early prototypes and many non-critical outdoor parts.

Advantages:
- Easy to print
- Good moisture resistance
- Good impact resistance

Considerations:
- Can creep under sustained load
- Dark parts may soften in direct summer sun
- Ultraviolet durability varies by formulation

### Nylon and Reinforced Nylon

Use nylon or fiber-reinforced nylon only when its benefits justify moisture control and more difficult printing.

Potential uses:
- Gears
- Bushings
- High-wear links
- Compact structural parts

Considerations:
- Moisture absorption
- Dimensional change
- Abrasive filament requires hardened nozzles
- Fiber-filled parts may have reduced layer bonding

### PLA

PLA may be used for fit checks, visual mockups, jigs, and indoor bench testing only. It is not approved for permanent outdoor or safety-critical components.

## Metals

### Stainless Steel

Preferred for exposed fasteners, shafts, pins, and hardware where corrosion resistance is important.

Select grade and strength based on the application. Stainless fasteners can gall; use suitable anti-seize where appropriate.

### Carbon Steel

Acceptable for protected shafts and high-strength components when corrosion protection is provided.

### Aluminum

Useful for tower members, plates, guards, and low-mass structural components. Avoid direct contact with dissimilar metals in wet environments without considering galvanic corrosion.

## Elastomers

### EPDM

Preferred preliminary diaphragm and outdoor seal material because of its resistance to weather, ozone, and water.

### Silicone

Useful for seals and flexible parts when temperature resistance is important. Mechanical fatigue performance must be tested for diaphragm use.

## Bearings

Use sealed, commercially available bearings with published dimensions and load ratings. Bearings must remain replaceable and should not be permanently encapsulated in printed parts.

## Adhesives and Sealants

Adhesive must not be the sole structural retention method for rotating or elevated safety-critical parts.

Outdoor sealants should be compatible with the selected polymer and allow maintenance where practical.

## Pond and Wildlife Compatibility

Materials near the pond must not intentionally leach toxic substances. Avoid exposed lubricants, coatings, pressure-treated materials, or uncured chemicals where runoff or direct contact could affect water quality.

## Material Documentation

Each released part must identify:
- Recommended material
- Approved alternatives
- Prohibited materials
- Environmental assumptions
- Required post-processing
- Test status
