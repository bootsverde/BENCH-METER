# Bench Test

A three-function bench meter built from AutomationDirect CLICK PLC parts and a C-more touch panel.

- **AC volts** to 480 V, through a VACT500-42L isolated true-RMS transducer
- **DC volts** to 30 V, through a 3:1 precision divider
- **Ohms and continuity**, using a ratio ohmmeter with 10 V excitation

## Hardware

| Part | Model |
|---|---|
| PLC | CLICK C0-02DD2-D (4 DC in, 4 sourcing out, 3 serial ports) |
| Analog I/O | C0-4AD2DA-2 (4 in / 2 out, 0–10 V) |
| Touch panel | C-more EA7-T8C (640 × 480) |
| AC transducer | AcuAMP VACT500-42L |
| 24 V supply | RHINO PSB24-060S-P |
| Conditioning board | BusBoard ST2 stripboard |

## Documents

Each document is an HTML page (open it in a browser) with a matching PDF for printing.

| File | Contents |
|---|---|
| `bench-meter-wiring` | System wiring diagrams, point-to-point wire list, parts and scaling math |
| `bench-meter-pcb` | Hole-by-hole ST2 stripboard layout: cuts, links and part placement |
| `bench-meter-ladder` | CLICK ladder program: address map, module setup and all rungs |
| `bench-meter-hmi` | C-more screens: mockups and object-by-object build sheet |
| `bench-meter-panel` | Front panel: HMI cutout, 22 mm controls, jack layout and hole schedule |

## Safety

The AC input is connected to line voltage up to 480 V. Only the AC jacks, fuses F1/F2 and the VACT input are rated for it. Build and test at 120 V first, and keep a CAT III/IV handheld meter for live troubleshooting.
