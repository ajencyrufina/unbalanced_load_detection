**⚡ Unbalanced Load Detection Using Simulink**

**📘 Project Overview**

This project presents the modeling and analysis of a three-phase electrical system to detect unbalanced load conditions using MATLAB/Simulink (Simscape Electrical).

Three-phase systems are widely used in power distribution due to their efficiency and ability to deliver constant power. However, load imbalance can cause:

Neutral current flow

Overheating of equipment

Voltage fluctuations

Increased power losses

Reduced system lifetime

This project demonstrates how unbalanced loads can be detected using phase current deviation and neutral current magnitude, along with a real-time visual lamp indicator.

**🎯 Objectives**

Design a three-phase electrical model in Simulink

Simulate both balanced and unbalanced load conditions

Measure phase voltages, phase currents, and neutral current

Detect load unbalance using measurement logic

Provide real-time visual indication using a dashboard lamp

**🛠️ Tools & Software Used**

MATLAB

Simulink

Simscape Electrical

**⚙️ System Components**

The model consists of the following major blocks:

1️⃣ Three-Phase Source

Symmetrical three-phase voltage supply

120° phase displacement

Typical line voltage: 400 V (configurable)

2️⃣ Three-Phase Load

Configurable RL load

Used to simulate:

Balanced condition (equal impedances)

Unbalanced condition (unequal impedances)

Example Unbalanced Load:

Phase A = 20 Ω  
Phase B = 25 Ω  
Phase C = 15 Ω  

3️⃣ Measurement Blocks

Voltage Measurement

Current Measurement

Neutral Current Sensor

4️⃣ Detection Subsystem

Unbalance detection is based on:

✔ Phase Current Deviation

If:

Imax − Imin >> 0

Then the system is unbalanced.

✔ Neutral Current

Balanced system → IN ≈ 0

Unbalanced system → IN > 0

Neutral current is the most reliable indicator.

5️⃣ Lamp Indicator (Dashboard)

🟢 Green → Balanced Load

🔴 Red → Unbalanced Load

Provides instant visual feedback during simulation.

6️⃣ Scopes

Phase Voltage Scope

Phase Current Scope

Neutral Current Scope

**📊 Simulation Results**

**✅ Balanced Load Condition**

Equal phase currents

120° phase shift maintained

Neutral current ≈ 0

Smooth sinusoidal waveforms

**❌ Unbalanced Load Condition**

Unequal phase currents

Noticeable neutral current

Voltage asymmetry

Clear waveform distortion

The neutral current amplitude increases as load imbalance increases.

**📈 Observations**

Neutral current is zero in perfectly balanced systems.

Neutral current increases significantly under unbalanced conditions.

Phase current deviation directly reflects load mismatch.

The lamp indicator provides an intuitive real-time status display.

**🏁 Results**

Successfully modeled a three-phase electrical system.

Clearly demonstrated balanced vs unbalanced behavior.

Verified neutral current as a reliable unbalance detection parameter.

Implemented real-time visual indication using a dashboard lamp.

**🔮 Future Scope**

Extension to fault detection systems

Integration with protection relays

Real-time monitoring using hardware implementation

IoT-based remote load monitoring

**📌 Conclusion**

This project effectively demonstrates how load imbalance in a three-phase system can be detected using Simulink. By analyzing phase current deviation and neutral current magnitude, unbalanced conditions can be accurately identified.

The model provides a simple, reliable, and user-friendly approach to studying power system imbalance.
