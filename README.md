# Projektidee – Therapieplätze & Wartezeiten (Monte-Carlo-Modell)
# Therapy Waiting Time Simulation using SimPy

## Project Overview
This repository contains a **discrete-event simulation model** for analyzing  
**waiting times and capacity constraints in a psychotherapeutic care system**.

The simulation is implemented using **SimPy** and models:
- patient arrivals with growing demand
- limited therapy capacity (resources)
- patients who drop out before starting therapy
- realistic therapy durations
- waiting queues and waiting times

The main objective is to study the impact of **undersupply** on waiting times over multiple years.
he project analyzes **waiting times and capacity constraints in a healthcare system**, focusing on therapy slots, patient arrivals, and demand growth.  
---

## Repository Structure
 MONTECARLO_project
┣  data    
┣  environment    # Environment configuration (e.g. virtual env, setup files)       
┣  notebooks      # Jupyter notebooks for analysis and exploration
┃ ┗ Final_01.ipynb
┣  README_files/libs   # Assets for rendered README (HTML support files)
┣  reports
┃ ┗  ABOUTME.txt  # Project description / report notes                     
┣  README.md      # Main project documentation
┣  README.html    
┗  .gitignore

---

## Simulation Model (Summary)

### Objective
To evaluate how **capacity limitations and demand growth** affect:
- waiting times
- system congestion
- risk of extreme delays

in a therapy-based healthcare system.

---

### Time Model
- **Time unit:** weeks  
- **Simulation horizon:** 3 years  
- **Therapy duration:** 30 weeks (adjusted for working weeks) 
- **Warm-up phase:** system starts fully occupied to avoid initial bias

---

### Demand Model
- Patient arrivals follow a **Poisson process**
- Only a fraction of arrivals actually start therapy
- Demand increases continuously over time (growth rate)

---

### Capacity Model
- Therapy capacity is modeled as a **limited resource**
- Capacity is derived from:
  - theoretical staff availability
  - break-even calculations
  - scenario-specific efficiency adjustments
- Undersupply scenarios intentionally create waiting queues

---

### Output Metrics
The simulation records and evaluates:
- number of patients starting therapy
- average waiting time
- median waiting time
- 90th percentile waiting time
- maximum waiting time

---

## Notebooks

`Final_01.ipynb` represents the consolidated final analysis.

---

## Installation & Usage

### Requirements
- Python ≥ 3.9

### Install dependencies
```bash
pip install numpy simpy jupyter
