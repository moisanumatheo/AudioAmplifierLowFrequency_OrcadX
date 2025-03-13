# AudioAmplifierLowFrequency_OrcadX
Audio Amplifier for low frequency project 


# Project Overview

  This project involves designing and implementing a low-frequency voltage amplifier with specific characteristics. The amplifier consists of multiple stages, ensuring signal amplification with high efficiency and minimal distortion. The design follows a series-parallel feedback structure to stabilize gain and enhance performance.

# Specifications

-Input Signal (ui): 60N [mV] → ui = 1380 [mV]
-Load Resistance (RL): 10N [Ω] → RL = 230 [Ω]
-Input Resistance (Ri): >150 kΩ
-Output Resistance (Ro): < 2.3 Ω
-Voltage Gain (Av): 10
-Operating Temperature Range: 0-70°C
-Power Supply Indicator: LED signaling power presence

# Block Diagram
-The amplifier consists of the following main blocks:
-Differential Stage - Enhances signal stability and noise rejection.
-Common-Emitter Stage - Provides significant voltage gain.
-Class AB Output Stage - Ensures efficiency and reduces crossover distortion.
-Current Source - Provides stable biasing.
-Current Mirror - Balances differential stage currents.
-Negative Feedback Network - Stabilizes gain and improves linearity.

# Circuit Design
- Differential Stage
Built using bipolar PNP transistors (Q1, Q2) with emitter degeneration resistors.
Maintains symmetry using a current mirror (Q3, Q4) to equalize currents.
Input: Non-inverting (Q1) receives the input signal, while inverting (Q2) gets feedback.
Enhances noise immunity and reduces common-mode signals.

- Common-Emitter Stage
Uses Q7 in a common-emitter configuration for additional voltage gain.
Includes Miller capacitance compensation to stabilize frequency response.
Class AB Output Stage
Push-pull configuration with NPN (Q10, Q11) and PNP (Q12, Q13) transistors.
Eliminates crossover distortion and improves efficiency over Class A and Class B.
Biasing diodes ensure proper transistor operation.

- Current Source & Mirror
Provides stable current through transistors Q5, Q8, and biasing diodes.
Maintains consistent operating conditions for amplification stages.

- Negative Feedback Network
Uses a voltage divider (R8, R9) to control gain and ensure stability.
Gain formula: Av = 1 + (R9 / R8) = 10.01

- Static Operating Point

The design ensures appropriate DC biasing across all stages for optimal performance.

# Conclusion

This low-frequency voltage amplifier design provides efficient signal amplification while maintaining stability and minimizing distortions. The use of negative feedback, current sources, and a class AB output stage makes it well-suited for applications requiring high fidelity and reliability.

# Author: Moisanu David-Matheo
# University: National University of Science and Technology Politehnica Bucharest
# Faculty: Electronics, Telecommunications, and Information Technology
# Year: 2024
