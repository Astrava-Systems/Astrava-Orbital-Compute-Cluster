# Conceptual Design – Orbital Compute Cluster

This document outlines a preliminary side-view layout of the orbital compute cluster. It illustrates the relationship between the central reactor, compute modules, and solar panel array.

---

## ASCII Layout – Side View (Not to Scale)

                            ^
                            |
                            |  (Central Spine)
                            |
        +---------------------------------------------+
        |             [Nuclear Reactor]               |
        +---------------------------------------------+
                            |
                            |
                    (Power, Data, Cooling)
                            |
                     +--------------+
                     | Compute Ring |
                     +--------------+
                            |
                            |
              (Radiator Corridor / Shadow Zone)
                            |
                            v
                 ~~~ Solar Panels Array ~~~

Key:
- [Nuclear Reactor] supplies primary power to the compute modules.
- Central Spine routes power and cooling to the Compute Ring.
- Compute Ring is composed of modules arranged in a circular pattern.
- Solar Panels provide:
    • Backup power
    • Radiative cooling
    • Sunshade (reduces direct solar heating on Compute Ring)

Notes:
- Orientation assumes the sun is on the bottom (panels casting shadow upward).
- Layout is modular — allows phased expansion and orbital maintenance.

---

## Description

### 🧠 Compute Module Ring
- Arranged in a **circular formation** around the central spine.
- Each module is self-contained and stackable.
- Designed for **thermal dissipation**, **autonomous diagnostics**, and **hot-swappable upgrades**.
- The ring structure allows **uniform exposure to space for radiative cooling** and optimal power distribution.

### ⚛️ Nuclear Reactor
- Mounted at the top of the spine.
- Primary power source for the cluster.
- Thermally and electromagnetically isolated from sensitive compute systems.
- Includes multi-layer shielding for radiation containment and safety.

### ☀️ Solar Panels
- Located on the **underside** of the cluster.
- Serve two roles:
  1. **Supplemental power** supply.
  2. **Shadow shield** — the panels block direct sunlight from the compute ring, reducing heat load and simplifying cooling infrastructure.

### 🛰 Central Spine
- A **rigid truss** running vertically through the station.
- Hosts power conduits, cooling lines, and structural mount points.
- Enables **robotic servicing**, stabilization systems, and future expansion.

---

## Design Objectives

- **Heat Management**: Reactor and compute modules are spaced to prevent thermal interference. Sun-facing components are kept minimal.
- **Shielding**: Solar panels double as radiation shields from solar wind and micrometeoroids.
- **Modularity**: Every component can be replaced, expanded, or serviced independently.
- **Safety**: High-voltage and radioactive components are isolated from sensitive equipment.
- **Longevity**: The cluster is designed for a **15+ year lifecycle** with modular upgrade cycles every 3–5 years.

---

## Notes

- This is a **conceptual layout** for phase 1. Real-world orbital dynamics, mass distribution, and redundancy systems will further influence the final configuration.
- Future versions may include **spin-based artificial gravity modules**, **docking ports**, and **orbital tugs** for positioning.

---

## Visuals

> [Placeholder] 3D CAD schematics and rendered diagrams will be added in the `/visuals/` folder as development progresses.