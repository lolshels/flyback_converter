# Flyback Switching Power Supply

Design and simulation work for an isolated flyback SPS.

## Target Specifications

| Parameter | Value |
|---|---|
| Input | 90–264 VAC |
| Input frequency | 60 Hz |
| Output | 12 V |
| Output power | 24 W |
| Output current | 2 A |
| Switching frequency | 100 kHz |
| Efficiency target | 85% |
| Regulation | ±5% |
| Isolation | Yes |

Output is fixed for this version. An adjustable-output version is planned as a future iteration.

## Project Status

- [x] Bridge rectifier + bulk capacitor front-end — designed and simulated in LTspice
- [ ] Inrush current limiting (NTC/fuse)
- [ ] Flyback transformer design
- [ ] Primary-side switch + controller selection
- [ ] Secondary-side rectification + output filtering
- [ ] Feedback/compensation loop
- [ ] PCB layout

## Repo Structure

```
/reports   - Written validation summaries with simulation screenshots
/sim       - LTspice schematic (.asc) and simulation files
```

## Reports

- [Rectifier & Bulk Capacitor Stage Validation](reports/rectifier_stage_validation_summary.md)

## Tools

- LTspice (schematic capture and simulation)
