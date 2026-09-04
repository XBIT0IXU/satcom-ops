# SATCOM Operations Console [SATCOM-OPS]

SATCOM-OPS is an independent desktop application project for monitoring and diagnosing Starlink systems. Its mission is to give operators a clear, local-first view of communications health without obscuring the underlying observations.

> [!IMPORTANT]
> SATCOM-OPS is an unofficial, independent source-available project. It is not affiliated with, endorsed by, or sponsored by Starlink, SpaceX, or their affiliates. Starlink and SpaceX are trademarks of their respective owners.

## Initial v0.1 scope

The first release is planned around:

- SITREP and current system status
- latency and ping success
- uptime and availability
- outages and operational events
- obstruction observations
- diagnostics
- local history and trend review

This repository currently contains the project foundation only. It does not yet contain a working application.

## Design direction

- Desktop-first and operator-focused
- Local-first data handling where practical
- Readable status, evidence, and failure states
- Clear separation between data acquisition, operational logic, platform integration, and presentation
- No commitment to a language or UI framework until requirements and supported interfaces are validated

See [docs/PROJECT_SCOPE.md](docs/PROJECT_SCOPE.md) for the initial architecture and scope boundaries.

## Status

**Foundation / pre-v0.1**

Interfaces, compatibility, packaging, and implementation technology are not yet established.

## License

Source code is available under the [PolyForm Noncommercial License 1.0.0](LICENSE). Copyright attribution to XBIT0IXU must be preserved as specified in [NOTICE](NOTICE). Commercial use is not permitted under this license and requires separate written permission from XBIT0IXU.
