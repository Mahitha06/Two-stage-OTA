# Two-stage-OTA
This project involves the hand-design, simulation, and analysis of a two-stage OTA using CMOS technology. It was developed as part of a classroom assignment for the Analog Circuits course at IIT Guwahati, with specifications requiring a DC gain ≥ 40 dB and implementation of a non-inverting amplifier with gain = 2.  
## OBJECTIVE:
  *** To design a two-stage operational transconductance amplifier (OTA) in TSMC180nm CMOS technology<br/>
  *** Ensure a minimum DC gain of 40 dB.<br/>
  *** Use the OTA in a non-inverting amplifier configuration with closed-loop gain = 2.
## Technologies & Tools used:
*LTspice for circuit simulation<br/>
*and calculations for transistor sizing and biasing<br/>
*MOSFET small-signal analysis.<br/>
## Design Overview:
### Stage-1:Differential Amplifier with Current Mirror Load
Differential input applied to M1 and M2 (NMOS).<br/>
Gate voltages:<br/>
Vcm + Vd/2 and Vcm - Vd/2 to isolate the differential mode and suppress common-mode.<br/>
Output voltage is the difference of drain voltages of M1 and M2.<br/>
Current mirror (M3, M4 – PMOS) used as active load.<br/>



