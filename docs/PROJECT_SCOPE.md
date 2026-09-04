# SATCOM-OPS Project Scope

## Purpose

SATCOM-OPS is intended to become an independent desktop console for observing the health of a Starlink system, investigating degraded service, and reviewing recent operational history.

The v0.1 objective is situational awareness and diagnostics. It is not service provisioning, account management, network control, or a replacement for vendor support tools.

## Planned v0.1 capabilities

| Area | Initial intent |
| --- | --- |
| SITREP | Summarize current reachability, service state, and notable conditions. |
| Latency | Present latency measurements and ping success without hiding failed samples. |
| Uptime | Track observed application and link availability. |
| Events | Record outages, recoveries, and diagnostically relevant state changes. |
| Obstructions | Present obstruction information when a supported, authorized interface provides it. |
| Diagnostics | Expose useful observations and clear failure reasons for troubleshooting. |
| History | Retain bounded local history for review and trend comparison. |

## Architecture direction

The source tree begins with four implementation-neutral boundaries:

- `src/app/` — application coordination and use cases
- `src/core/` — domain models and operational rules
- `src/platform/` — operating-system, storage, and external-interface adapters
- `src/ui/` — desktop presentation

These boundaries are provisional. A language, desktop toolkit, persistence layer, packaging system, and supported data interfaces will be selected only after requirements and interface availability are validated.

## Operating principles

- Prefer local processing and storage where practical.
- Collect only data required for an operator-visible capability.
- Never embed credentials or identifying network data in source, fixtures, logs, screenshots, or issue templates.
- Distinguish observed facts from inferred conditions.
- Preserve failed and unavailable states instead of presenting stale data as current.
- Document supported interfaces and their stability before depending on them.

## Explicitly out of scope for the foundation

- Working application code
- Selection of a programming language or desktop framework
- Vendor account access or automation
- Remote control of customer equipment
- Cloud telemetry collection
- Logos, product trade dress, or any claim of vendor endorsement
- Promises of compatibility with undocumented or unstable interfaces

## Project identity

SATCOM-OPS is unofficial and independent. It is not affiliated with, endorsed by, or sponsored by Starlink, SpaceX, or their affiliates. Product and company names are used only to describe the systems the project is intended to observe.

