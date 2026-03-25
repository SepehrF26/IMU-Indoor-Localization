# IMU-based Indoor Localization (PDR System)

A Pedestrian Dead Reckoning (PDR) system designed for GPS-denied indoor environments, focusing on mitigating IMU sensor drift through probabilistic filtering.

## Technical Overview
This project implements a complete localization pipeline using a Raspberry Pi (Sense HAT) to process raw inertial data. The core challenge addressed is the accumulation of error (drift) in low-cost MEMS sensors.

### Key Implementation Details
* **Heading Estimation:** Kalman Filtering for sensor fusion of accelerometer and gyroscope data.
* **Position Correction:** Bayesian grid-based filtering and Particle Filtering to constrain motion models.
* **Motion Model:** Stride detection and step-length estimation algorithms optimized for real-time performance.

## Repository Contents
* `DFA_Report.ipynb`: Technical report containing mathematical derivations and Python implementation.
* `*.log`: Experimental data sessions (fast, slow, and sampled) for filter validation.

## Academic Context
Developed as part of the **Smart Systems Engineering** Master's program at Hanze University of Applied Sciences. This project demonstrates the application of probabilistic robotics and sensor fusion in embedded systems.