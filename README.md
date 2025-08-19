<!-- SPDX-License-Identifier: ASYS-1.0 -->
# Astrava — Orbital Compute Cluster

**Status:** Concept → Architecture → Prototype  
**Scope:** Modular, laser-meshed, self-maintaining orbital supercomputer  
**Identity:** Astrava Systems — Cluster Division

---

## TL;DR
The Astrava Orbital Compute Cluster is a modular, hex-tiled constellation of self-powered compute modules designed to form a massively scalable, secure, and serviceable supercomputer in orbit. Each unit carries its own hexagon solar sail (power + structural frame) and a replaceable compute & laser core. Modules connect via high-bandwidth, per-edge laser links to form a resilient mesh. Robotic hubs perform maintenance and hot-swap of compute cores. The cluster is designed to be useful from the first module and to scale to thousands (and beyond) as launch capacity and resources grow.

---

## Why this project exists
- Earth-bound compute is energy-, cooling-, and space-limited.  
- Placing compute in orbit gives abundant solar energy, vacuum cooling, and linear physical scalability.  
- A modular, serviceable lattice reduces risk — failed compute cores are replaceable, and the network self-heals.  
- The Cluster is the strategic revenue engine and technical backbone for Astrava’s broader civilizational projects (AI compute, simulation, and orbital infrastructure).

---

## Core principles
1. **Modularity first** — every unit is useful standalone and plugs into the lattice.  
2. **Interface over internals** — standard Astrava-Bus interfaces (power & mechanical docking) decouple hardware generations.  
3. **Compute-dominant** — ~90–95% compute units; the remainder are power, comms, robot hubs, fabrication, or habitat attachments.  
4. **Optical data, power cable only** — all inter-module data transfers are laser optical; only power is cabled through the lattice.  
5. **Serviceability** — compute cores are hot-swappable; robot hubs perform repair and assembly.  
6. **Security & sovereignty** — hardware attestation, link-level crypto, and isolation domains by design.  
7. **Generation-aware** — Gen V1 (conventional accelerators) → Gen V2 (neuromorphic) migration path is supported.

---

## What this repo contains
```bash
Orbital_Compute_Cluster/
│
├── README.md # (this file)
├── LICENSE # ASYS-1.0 short license (see repo root)
│
├── 00_OVERVIEW/
│ ├── vision.md
│ ├── roadmap.md
│ └── key_principles.md
│
├── 01_ARCHITECTURE/
│ ├── system_design.md
│ ├── networking.md
│ ├── modules.md
│ └── attachment_and_station.md
│
├── 02_HARDWARE/
│ ├── compute_modules.md
│ ├── hex_sail.md
│ ├── comms_optical.md
│ ├── power_bus.md
│ └── edge_docking_interface.md
│
├── 03_SOFTWARE/
│ ├── cluster_management.md
│ ├── actuation_controller.md
│ └── AstravaOS_link.md
│
├── 04_OPERATIONS/
│ ├── launch_plan.md
│ ├── robot_ops.md
│ └── scaling.md
│
├── manifests/
│ └── module_manifest_example.yaml
│
├── visuals/ # diagrams, ASCII art, schematics
└── docs/
└── glossary.md
```

---

## Key architecture concepts (quick)
- **Frame vs Payload**  
  Each module has two logical parts:
  - **Frame (permanent):** solar sail + docking/power bus + mechanical hardpoints. Long-lived in orbit.
  - **Payload (replaceable):** compute & laser core — hot-swappable by robots.

- **Laser Mesh**  
  One optical transceiver per hex edge (up to 6). PAT (Pointing–Acquisition–Tracking) + WDM lanes allow multi-Gbps/Tbps per link. A low-rate RF fallback exists for safe bring-up only.

- **Astrava-Bus (power)**  
  Only power rails cross physical connections (hot-pluggable high-current blind-mate connectors with SSDs). All data is optical.

- **Robotic Hubs**  
  Small fraction of units that host 1–2 multi-joint manipulators. They assemble, replace, inspect, and rescue modules.

- **Fault tolerance & self-healing**  
  Mesh routing + robot-mediated physical replacement + per-node UPS and checkpointing make the cluster resilient to single or multi-node failures.

---

## Roadmap — highlights
1. **Phase 0 (Present)** — Architecture specs, AstravaOS demo integration, initial CAD + breadboards.  
2. **Phase 1 (1–3 years)** — Single-module prototype: hub + deployable hex sail + replaceable compute core. Launch pathfinder(s).  
3. **Phase 2 (3–6 years)** — Lattice formation: multiple modules link, cluster orchestration, petaflop→exaflop capability.  
4. **Phase 3 (6–10 years)** — Zettaflop target: mix in advanced power modules, comms backbone, begin neuromorphic testbeds.  
5. **Phase 4 (10+ years)** — Scale via asteroid-supplied materials; full civilization-scale infrastructure.

(See `00_OVERVIEW/roadmap.md` for full timeline and milestones.)

---

## Getting started — for engineers and contributors
1. Clone the repo:
   
   ```bash
   git clone git@github.com:astrava/Astrava-Cluster.git
   cd Astrava-Cluster
