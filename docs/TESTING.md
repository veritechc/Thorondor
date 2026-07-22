# Thorondor Testing Standard

Testing is required to turn Thorondor from a concept into a reproducible engineering platform. Every test must identify the configuration, method, measurements, limitations, and result.

## Test Principles

- Test subsystems independently before full-system testing.
- Use measurable acceptance criteria whenever practical.
- Record failures, not just successes.
- Preserve raw data and photographs.
- Do not claim performance beyond the tested configuration.
- Stop testing when an unsafe condition appears.

## Required Test Record

Each test report should include:

- Test identifier
- Date and location
- Prototype and part revisions
- Objective
- Equipment and instruments
- Environmental conditions
- Procedure
- Measurements
- Observations
- Pass/fail criteria
- Result
- Damage or wear found
- Recommended actions

## P0 Test Categories

### Rotor Free-Spin Test

Measures bearing drag, alignment, wobble, and coast-down behavior.

Record:
- Starting RPM if instrumented
- Coast-down time
- Visible runout
- Noise or binding

### Startup Wind Test

Determines the approximate wind speed at which the unloaded rotor starts and continues rotating.

Record:
- Wind speed
- Wind direction variability
- Rotor configuration
- Startup behavior

### Loaded Rotation Test

Evaluates whether the rotor can drive the crank and pump without stalling.

Record:
- Wind speed
- Rotor RPM
- Load configuration
- Stalling or pulsation

### Airflow Test

Measures delivered airflow at defined backpressure.

Record:
- Liters per minute
- Backpressure
- Rotor RPM
- Wind speed
- Pump stroke and diaphragm configuration

### Shallow Diffuser Test

Confirms visible and sustained aeration through a shallow-water diffuser.

### Vibration Test

Checks rotor imbalance, structural resonance, loose fasteners, and bearing movement.

### Endurance Test

Runs the system for a defined period and inspects wear.

P0 target: cumulative 25 hours before progression to P1.

## Initial Performance Targets

These are provisional targets, not certified ratings:

- Unloaded self-start in moderate natural wind
- No persistent bearing binding
- Stable operation without visible fastener migration
- Measurable airflow under load
- Visible bubbles through a shallow diffuser
- No cracks, delamination, or permanent deformation after P0 endurance testing

Numerical wind, airflow, pressure, and vibration thresholds will be established after baseline measurements.

## Instrumentation

Preferred instruments include:

- Handheld anemometer
- Optical or magnetic tachometer
- Low-pressure gauge or manometer
- Airflow meter
- Thermometer or infrared thermometer
- Dial indicator for runout when available
- Scale and calipers

Instrument model and accuracy should be recorded.

## Safety During Testing

- Establish an exclusion zone around rotating parts.
- Never stand in the rotor plane.
- Use guards where practical.
- Secure loose clothing and hair.
- Provide an emergency stop, brake, restraint, or rapid unload method appropriate to the test.
- Do not test elevated structures before validating the rotor and drive system at low height.
- Inspect all fasteners before and after testing.

## Test Result Status

Use one of the following:

- **Pass** — all stated criteria met
- **Conditional Pass** — usable with documented limitations
- **Fail** — one or more criteria not met
- **Aborted** — stopped because of safety, equipment, weather, or procedural issues
- **Exploratory** — no formal acceptance criteria; information-gathering only

## Storage

Place procedures, raw data, photographs, and reports under `testing/` using a folder named for the test identifier.
