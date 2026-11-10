# AURORA — Crew Health Companion

AURORA is a self-guided health monitoring prototype for long-duration crewed missions. It helps an astronaut gather routine observations, review personal patterns, and prepare a concise summary for medical support. It is designed for self-sufficiency during communication delays while keeping clinical decisions with the crew health plan and flight surgeon.

## Open the prototype

Open `index.html` in a modern browser. It is a single-file web app with no server, installation, or external runtime dependencies. The sample mission and readings are fictional. Use **Record check-in** to enter your own values; the app stores those entries in that browser’s local storage.

## What it does

- Shows a mission-oriented overview with heart rate, blood pressure, oxygen saturation, temperature, sleep, and mood.
- Provides a guided check-in for those measures, optional blood glucose, symptoms, and notes about context.
- Shows sample trends before personal entries exist. After an entry is saved, charts use only saved readings; a dashed line appears as a personal median after three or more readings. It is descriptive, not a clinical limit.
- Lets the crew explore cardiovascular, sleep and wellbeing, bone and muscle, immune and environmental, and nutrition context.
- Prompts the user to follow the onboard emergency medical protocol when they select severe chest pain, severe difficulty breathing, fainting, or new confusion.
- Builds a reviewable care summary that the user can download and share through an approved mission channel.
- Works without a network connection after the file is available. Check-ins are stored locally and are not automatically transmitted.

## Why this approach

NASA’s Human Research Program describes five connected hazards: radiation, isolation and confinement, distance from Earth, altered gravity, and hostile or closed environments. Those exposures can affect cardiovascular function, bone and muscle, immune responses, sleep, mood, and nutrition. A useful check-in therefore combines measurements with symptoms, sleep and wellbeing, routine countermeasures, and the context around a reading.

Generic “normal” ranges can be misleading during spaceflight and across individual crew members. A flight-ready version should load clinician-approved thresholds and measurement schedules for each astronaut and mission, account for sensor provenance and measurement conditions, and route alerts through secure private medical communications. AURORA’s prototype deliberately avoids diagnosis, automatic treatment advice, and fabricated alert cutoffs.

## Prototype scope and next steps

This is a front-end challenge prototype, not certified medical software. It has no device integration, encryption, authenticated user accounts, crew-specific clinical thresholds, clinical decision support, or connection to mission control. Local browser storage is not encrypted and should not be used for real medical records.

For a flight-ready concept, the next steps are to co-design with flight surgeons and crew, define mission-specific measurement procedures and escalation thresholds, protect data at rest and in transit, support delayed private store-and-forward communication, validate sensor inputs and usability in analog environments, and evaluate the software under the program’s medical operations and safety requirements.

## References

- [NASA Space Apps — Health Monitoring Software challenge](https://www.spaceappschallenge.org/2026/challenges/health-monitoring-software/)
- [NASA Human Research Program — Five Hazards of Human Spaceflight](https://www.nasa.gov/hrp/hazards/)
- [NASA Human Research Program — Risks of Human Spaceflight](https://www.nasa.gov/hrp/risks/)
- [NASA-STD-3001 — Medical Operations](https://www.nasa.gov/reference/6-0-medical-operations/)
- [NASA — Cardiovascular and Vision Research](https://www.nasa.gov/directorates/esdmd/hhp/cardiovascular-and-vision/)
