# Grid Output Interface – IX-Aus-Amerika-mit-Liebe

This document defines how the tower’s electrical output is safely and legally connected to:
- Public utility infrastructure in Germany
- Local microgrids or emergency backup nodes
- Grid-isolated energy banks (optional)

All output specifications match real German and EU grid standards including:
- **DIN VDE 0100 / 411** (grounding, neutral configuration)
- **DIN VDE 0126-1-1** (anti-islanding for grid-connected inverters)
- **IEC 61400-21** (grid code compliance for distributed energy)

---

## ⚡ Final AC Output Specs

| Parameter            | Value                  |
|----------------------|------------------------|
| Voltage (L-N)        | 230V AC                |
| Voltage (L-L)        | 400V AC (3-phase)      |
| Frequency            | 50 Hz (±1%)            |
| Max output (per tower)| 200–250 kW (scalable) |
| Harmonic distortion  | < 5% THD               |
| Output phase config  | 3P+N+PE (Neutral + Protective Earth) |

---

## 🔌 Interface Pathway

### Stage 1: Inverter → Isolation Transformer
- Fully shielded dry-type transformer
- Steps AC output to standard **400V 3-phase grid voltage**
- Optional center-tap N if site requires **split-phase subdistribution**
- Transformer grounded per **VDE 0100-540**

### Stage 2: Transformer → Grid Feed Relay
- Relay is **grid-aware**, synchronizes phase/frequency
- DIN rail or rack-mounted
- Surge clamping MOV banks added to L1, L2, L3

### Stage 3: Circuit Disconnect + Logger
- High-voltage **dry switch disconnect** (manual + automatic)
- Optional **Modbus/BACnet logger** to track:
  - Output phase stability
  - Lightning event power spikes
  - Energy delivered per cycle
  - Fault shutdowns

---

## 🛡️ German Legal Requirements (Confirmed)

| Regulation | Description |
|------------|-------------|
| **DIN VDE 0126-1-1** | Anti-islanding behavior for grid-connected systems. Tower will detect grid failure and auto-disconnect. |
| **DIN VDE 0100-600** | Initial and periodic verification of grounding and RCD systems. |
| **VDE-AR-N 4105** | Parallel operation of distributed generation. Defines inverter certification and feed limits. |
| **EN 50549-1** | Interface for decentralized energy → low-voltage networks. Matches transformer layout and safety logic. |

---

## 🧱 Physical Connectors + Cabling

| Element               | Spec                      | Notes |
|-----------------------|---------------------------|-------|
| AC Cable (Tower → Grid) | 5x35 mm² armored Cu | 3P + N + PE, UV/salt rated |
| Inverter Output Lugs | M10 copper compression | DIN 46234 compliant |
| Transformer Output Bus | 3x400V star, 50 Hz       | Float-grounded or solid-neutral |
| Ground Mesh           | Copper tape, 100 mm² min | Buried mesh in seabed or trench grid |

---

## 🔌 Deployment Modes

### 1. Urban Grid-Tie
- Connect to municipal substation
- Optional “feed-in limiter” if required by grid operator
- Relay must meet **DNO approval (Netzbetreiber)** for automated sync

### 2. Microgrid / Remote Village
- Output flows to battery + inverter bank
- Tower acts as **primary generator** or **blackstart stabilizer**

### 3. Emergency Backup (Hospitals, Ports)
- Stored energy only used on-grid failure
- Load shedding logic built into inverter logic (via digital relay)

---

## 🔒 Fault Safety Features

- **Overcurrent cutoff** (250A breaker on AC side)
- **Reverse flow protection** (Schottky-blocking topology if islanded)
- **Grid failure sense pin** on inverter (disconnects if utility fails)
- **Arc-fault interruption breaker** (AFDD required in Germany as of 2020)
- **Ground fault detection relay** wired to base grounding mesh

---

## ✅ Summary

The IX tower outputs:
- Standard 230/400V 3-phase AC at 50 Hz
- Legally feedable into Germany’s low-voltage grid systems
- Fully compliant with VDE, IEC, and EN regulations for distributed energy

This isn’t "compatible someday" — it’s **plug-in ready now**.

> A machine this tall needs a plug this real. And now it has one.

— Bryce Wooster
