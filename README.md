\# IMU-based Indoor Localization (PDR System)



This project implements a \*\*Pedestrian Dead Reckoning (PDR)\*\* system designed for GPS-denied indoor environments. It processes raw IMU data (accelerometer and gyroscope) to track a user's position and orientation in real-time.



\## 🛠 Technical Highlights

\* \*\*Sensor Fusion:\*\* Implemented \*\*Kalman Filtering\*\* to combine accelerometer and gyroscope data for stable heading estimation.

\* \*\*Probabilistic Localization:\*\* Developed \*\*Bayesian grid-based filtering\*\* and \*\*Particle Filtering\*\* to mitigate cumulative sensor drift.

\* \*\*Hardware:\*\* Developed for the \*\*Raspberry Pi (Sense HAT)\*\*, focusing on efficient real-time data processing.

\* \*\*Feature Extraction:\*\* Includes stride detection and step-length estimation algorithms.



\## 📁 Repository Structure

\* `DFA\_Report.ipynb`: Full technical analysis, mathematical derivations, and visualization of results.

\* `\*.log`: Raw sensor data sessions (fast, slow, and sampled) used for testing the filters.



\## 🚀 How it Works

The system uses a motion model to predict the user's next position based on detected steps and heading. It then uses map-aware constraints and probabilistic filters to "correct" the position, significantly reducing the error compared to raw integration.

