# Wildlife Observation Drone Payload Release

Build a drones prototype that uses flight controller, optical flow sensor, camera to release a lightweight payload at a target. Include setup instructions, a circuit diagram, tested firmware, and sample output.

> Build and test at safe low voltage. Real machinery, vehicles, aircraft, pumps, and power systems require qualified engineering review and certified safeguards.

## Project details

| Field | Value |
| --- | --- |
| Roadmap ID | 856 |
| Category | Drones |
| Platform | Pixhawk + Raspberry Pi |
| Difficulty | Beginner |
| Estimated build time | 16 hours |
| Connectivity | MAVLink |
| Core components | flight controller, optical flow sensor, camera |
| Control mode | closed loop control |

## Repository layout

- `src/main.py`: runnable firmware or application
- `docs/wiring.md`: suggested low-voltage wiring plan
- `docs/architecture.md`: system data flow
- `docs/test-plan.md`: repeatable verification steps
- `sample-data/example.json`: example telemetry record
- `tools/validate.py`: dependency-free repository validation

## Quick start

1. Run `python -m src.main --iterations 10 --interval 0.5`.
2. Run `python -m unittest discover -s tests -v`.
3. Replace `simulated_values()` with a hardware adapter after bench testing.

## Expected behavior

Payload Release demonstration with repeatable test steps. The default implementation supports simulated or generic analog inputs so the control path can be exercised before hardware-specific drivers are added.

## Hardware adaptation

The included code is a safe reference implementation. Update pin assignments and sensor conversions from the exact component datasheets, then repeat the test plan before connecting actuators.

## License

MIT
