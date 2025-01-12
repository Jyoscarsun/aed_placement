# Optimizing AED Placement in Scotland

This repository contains the codebase for optimizing the placement of Automated External Defibrillators (AEDs) based on historical cardiac arrest data and geographic constraints. The project leverages the HiGHS optimization library to determine optimal AED placement to maximize coverage within a given region.

## Project Overview

The goal of this project is to enhance emergency response by strategically placing AEDs across Scotland, using past cardiac arrest data to inform optimal placement. The optimization process involves:

- Translating cardiac arrest and AED location data into a compressed sparse matrix (CSM) representation for efficient computation.
- Implementing constraints and objective functions to maximize coverage while considering geographic and operational constraints.
- Running optimization models using the HiGHS library, developed by researchers at the University of Edinburgh.

## Features

- Calculation of distances between cardiac arrest locations and potential AED placement sites using the Haversine formula.
- Filtering of potential AED locations to remove redundant placements and improve computational efficiency.
- Flexible setup to explore multiple iterations with varying numbers of AEDs for different geographic regions.

## Requirements

- Python 3.8 or higher
- Required Python libraries:
  - `numpy`
  - `pandas`
  - `highspy`
