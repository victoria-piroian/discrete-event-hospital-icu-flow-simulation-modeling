# Hospital Ward and ICU Flow Simulation

## Overview
This project presents a discrete-event simulation model of patient flow across hospital acute wards and the Intensive Care Unit (ICU) using Simio. The model uses statistically fitted arrival processes and service-time distributions derived from real hospital data to analyze congestion, waiting times, bed utilization, and patient flow dynamics. The workflow includes:

- Data modeling: Statistical fitting of arrival and service-time distributions using real hospital data.
- Input modeling: Time-dependent arrivals and ward-specific service processes.
- System simulation: Discrete-event modeling of acute wards and ICU flow.
- Scenario analysis: Evaluation of operational policies including ward consolidation and diversion strategies.
- Optimization: Threshold-based diversion policy optimization using ranking-and-selection methods.

---

## Key Features

### Input Modeling
- Time-dependent arrival modeling using hourly rate tables
- Empirical estimation of ward-routing probabilities
- Distribution fitting (Normal, Lognormal, Gamma, Weibull, Exponential)
- QQ-plot validation and goodness-of-fit testing
- Parameterized distributions implemented in Simio

### Simulation Model
- Four acute wards: Internal Medicine, Musculoskeletal, Neurology, Cardiovascular
- ICU with limited bed capacity
- Capacity constraints and queueing dynamics
- Bed blocking behavior
- ICU overflow and diversion logic
- Probabilistic patient routing and crash modeling
- Mortality and discharge pathways

### Scenario Analysis
- **Base Model:** Realistic hospital operations with capacity constraints
- **Ward Consolidation Scenario:** Merged acute wards into a single generalized ward
- **Diversion Policy Scenario:** Threshold-based diversion of arrivals under congestion
- Ranking-and-selection optimization experiment
- Objective function optimization:
  
  **Objective = Average Queue Length + 120 × Proportion of Diverted Arrivals**

### Performance Metrics
- Average waiting time per ward
- Queue lengths
- Bed utilization rates
- ICU congestion levels
- Bed blocking frequency
- Diversion rates
- External patient rejection rates
- System throughput

---

## Evaluation
- Comparative scenario performance analysis
- Congestion and utilization metrics
- Queue stability assessment
- Optimization performance benchmarking
- Bottleneck identification
- Policy impact quantification

---

## Usage
1. Clone the repository:
```bash
git clone <repo-url>
```
2. Run statistical modeling in R:
- Fit arrival and service-time distributions
- Generate distribution parameters

3. Open Simio models:
- Load fitted distributions
- Run base model simulation
- Execute scenario experiments
- Run optimization experiments

4. Analyze outputs:
- Review congestion metrics
- Compare scenario performance
- Evaluate diversion policy effectiveness
- Generate plots and reports from outputs folder

---

## Goals
- Model realistic hospital patient flow dynamics
- Identify operational bottlenecks
- Evaluate structural policy changes (ward consolidation)
- Optimize diversion strategies
- Support data-driven hospital operations planning
- Demonstrate simulation as a decision-support tool for healthcare systems

---

## Author

Victoria Piroian

University of Toronto

Faculty of Applied Science & Engineering, 2022
