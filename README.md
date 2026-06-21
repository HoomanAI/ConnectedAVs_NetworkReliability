## Reliability-Aware Routing for Connected Autonomous Vehicles in Post-Disaster Emergency Response

### Overview

A reliability-aware routing framework for Connected Autonomous Vehicles (CAVs) in post-disaster emergency response. The project models the impact of V2X communication network degradation on routing performance using a reliability-adjusted traffic model, fuzzy time windows, and multi-objective optimization to improve patient service quality, travel efficiency, and network resilience.

The proposed approach integrates:

- Connected Autonomous Vehicle (CAV) routing
- Vehicle Routing Problem with Fuzzy Time Windows (VRPTW-FTW)
- Network reliability modeling
- Time-Dependent Bureau of Public Roads (TD-BPR) traffic congestion model
- Multi-objective optimization
- Quantum-Inspired Genetic Algorithm (QiGA)

The framework is designed to support emergency medical operations where rapid response, service quality, and route reliability are critical under disrupted road and communication networks.

---

## Key Features

- Reliability-aware emergency vehicle routing
- Unified cyber-physical infrastructure degradation model
- Fuzzy time windows for patient service satisfaction
- Time-dependent traffic congestion modeling
- Multi-objective optimization framework
- Priority-based patient triage handling
- Route reliability maximization
- Service coverage optimization
- Quantum-inspired evolutionary optimization

---

## Problem Description

Following a disaster, transportation and communication infrastructures often experience partial failures. These disruptions reduce road capacity, degrade V2X connectivity, and increase emergency medical demand.

This project addresses the routing of autonomous emergency vehicles tasked with serving patients across multiple triage levels while considering:

- Travel time uncertainty
- Traffic congestion
- Infrastructure reliability
- Patient service quality
- Emergency response priorities

The framework models road and communication degradation using a unified reliability coefficient that simultaneously affects:

- Arc feasibility
- Effective road capacity
- Route reliability

---

## Objectives

The optimization framework simultaneously:

1. **Minimizes patient dissatisfaction**
   - Fuzzy time-window violations weighted by triage priority.

2. **Maximizes patient service coverage**
   - Prioritizes critical and urgent patients.

3. **Maximizes route reliability**
   - Prefers routes traversing highly reliable infrastructure.

---

## Traffic Model

The framework employs a Time-Dependent Bureau of Public Roads (TD-BPR) model:

\[
t_{ij}(p)=t_{ij}^{0}\left[1+\alpha\left(\frac{V_{ij}(p)}{C_{ij}^{0}\phi_{ij}}\right)^\beta\right]
\]

where:

- \(t_{ij}^{0}\) = free-flow travel time
- \(V_{ij}(p)\) = traffic volume during period \(p\)
- \(C_{ij}^{0}\) = nominal road capacity
- \(\phi_{ij}\) = infrastructure reliability
- \(\alpha = 0.15\)
- \(\beta = 4\)

This formulation captures both congestion and disaster-induced capacity degradation.

---

## Methodology

The proposed solution combines:

- Multi-objective optimization
- Reliability-constrained routing
- Fuzzy service quality modeling
- Quantum-Inspired Genetic Algorithm (QiGA)

QiGA is enhanced with a reliability-feasibility repair operator that ensures generated routes satisfy minimum reliability requirements.

---

## Repository Structure

```text
├── data/
│   ├── network/
│   ├── traffic/
│   └── reliability/
│
├── models/
│   ├── optimization/
│   ├── traffic/
│   └── reliability/
│
├── algorithms/
│   ├── qiga/
│   ├── nsga2/
│   └── moead/
│
├── experiments/
│
├── results/
│
├── figures/
│
└── README.md
```

---

## Research Contributions

- Reliability-adjusted TD-BPR traffic model
- Unified cyber-physical reliability representation
- Multi-objective CAV emergency routing formulation
- Fuzzy triage-aware service quality model
- Reliability-constrained QiGA optimization framework
- Analysis of service quality degradation under network failures

---

## Potential Applications

- Disaster response logistics
- Autonomous ambulance dispatching
- Emergency medical services
- Smart city resilience planning
- Humanitarian logistics
- Connected vehicle networks

---

## Citation

If you use this repository in your research, please cite the associated publication once available.

```bibtex
@article{cav_vrptw_nr,
  title={Reliability-Aware Routing for Connected Autonomous Vehicles in Post-Disaster Emergency Response},
  author={Razavi, Hooman and Co-authors},
  journal={Under Review},
  year={2026}
}
```

---

## License

This project is released under the MIT License.

---

## Contact

Hooman Razavi

Faculty of Engineering  
Tecnológico de Monterrey  
University of Ottawa
