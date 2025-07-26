# Safety Guidelines – IX-Aus-Amerika-mit-Liebe

This document defines all **operational safety protocols** required for:
- Construction personnel
- Electrical engineers
- Coastal maintenance teams
- Emergency responders

All recommendations align with:
- **DIN VDE 0105-100** (operation of electrical installations)
- **IEC 61482-1-2** (arc flash protection)
- **ISO 12402** (marine access safety)
- **EN 50110** (live system maintenance)

---

## ⚠️ General Hazard Zones

| Zone             | Radius      | Risk Type                      |
|------------------|-------------|--------------------------------|
| Strike apex zone | ~3 meters above rod tip | Fatal electrical arc exposure |
| Coil resonance zone | ~6 meters from core (internal) | EM interference / static arc |
| Base transformer zone | 2–3 meters from pad | Inductive shock from output surge |
| Ground mesh perimeter | 10m radius (during strike) | Induced voltage transients |

---

## 👷 Personal Protective Equipment (PPE)

| Area            | Required PPE Standard |
|-----------------|------------------------|
| Inside tower    | Cat 3 arc suit (IEC 61482-2) + EM shielding liner |
| Maintenance shaft | Full harness, IP68 helmet w/ RF attenuation |
| Base electronics | HV-insulated gloves (Class 4 IEC 60903) |
| Exterior surface (cleaning) | Marine-rated static discharge boots + tether rigging |

---

## ⚡ Lightning Hazard Protocol

| Condition                    | Action |
|-----------------------------|--------|
| Storm within 10km radius    | All access locked, system sealed |
| Lightning strike detected   | 15-minute minimum post-strike cooldown |
| EM field spike (>2 mT)      | Evacuate coil chamber immediately |
| Grid blackout + active storm | Remain clear of tower for 1 hour minimum |

Field crews should **never occupy the tower during electrical storm activity** — even in standby mode, capacitors may auto-discharge with lethal voltage.

---

## 🔧 Maintenance Access Protocols

### Entry Conditions:
- Confirm **isolation switch is open**
- Check **capacitor bank voltage < 60V**
- Verify **ground rod continuity** via megohmmeter
- Ventilation must run **3 minutes prior to human entry**

### Ladder Access:
- Harness attachment at every rung transition
- Use marine-rated tethered tool system
- Only one technician inside internal shaft at a time

---

## 🔌 Electrical Service Rules

| Task | Rule |
|------|------|
| Capacitor bank swap | Use 2-person lockout-tagout, discharge via resistor |
| Inverter service | Ground-check and isolate grid tie relay before access |
| Rectifier replacement | Confirm strike counter shows 0 for current month |
| Sensor swap or logger access | Remove coil shielding cage, reattach within 1 hour |

---

## 🌊 Marine & Coastal Safety

| Condition | Required Action |
|-----------|------------------|
| High tide flood risk | Remote shutoff of all outputs |
| Submersion event (e.g. rogue wave) | Disable all active electronics, initiate dry-out protocol |
| Barnacle or fouling cleaning | Only with tower power fully disconnected and tested |
| Mooring chain tension drop | Re-balance tower footing via ballast tanks or crane reset |

---

## 🔥 Arc Flash Boundaries

- Arc incident energy near rod tip: **>40 cal/cm²**
- Arc boundary: **~4.2 meters horizontal from rod base**
- Use Class 4+ PPE within that boundary **even if not energized**

Never bypass spark gaps or arc diverters during inspection — they remain charged even when isolated.

---

## ✅ Summary

**This is not a tower to take lightly.**  
It is a live energy organ, conducting hundreds of thousands of amps per event.

But with the proper procedures:
- ⚙️ It can be safely maintained
- ⚡ Repaired under live-grid edge protocols
- 🌩️ Endure strike after strike without failure

Safety is not optional. It is how this machine earns its place among your infrastructure.

— Bryce Wooster
