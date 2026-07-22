# Thorondor Versioning Standard

Thorondor uses prototype-oriented versioning until the first stable hardware platform release.

## Prototype Versions

Prototype versions use the format:

`P<stage>.<revision>`

Examples:

- `P0.1` — first bench prototype revision
- `P0.2` — second bench prototype revision
- `P1.0` — first functional outdoor prototype baseline

The prototype stage communicates maturity:

- `P0` — bench proof of concept
- `P1` — functional outdoor prototype
- `P2` — weather-resistant field prototype
- `P3` — full-size Valinor installation

## Part Revisions

Individual parts use a revision suffix:

`THR-ROT-001-A`

Increment the revision when fit, function, safety, material, interface, or manufacturing changes.

## Releases

A release should include:

- Tagged source state
- Matching CAD and exports
- BOM
- Assembly guidance
- Print settings
- Test status
- Known limitations
- Changelog entry

## Compatibility

Changes that break module or mechanical compatibility must be clearly labeled.

Compatibility claims require documented fit and functional testing.

## Stable Versioning

After the platform reaches a stable release, the project may adopt semantic versioning or another release model through an Engineering Decision Record.
