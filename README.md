# Hospital Ward and ICU Flow Simulation

## Overview
This project presents a discrete-event simulation model of patient flow across hospital acute wards and the Intensive Care Unit (ICU) using Simio. The model uses statistically fitted arrival processes and service-time distributions derived from real hospital data to analyze congestion, waiting times, bed utilization, and patient flow dynamics. The workflow includes:

- Data modeling: Statistical fitting of arrival and service-time distributions using real hospital data.
- Input modeling: Time-dependent arrivals and ward-specific service processes.
- System simulation: Discrete-event modeling of acute wards and ICU flow.
- Scenario analysis: Evaluation of operational policies including ward consolidation and diversion strategies.
- Optimization: Threshold-based diversion policy optimization using ranking-and-selection methods.

---

## Project Structure
data/ # Raw hospital arrival and service-time datasets
r_analysis/ # R scripts for statistical distribution fitting
simio_models/ # Simio simulation model files
notebooks/ # Data analysis and preprocessing notebooks
outputs/ # Simulation results, plots, and performance metrics
README.md # Project documentation
