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
*Differential input applied to M1 and M2 (NMOS).<br/>
*Gate voltages:<br/>
Vcm + Vd/2 and Vcm - Vd/2 to isolate the differential mode and suppress common-mode.<br/>
*Output voltage is the difference of drain voltages of M1 and M2.<br/>
*Current mirror (M3, M4 – PMOS) used as active load.<br/>
### Stage-2: Common Source Gain Stage
*Receives the output from Stage 1.<br/>
*Consists of a common-source PMOS(M5) and NMOS(M6) pair.<br/>
*Acts as a voltage amplifier and provides additional gain.<br/>
*Connected (M6) to the current mirror for biasing.<br/>
## Key Parameters:
*Gain of Stage 1: Gm × Rout<br/>
---Gm : Equivalent gm of stage-1<br/>
---Rout : equivalent Rout of stage-1<br/>
=> Gain(stage-1) = (gm1)(ro4||ro2)<br/>
=> Gain of stage-2 = gm5(ro5||ro6)<br/>
*Overall Gain: Product of stage-1 and stage-2 gains<br/>
=> Overall gain of 2 stage OTA = (gm1)(ro4||ro2)gm5(ro5||ro6)<br/>
*DC Gain Requirement: ≥ 40 <br/>
*Gate Overdrive Voltage: Assumed 200 mV during hand calculations<br/>



