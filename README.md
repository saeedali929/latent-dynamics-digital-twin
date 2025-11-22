Latent Space Dynamics: A Digital Twin for Embedded Systems

1. Project Abstract

This project demonstrates a Physics-Informed Machine Learning (PIML) approach to anomaly detection in resource-constrained embedded systems (Raspberry Pi).

Unlike traditional monitoring that relies on static thresholds (e.g., Temp > 55°C), this architecture identifies Topological Violations in the system's phase space. It posits that a healthy cyber-physical system is constrained to a low-dimensional Manifold determined by its internal physics (e.g., Thermodynamics, Ohm's Law, and Scheduler Logic).

2. The Architecture

The system operates on a Dual-Agent model to prove the Manifold Hypothesis:

The Actuator (The "Hidden Hand"): A custom kernel script (sine_cpu_load.py) that uses Pulse Width Modulation (PWM) on CPU cycles to force the system into a known, rhythmic latent state.

The Observer (The "Shadow Reader"): A real-time ingestion pipeline (manifold_visualizer.py) that projects high-dimensional sensor data (CPU_Load, Frequency, Temperature) into a 3D Phase Space.

3. Usage

A. Installation

pip install psutil matplotlib numpy


B. Run the Experiment

Terminal 1 (Start Physics): python sine_cpu_load.py
Terminal 2 (Start Twin): python manifold_visualizer.py

4. Relevance to Industrial Applications

While demonstrated on a Raspberry Pi, this "Latent Space Extraction" methodology is hardware-agnostic. It is directly applicable to Predictive Maintenance (detecting drift in mechanical coupling) and Sensor Fusion (distinguishing sensor noise from system failure).
