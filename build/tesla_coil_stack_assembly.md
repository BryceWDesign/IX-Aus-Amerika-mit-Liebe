# 🛠️ Tesla Coil Stack Assembly + ZeroCell Integration (Per Tower)

This document provides complete build instructions for assembling the internal coil chamber of each lightning-harvesting tower, including spark gap positioning, ZeroCell modules, and full Gankyil-wound Tesla array logic.

---

## ⚙️ Materials Required

| Component                     | Quantity | Notes |
|------------------------------|----------|-------|
| 6 AWG Copper Magnet Wire     | 1500 m   | For bifilar and triplet winding |
| PVC Coil Forms (150mm dia)   | 6        | Heat-resistant polymer tubing |
| ZeroCell Ferrite Cores       | 3        | One per coil triplet |
| High-Speed Spark Gap Switches| 3        | Modular, humidity-rated |
| Insulating Enclosure Resin   | 10 L     | Marine-grade epoxy |
| Tungsten Ground Rods         | 3        | Lightning inlet rods |
| Kapton Tape (100m)           | 2 rolls  | High-voltage insulation wrap |
| Structural Mounting Rings    | 6        | Non-conductive polymer clamps |
| Ground Mesh Cable (10mm²)    | 100 m    | For tower base dissipation mesh |

---

## 🧱 Coil Construction Process

### 1. **Form Preparation**
- Cut PVC tube to 1.2m lengths.
- Sand outer layer and apply dielectric resin primer.
- Cure overnight.

### 2. **Bifilar Winding**
- Wind each form using bifilar method (two wires wound together).
- Target: 369 turns for each pair, spaced evenly.
- Secure ends using Kapton and terminate into ceramic junctions.

### 3. **Triplet Stack Configuration**
- Vertically mount 3 bifilar coils using isolation rings.
- Insert ZeroCell core between middle and bottom coils.
- Gankyil pattern achieved by twisting current direction on 2nd coil.

---

## 🔩 Spark Gap Placement

- Position tungsten spark gap 5 cm downstream of top coil output.
- Adjust gap to ~2mm default; tune based on humidity (auto-tunable preferred).
- Spark gap exhaust must have forced air or passive ceramic venting.

---

## 💠 ZeroCell Embedding

- Insert EM-damped ferrite composite (graphite/quartz/ferrite) into center buffering well.
- Coil around this core with 369 μm copper braid (Tesla harmonic sleeve).
- Lock into place using cryogenic thermal epoxy if needed.

---

## ⚡ Final Assembly

- Each coil triplet becomes one harmonic pillar inside the “shot glass” tower.
- Mount coils using vibration-damped brackets inside insulated cage.
- Ensure common ground return path is bonded at tower base with 5m-deep rod mesh.

---

## ✅ Final Verification Checklist

- [ ] Coil winding complete with 369 turns/pair × 3 stacks
- [ ] Spark gaps calibrated and sealed
- [ ] ZeroCell modules securely mounted and bonded
- [ ] Dielectric clearance >10mm throughout
- [ ] All joints torqued and weatherproofed

---
