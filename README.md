# Rover Device Drivers

Open-source, reusable sensor and hardware integration work for small robots and connected devices. This repository is public so people can inspect, use, and contribute to drivers that stand on their own.

**Status:** project scaffold. No Rover-authored driver has been released or physically validated here yet. The working StickC Plus SE light-meter diagnostic currently lives in the private Rover robot project; it is not a published library.

## What belongs here

- `drivers/`: original, device-focused drivers and adapters with documented interfaces and tests.
- `examples/`: minimal standalone examples that demonstrate one component at a time.
- `hardware/`: verified pinouts, wiring, power requirements, and reusable mechanical reference material.
- `docs/`: supported boards, module revisions, measurements, and upstream attribution.

Each driver should state its tested board and module revision, supported toolchain, wiring and power assumptions, measurement units, failure behaviour, and exact validation evidence. Releases will be versioned so applications can pin a known working version.

## Boundary

The Rover robot application is private. Its movement policy, sensor fusion, app protocol, credentials, device identity, and raw evidence are not published here. This repository does not contain firmware for the full robot or any deployment keys.

We use upstream libraries when they already solve a device well. We do not copy vendor source code, datasheets, product photography, or schematics into this repository without reviewing their licences and attribution. See [upstream components](docs/upstream.md).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Source originally created for this repository is available under the [MIT License](LICENSE). Third-party projects retain their own licences.
