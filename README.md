# Thorondor

> **Harnessing Wind. Empowering Innovation.**

**Project Thorondor** is an open-source engineering initiative by **Sillmiron Studios LLC** to create a modular, mostly 3D-printable wind-powered mechanical platform.

Thorondor is not intended to be a single-purpose windmill. It is being developed as a reusable mechanical platform capable of driving interchangeable modules through a standardized power interface. The first application is pond aeration; future modules may support water pumping, electrical generation, environmental monitoring, irrigation, and other wind-powered tools.

## Project Status

Thorondor is currently in the **P0 — Bench Prototype** phase. Specifications, interfaces, and components are expected to change as testing progresses.

## Vision

Build a beautiful, repairable, expandable, and affordable wind-powered platform that can be manufactured using consumer 3D printers and commonly available hardware.

### Core Principles

- Modular by design
- Mostly 3D printable
- Open-source and community-friendly
- Repairable with ordinary tools
- Built around standardized, readily available hardware
- Scalable from desktop prototypes to full-size installations
- Designed for outdoor service and long-term iteration

## Current Objective

Develop and validate a wind-powered pond aeration system using:

- A helical Savonius vertical-axis rotor
- A modular drive head
- A direct mechanical crank system
- A diaphragm air-pump module
- Bottom-diffuser pond aeration

## Prototype Roadmap

| Stage | Goal |
|---|---|
| **P0** | Bench rotor, bearing, drive-head, and air-pump proof of concept |
| **P1** | Small outdoor functional prototype with measurable airflow |
| **P2** | Weather-resistant field prototype with modular interface |
| **P3** | Full-size Valinor installation and long-term durability testing |

See [ROADMAP.md](ROADMAP.md) for the detailed roadmap.

## Planned Modules

- Pond aeration
- Water pumping
- Electrical generation
- Decorative fountain
- Weather and environmental monitoring
- Battery charging
- Irrigation

All modules are intended to share a common mechanical interface so they can be changed without redesigning the tower or rotor.

## Design Constraints

Every major printable component should:

- Fit within a **256 × 256 × 256 mm** print volume
- Be printable on consumer-grade fused-filament printers
- Prefer standard metric fasteners and commercially available bearings
- Be field-serviceable with basic tools
- Minimize proprietary or difficult-to-source components
- Be documented with source CAD, export files, print guidance, and revision history

See [docs/STANDARDS.md](docs/STANDARDS.md) and [DESIGN_PRINCIPLES.md](DESIGN_PRINCIPLES.md).

## Repository Structure

```text
Thorondor/
├── cad/                 Source CAD and neutral STEP exports
├── docs/                Architecture, standards, BOMs, and engineering decisions
├── electronics/         Future electronics and sensor designs
├── firmware/            Future firmware and telemetry software
├── images/              Project photographs and documentation images
├── prototypes/          Prototype-specific files and notes
├── renders/             CAD renders and visual concepts
├── stl/                 Release-ready printable mesh files
└── testing/             Test procedures, raw results, and reports
```

## Engineering Decisions

Major design choices are recorded as Engineering Decision Records in [`docs/decisions/`](docs/decisions/). These records document the problem, alternatives, decision, and consequences so future contributors can understand why the system evolved as it did.

## Safety

Thorondor includes rotating machinery, elevated structures, stored mechanical energy, outdoor electrical equipment, and pond installations. Prototype designs are experimental and must be evaluated for local conditions before use. See [SECURITY.md](SECURITY.md) for reporting safety-sensitive design problems.

## Contributing

Contributions involving CAD, mechanical design, testing, documentation, electronics, firmware, and new modules are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting changes.

## License

Unless a subdirectory states otherwise, the repository is released under the [MIT License](LICENSE).

The project may adopt purpose-specific licenses for hardware design files, software, and documentation as the repository matures. Any future licensing change will be documented clearly and will not retroactively alter prior releases.

## About

Thorondor is designed and maintained by **Sillmiron Studios LLC**.

The name is inspired by the works of J.R.R. Tolkien. Project Thorondor is an independent engineering project and is not affiliated with or endorsed by the Tolkien Estate or related rights holders.
