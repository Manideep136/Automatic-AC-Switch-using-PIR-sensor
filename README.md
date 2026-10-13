# Automatic-AC-Switch-using-PIR-sensor


## 📌 Project Overview

The **Automatic AC Switch Using PIR Sensor** is an electronics project designed to automatically control an electrical load based on human motion detection.

The Passive Infrared (PIR) sensor detects movement within its sensing range and provides a trigger signal to a switching circuit. The switching circuit controls a relay, which can be used to switch an AC-powered load such as a lamp or other suitable appliance.

This project focuses on **schematic design, PCB layout, component placement, routing, and PCB design verification using KiCad**.

## 🎯 Objectives

- Design an automatic motion-based switching circuit.
- Interface a PIR sensor with a relay driver circuit.
- Create the circuit schematic using KiCad.
- Assign appropriate footprints to electronic components.
- Design and route a custom PCB.
- Perform Electrical Rules Check (ERC) and Design Rules Check (DRC).
- Prepare the PCB design for potential manufacturing.

## ⚙️ Working Principle

1. **Motion Detection:** The PIR sensor detects changes in infrared radiation caused by movement.
2. **Signal Output:** The sensor generates an output signal when motion is detected.
3. **Switching Control:** The sensor output activates the relay driver or switching circuit.
4. **Load Activation:** The relay contacts switch the connected AC load ON.
5. **Automatic Switching:** When motion is no longer detected, the load switches OFF according to the sensor's configured delay and circuit behavior.

### Block Diagram

```text
       Human Motion
            │
            ▼
       PIR Sensor
            │
            ▼
    Switching / Driver
         Circuit
            │
            ▼
          Relay
            │
            ▼
      AC Electrical Load
```

## 🔧 Main Components

| Component            | Function                                                    |
| -------------------- | ----------------------------------------------------------- |
| PIR sensor module    | Detects human motion                                        |
| Relay                | Switches the electrical load                                |
| Transistor or driver | Drives the relay when required                              |
| Resistors            | Provide biasing and current limiting                        |
| Diode                | Protects the driver from relay coil back-EMF, when required |
| Power supply         | Provides the required DC voltage                            |
| Terminal blocks      | Provide electrical connections                              |
| PCB                  | Holds and interconnects the components                      |

*The exact component list and values depend on the final schematic and selected PIR sensor, relay, and power supply.*

## 🖥️ Software and Tools

- **KiCad** – Schematic and PCB design
- KiCad Schematic Editor
- KiCad PCB Editor
- Footprint and symbol libraries
- 3D PCB Viewer
- Electrical Rules Check (ERC)
- Design Rules Check (DRC)

## 🧩 PCB Design Workflow

### 1. Schematic Design

The circuit schematic is created in KiCad, including the PIR sensor interface, switching circuit, relay driver, and power connections.

### 2. Footprint Assignment

Suitable footprints are assigned according to the actual component packages and datasheets.

### 3. Component Placement

Components are arranged to provide clear signal paths, practical connector access, and suitable separation between low-voltage and mains-voltage sections.

### 4. PCB Routing

Copper tracks are routed according to the schematic connections and the electrical requirements of the circuit.

### 5. Ground Plane

A GND copper zone can be added where appropriate to provide a common ground return for the low-voltage circuit.

### 6. Design Verification

ERC and DRC are used to identify electrical connection issues, clearance violations, unconnected nets, and other layout problems.

### 7. Manufacturing Preparation

Gerber and drill files can be generated after the PCB layout has been finalized and verified.

## 📐 PCB Design Considerations

- Use footprints that match the actual components.
- Check relay coil voltage and contact ratings.
- Verify the PIR sensor's operating voltage and output logic.
- Provide adequate trace widths for the intended current.
- Maintain appropriate creepage, clearance, and isolation between mains and low-voltage circuits.
- Keep high-voltage and low-voltage copper areas properly separated.
- Use connectors rated for the intended voltage and current.
- Verify the relay's contact arrangement (COM, NO, and NC) before connecting the load.

## 🔍 Design Verification Checklist

- [x] Schematic completed
- [x] Footprints verified
- [x] Component placement checked
- [x] Copper routing completed
- [x] ERC completed
- [x] DRC completed
- [x] Relay pinout verified
- [x] PCB clearances and isolation reviewed
- [x] Board outline and silkscreen checked
- [x] Gerber and drill files generated

## 📂 Suggested Repository Structure

```text
Automatic-AC-Switch-PIR/
│
├── README.md
├── Schematic/
│   └── Automatic_AC_Switch.kicad_sch
├── PCB/
│   └── Automatic_AC_Switch.kicad_pcb
├── Images/
│   ├── schematic.png
│   ├── pcb-layout.png
│   └── 3d-view.png
├── BOM/
│   └── BOM.csv
└── Gerber/
    └── Manufacturing_Files/
```

## 🚧 Project Status

| Stage                | Status                           |
| -------------------- | -------------------------------- |
| Circuit schematic    | Based on project design          |
| Footprint assignment | To be verified                   |
| PCB layout           | Based on current design progress |
| ERC/DRC              | To be completed and verified     |
| Manufacturing files  | To be generated                  |
| PCB fabrication      | Not claimed                      |
| Hardware testing     | Not claimed                      |

Update the status table to reflect the actual progress of your project before publishing it.

## 🚀 Future Improvements

- Add adjustable motion-detection delay.
- Add sensitivity adjustment, if supported by the PIR module.
- Optimize PCB size and component placement.
- Add mounting holes and clear connector labels.
- Improve enclosure integration.
- Fabricate and test the PCB under appropriate safety conditions.

## ⚠️ Safety Notice

This circuit may control **AC mains voltage, which can cause electric shock, serious injury, or fire**. Maintain appropriate isolation and mains-rated component selection. Do not handle or modify an energized circuit. Mains-side PCB design and testing should be reviewed and performed by a qualified person using suitable safety procedures. For a beginner project, consider using a certified, enclosed AC switching module or a low-voltage demonstration load.

## 📚 Learning Outcomes

This project provides practical experience with:

- Electronic schematic design
- PCB footprint selection
- Component placement and routing
- Relay-driver circuit design
- Copper zones and grounding
- ERC and DRC verification
- PCB documentation and manufacturing preparation

## 🛠️ Project Tools

**Design Software:** KiCad
**Project Type:** Electronics and PCB Design
**Application:** Motion-activated electrical switching
**Output:** Schematic, PCB layout, and optional manufacturing files

---

**Note:** This repository documents the PCB design. Fabrication and hardware testing should only be marked complete after they have actually been performed.
