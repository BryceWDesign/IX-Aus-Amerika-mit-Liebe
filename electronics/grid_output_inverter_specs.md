# 🔌 Grid Output Inverter Specifications and Integration

This document specifies the full configuration and real-world inverter components required to take the harmonized DC output from the capacitor tank and convert it into 230V AC @ 50Hz, synchronized with Germany’s grid standards.

---

## 🎯 Functional Requirements

| Parameter         | Target Value              |
|------------------|---------------------------|
| Input Voltage     | 180V–420V DC              |
| Output Voltage    | 230V AC ±5%               |
| Frequency         | 50 Hz ±0.5 Hz             |
| Continuous Output | ≥100 kW (per tower)       |
| Surge Handling    | 200% for 2 sec (lightning burst damping) |
| Total Harmonic Distortion (THD) | <3%        |
| Sync Method       | PLL Grid Auto-Sync        |

---

## 🧰 Real-World Inverter BOM

| Component                  | Spec / Source Example                        | Notes |
|---------------------------|----------------------------------------------|-------|
| Inverter Core             | SMA Sunny Tripower CORE2 (or equiv.)         | 110 kW, grid-tied |
| MPPT Tracker              | Victron BlueSolar MPPT 250/100               | DC voltage stabilization |
| Surge Arrestor            | DEHNventil M TT 275                          | Lightning class I protection |
| DC Disconnect             | Siemens 5SE2 or Schneider GV2 series         | Isolation safety |
| EMI Filter Unit           | Schaffner FN3280-100-34                      | Grid compliance |
| AC Contactor              | ABB AF1350 or Eaton DILMP1500                | For failover and maintenance switching |
| Smart Grid Interface      | RS485/Modbus or EtherCAT protocol bridge     | Supports regional utility sync |

---

## ⚙️ Control + Protection Logic

- **DC input** from capacitor bank is routed through MPPT to handle voltage drift.
- **Inverter** auto-detects local grid phase using Phase-Locked Loop (PLL).
- **THD filter** ensures output is clean and safe for residential use.
- **Smart grid comms** allow for demand response, remote monitoring, and dynamic load control.

---

## 🧪 Wiring Notes

- Use **6 AWG** DC cable with double insulation from capacitor array.
- Install **galvanic isolation** if connecting to residential load centers.
- Ground inverter chassis via **dedicated earth rod** — separate from tower discharge mesh.
- Optional: Integrate **CryoCore DC bus split** if excess energy is to be stored locally.

---

## 📈 Output Capacity (per tower)

| Scenario                     | Output (kWh/day) |
|-----------------------------|------------------|
| 2 lightning strikes/day     | 200–400 kWh      |
| 5 strikes/day               | 500–1000+ kWh    |
| Combined (3 towers, avg)    | 1500–3000+ kWh   |

> Enough to partially or fully supply 80–150 average German homes depending on energy profile and strike frequency.

---

## 📎 Compliance

This design adheres to:
- VDE-AR-N 4105 (Low Voltage Grid Integration, Germany)
- IEC 62109 (Inverter Safety)
- EN 50549 (Distributed Generation Standards)

---
