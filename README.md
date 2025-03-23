# CURRENT-MIRROR  
A current mirror circuit is a fundamental building block in analog electronics designed to replicate or "mirror" a reference current from one part of the circuit to another with high accuracy. It leverages matched transistor characteristics to ensure the output current closely follows the input current, even under varying conditions.  
# Core Components and Operation  
1. Basic Configuration:
   
   Uses two transistors (BJT or MOSFET), where one acts as the reference (input) and the other as the mirror (output).
   
   The reference transistor is often diode-connected (base/collector shorted in BJTs, gate/drain shorted in MOSFETs) to set the control voltage.
2. Current Copying:
   
   The reference current is forced through the diode-connected transistor, establishing a specific VGS.
   
   This voltage is applied to the mirror transistor, inducing a similar current in its output branch, assuming matched device parameters.
3. Scaling Currents:
   By adjusting the physical size f the mirror transistor relative to the reference, the output current can be scaled.

# Key Characteristics  
Accuracy: Depends on transistor matching and process uniformity. Integrated circuits (ICs) achieve high precision due to fabrication proximity.  

Output Impedance: High output impedance is desirable for ideal current sources. Techniques like cascode or Wilson mirrors improve this by reducing Early effect (BJT) or channel-length modulation (MOSFET) impacts.  

Temperature Stability: VGS variations with temperature can affect performance, often mitigated through biasing techniques.  

# Applications  
Biasing: Provides stable bias currents for amplifiers and other analog blocks.  
Active Loads: Replaces resistors in differential pairs to enhance voltage gain.  
Current Scaling: Generates multiple proportional currents from a single reference.  
Signal Processing: Used in current-mode circuits like current amplifiers or DACs.  

Circuit Diagram  

![Image](https://github.com/user-attachments/assets/c28085ab-1743-4b78-aad1-d5dd31c3ec9c)  





   
   
   
