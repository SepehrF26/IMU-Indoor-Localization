# 📍 IMU-based Indoor Localization (PDR System)

This project implements a **Pedestrian Dead Reckoning (PDR)** system designed for GPS-denied indoor environments. It processes raw IMU data to track a user's position and orientation in real-time.

---

### 🚀 Key Features
* ⚖️ **Sensor Fusion:** Uses **Kalman Filtering** to combine accelerometer and gyroscope data for stable heading estimation.
* 🎲 **Probabilistic Localization:** Implements **Bayesian Grid-based Filtering** and **Particle Filtering** to reduce cumulative sensor drift.
* 👣 **Motion Modeling:** Includes custom algorithms for stride detection and step-length estimation.
* 📟 **Embedded Integration:** Optimized for the **Raspberry Pi (Sense HAT)** for real-time processing.

---

### 🛠 Technical Architecture
The system follows a standard probabilistic robotics pipeline:
1. **Prediction:** Motion model predicts the next state based on IMU data.
2. **Correction:** Bayesian/Particle filters use map constraints to correct position.
3. **Filtering:** Kalman Filter smoothes the heading to prevent "spinning" errors.


---

### 📂 File Guide
* 📓 **DFA_Report.ipynb:** The main technical report containing mathematical derivations and Python implementation.
* 📊 **bayes_session_*.log:** Data logs used for testing the Bayesian grid-based filter.
* 🧬 **particle_session_*.log:** Data logs used for testing the Particle filter.

---

### 🎓 Academic Context
Developed as part of the **Smart Systems Engineering** Master's program. This project demonstrates the mitigation of IMU drift through advanced probabilistic methods.