🚢 Operation Abyssal Echo
Acoustic Forensic Reconstruction System
📌 Overview

Operation Abyssal Echo is an advanced acoustic signal processing system designed to reconstruct the trajectory of a submerged vessel using underwater sensor data.

The system performs forensic analysis of acoustic intercepts, applying physics-based corrections and signal filtering to estimate accurate positions in a complex deep-sea environment.

🎯 Objectives
Analyze raw acoustic signals from multiple sensor stations
Filter primary signals from echoes/noise
Correct signal timing using clock drift interpolation
Apply environmental corrections using the Mackenzie equation
Perform 3D trilateration to reconstruct vessel trajectory
Visualize results using interactive dashboards
⚙️ Features
🔊 Acoustic Signal Processing
Groups signals by packet/event
Identifies primary signals based on intensity
Filters echo/ghost signals
🌊 Environmental Correction
Uses temperature, salinity, and pressure data
Computes sound velocity using Mackenzie equation
⏱️ Time Synchronization
Corrects clock drift using sync pulse data
Improves accuracy of time-of-arrival calculations
📍 Position Reconstruction
Uses multi-sensor trilateration
Generates accurate 3D coordinates
📊 Visualization Dashboard
3D trajectory reconstruction (corrected vs raw)
2D overhead tracking
Acoustic waterfall plot
Real-time HUD (speed, depth, sound velocity)
Mission statistics panel
🛡️ Robust System Design
Handles missing or noisy data
Prevents runtime crashes (safe validation added)
Works with real-world datasets
🧠 Core Technologies Used
JavaScript (Vanilla JS)
Plotly.js – Data visualization
PapaParse – CSV parsing
Acoustic Signal Processing Concepts
Physics-based Modeling (Ocean Acoustics)
🧮 Key Algorithms
1. Mackenzie Equation (Sound Speed)

Used to compute speed of sound underwater based on:

Temperature
Salinity
Depth
2. Clock Drift Interpolation
Synchronizes timestamps across sensor network
Uses reference sync pulses
3. Signal Filtering
Selects highest intensity signal per station
Removes echoes and noise
4. Trilateration (3D Positioning)
Uses distances from multiple sensors
Computes vessel coordinates in 3D space
📁 Input Files Required

Upload the following CSV files:

vessel_specifications.csv
sensor_network_registry.csv
buoy_sync_pulses.csv
environmental_log.csv
vessel_engine_telemetry.csv
acoustic_telemetry_raw.csv
▶️ How to Run
Open the HTML file in a browser
Upload all 6 required CSV files
Click “DECRYPT & PROCESS INTEL”
View reconstructed trajectory and analytics
📈 Output
Reconstructed 3D trajectory
Signal classification (primary vs echo)
Depth and speed estimates
Environmental corrections
CSV export of trajectory data
🐞 Error Handling Improvements

This version includes fixes for:

❌ Undefined sensor references
❌ Invalid trilateration inputs
❌ Plotly rendering crashes (anchor error)
❌ Missing environmental data

✔ Ensures stable execution even with imperfect datasets

🚀 Applications
Submarine tracking
Naval surveillance systems
Oceanographic research
Acoustic signal intelligence
Defense analytics
🎓 Academic Relevance

This project demonstrates concepts from:

Data Structures & Algorithms
Signal Processing
Computational Geometry
Physics-based Modeling
Data Visualization
👨‍💻 Author

Ritesh Khotale
Computer Engineering Student

📌 Future Improvements
🤖 AI-based echo classification
📡 Real-time IoT integration
🧠 Kalman filtering for trajectory smoothing
🌐 Web-based live dashboard