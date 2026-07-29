# Drone_guidance_python_simulations
Python simulation for autonomous drone altitude stabilization and boat path tracking using closed-loop PID control and trajectory tracking algorithms.

# Autonomous Drone Guidance & Path Tracking Simulation

A Python-based simulation modeling autonomous trajectory control and path tracking mechanics for aerial vehicles and marine vehicles operating under environmental disturbances such as wind and water current.

---

## Project Objectives & Performance Metrics

The primary goal of this project is to tune closed-loop control systems to achieve stable target state tracking while satisfying four critical performance criteria:
1. **Faster Response:** Optimizing rise time to target setpoints under 1.0 second.
2. **Minimum Overshoot:** Mitigating extreme initial state excursions to prevent system crashes.
3. **Reduced Oscillation:** Accelerating settling time to stabilize system states smoothly.
4. **Better Disturbance Rejection:** Attenuating dynamic, random external noise injections (e.g., wind gusts, cross-current forces).

---

## Performance Visualizations

### 1. Altitude Stabilization (PID Control Tracking)
Optimized Proportional-Integral-Derivative parameters ($K_p = 5.50$, $K_i = 1.20$, $K_d = 4.00$) to achieve rigid altitude target stabilization at 10 meters. The closed-loop controller successfully rejects random wind gust vectors injected at the 6.0-second timestamp, maintaining steady-state bounds without divergent oscillations.


### 2. Autonomous Boat Path Tracking (Guidance Logic)
Implemented Cross-Track Error minimization constraints to bind vehicle trajectories cleanly onto parametric path matrices. Operating under configured ambient current vectors, the optimized parameters ($Gain = 1.50$, $Damping = 1.70$) force the actual path trajectory to lock perfectly onto the target sinusoidal path layout.



---

##  Environment & Technical Tooling
* **Programming Language:** Python 3 Core Runtime
* **Numerical Processing:** NumPy (Vector coordinate transforms and matrix evaluations)
* **Visualization Layer:** Matplotlib (High-fidelity telemetry plot generation)
* **Runtime Framework:** Google Collab Interactive Notebooks
