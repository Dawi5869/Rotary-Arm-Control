# 🤖 Rotary Arm Control – PD Control System for Rigid Arm

<p align="center">
  <img src="ASEN 2803 Lab 3 (1).png" alt="HappyCam Product Photo" width="850"/>
</p>

## ✨ Overview
This was a lab project for our Dynamics & Controls course (ASEN 2803), where our group designed and implemented a **proportional-derivative (PD) controller** for a rigid rotary arm system. The goal was to model the arm’s dynamics, design a controller to meet performance specs (under 20% overshoot, settling time < 1s), simulate the response in MATLAB, and then validate the design on real hardware using NI myRIO.

We worked through multiple stages including deriving transfer functions from system dynamics, tuning gains in MATLAB, and physically verifying performance against theory using LabVIEW-based hardware-in-the-loop systems.

---

## 👨‍💻 Personal Contributions

- **Experimental Testing**
  - Used the NI myRIO interface to test gain sets on a real rotary arm rig.
  - Collected and plotted system response data in MATLAB.
  - Compared theoretical model behavior with experimental outcomes and Simulink simulations.
  - Observed differences in system performance due to real-world factors like natural damping and friction.
  - Create a functional block diagram to showcase our understanding of the integrated system.

- **Performance Tuning**
  - Designed and validated a controller with:
    - **Proportional Gain (K₁):** 19.9  
    - **Derivative Gain (K₃):** 1.38  
  - Achieved target performance of <20% overshoot and <1 second settling time in both MATLAB and hardware (on Arm 1).

- **Hardware Debugging**
  - Investigated discrepancies between arms, identifying that Arm 2 had lower friction and thus higher overshoot.
  - Analyzed the impact of actuator saturation (10V limit) on the fidelity of the system’s response versus simulation.

---

## 🛠 Tools & Technologies
- **MATLAB + Control Systems Toolbox** – Transfer function modeling, simulation, and performance analysis.
- **NI myRIO** – Used for real-time hardware implementation of control gains and system feedback.
- **Simulink** – Provided benchmark simulations with modeled physical damping for comparison.
- **LabVIEW** – Used via the VI interface to configure gains and log voltage/angular data during tests.

---

## 📊 Key Results
- **Simulation vs Hardware:**
  - MATLAB predicted higher overshoot due to lack of natural damping modeling.
  - Real-world data showed improved settling time and slightly lower overshoot (especially on Arm 1) due to friction/damping.
- **Requirement Fulfillment:**
  - Final controller met performance goals in both simulation and hardware for Arm 1.
  - Arm 2 exceeded overshoot specs due to lower resistance and unmodeled voltage spikes.

---

## 📬 Contact
Reach out at dawi5869@colorado.edu
