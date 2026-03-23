\# Solar Forecasting-Informed Grid Decisions for Weak-Grid Mini-Grids



\## Objective

This project evaluates how solar forecast uncertainty affects operational decisions in weak-grid and mini-grid systems.



The focus is not only forecast accuracy, but how that uncertainty changes battery dispatch, reliability outcomes, and the tradeoff between conservative operation and energy efficiency.



\## Core Question



Given forecast uncertainty, what should an operator do differently?



\## Purpose



Phase 3 translates:



forecast error → dispatch choice → reliability consequence → engineering decision



The focus is not on forecasting model internals.  

It is on decision policies, tradeoffs, and operator-facing conclusions.



\## System Context



This repository reuses the Phase 2 mini-grid context:



\- solar PV generation

\- battery storage

\- peri-urban load profile



and evaluates alternative dispatch policies under uncertainty.



\## What This Repository Tests



The repository compares deterministic operating policies such as:



\- baseline dispatch

\- evening reserve dispatch

\- forecast-margin dispatch



and evaluates their consequences in terms of:



\- unserved energy

\- loss-of-load hours

\- curtailment

\- battery stress

\- policy tradeoffs



\## Structure



```text

data/                  processed Phase 2 handoff and documentation

src/                   policy, scenario, metrics, and sensitivity logic

notebooks/             execution workflow and visual analysis

reports/               final decision-oriented summary

