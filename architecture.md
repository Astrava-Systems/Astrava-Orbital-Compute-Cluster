# Orbital Compute Cluster – Architecture

---

## Module Design
- **Shape**: Hexagonal “sail” modules for tiling and scalability.  
- **Example size**: ~25 m across (~400 m² surface area). *Note: size is an example and may change.*  
- **Internal layers**:  
  - Compute layer with stacked chip modules  
  - Power delivery layer  
  - Cooling & radiators  
  - Networking interconnects  

---

## Module Classes
1. **High-spec nuclear seed modules**
   - Deployed first: 6 units around a central nuclear reactor module  
   - Provides exaflop-scale compute rapidly  
   - Nuclear backbone ensures stable energy for AI training & critical workloads  

2. **Low-spec solar modules**
   - Scaled afterward in larger numbers  
   - Each delivers multiple petaflops  
   - Powered by solar arrays and optimized for efficiency  

*Compute performance numbers are indicative only and subject to refinement.*  

---

## Networking
- **Short-range interconnects** between adjacent modules for ultra-low latency.  
- **Laser communication** for inter-cluster networking.  
- **Redundancy**: Multiple paths for fault tolerance.  

---

## Deployment Strategy
- Launch in batches of ~20 modules per set using multiple rockets.  
- Initial focus: 7-module seed system (>1 exaflop).  
- Expansion: gradual build-out with solar modules.  

---

## Feasibility Notes
- Design emphasizes **cost efficiency** — avoiding overpriced “space-grade” components where not necessary.  
- Modular units enable repair, replacement, and upgrades.  
- Manufacturing scale is key to reducing per-unit cost over time.  
