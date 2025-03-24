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

IOUT = IRef*(W/L)2 / (W/L)1  
# QUESTION  
 Design and analyze current mirror circuit as active load in amplifier circuit Vdd=1.8V  
 

 Let Power = 0.75mW , Itotal = P/Vdd = 0.75mW/1.8 = 0.416mA  
 Iref = 0.208mA  

A)1:1  
1) LENGTH = 180n  
DC ANALYSIS

![Image](https://github.com/user-attachments/assets/bc2930c2-cc08-4492-9a99-01c298ea3f5a  

TRANSIENT ANALYSIS  

![Image](https://github.com/user-attachments/assets/213ebda6-a42b-4107-91a0-0b7d839160bc)  

AC ANALYSIS  

![Image](https://github.com/user-attachments/assets/a5409300-ae7e-4d54-a515-b8cb62812494)  

The obtained gain = 28.559dB  
3dB gain = 25.559dB  
Frequency = 10MHz  
Bandwidth = 56.67MHz  

2) LENGTH = 500n

DC ANALYSIS  

![Image](https://github.com/user-attachments/assets/bbb1533d-324e-460d-bef3-e755cf8f93a0)  

TRANSIENT ANALYSIS  

![Image](https://github.com/user-attachments/assets/adfc666a-12f5-4ae7-8221-6a891261db54)  

AC ANALYSIS  

![Image](https://github.com/user-attachments/assets/47f49792-6f94-4ff0-8006-2f762d2f5485)  

The obtained gain = 38.044dB  
3dB gain = 35.044dB  
Frequency = 11.01MHz  
Bandwidth = 47.07MHz  

3)Length = 1u  

DC ANALYSIS  

![Image](https://github.com/user-attachments/assets/10439f63-0da4-41c3-ae6f-8a98cb64bff7)  

TRANSIENT ANALYSIS  

![Image](https://github.com/user-attachments/assets/9c6787e1-f335-4a33-b8a5-c9975448086c)  

AC ANALYSIS  

![Image](https://github.com/user-attachments/assets/a1c60449-faf8-4cf9-b95e-5709455b420f)  
The obtained gain = 40.327dB  
3dB gain = 37.327dB  
Frequency = 9.68MHz  
Bandwidth = 28.88MHz  

B) 1:2  

1) LENGTH = 180n

DC ANALYSIS  

![Image](https://github.com/user-attachments/assets/086470e7-6d27-4154-bac6-245d2b584583)  

TRANSIENT ANALYSIS  

![Image](https://github.com/user-attachments/assets/097eaa95-d069-4c57-8159-48ce4f71fb28)  

AC ANALYSIS  

![Image](https://github.com/user-attachments/assets/59029e13-5339-4c26-82fe-ffaacb2ba050)  

The obtained gain = 24.34dB  
3dB gain = 21.34dB  
Frequency = 9.74MHz  
Bandwidth = 40.30MHz  

2) LENGTH = 500n

DC ANALYSIS  

![Image](https://github.com/user-attachments/assets/1daa9dfd-6b98-42ab-bb74-098c9b68b0a3)  

TRANSIENT ANALYSIS  

![Image](https://github.com/user-attachments/assets/ab492f22-666d-4097-b3fa-9c7351fef1a8)  

AC ANALYSIS  

![Image](https://github.com/user-attachments/assets/469ad180-364d-41bf-bc8f-53e03d12b793)  

The obtained gain = 29.39dB  
3dB gain = 26.39dB  
Frequency = 9.31MHz  
Bandwidth = 118.80MHz  

3) LENGTH = 1u

DC ANALYSIS  

![Image](https://github.com/user-attachments/assets/8d3b1abf-bb13-4dbf-a980-f6cfc3d72a14)  

TRANSIENT ANALYSIS  

![Image](https://github.com/user-attachments/assets/ef44027f-8fe1-4efe-ad96-5b0a923c3ba1)  

AC ANALYSIS  
![Image](https://github.com/user-attachments/assets/57456a73-07f5-4d4f-b858-a71b421e5aee)  

The obtained gain = 14.77dB  
3dB gain = 11.77dB  
Frequency = 10MHz  
Bandwidth = 398.93MHz  







































 
 
   





   
   
   
