# EXPERIMENT-1

## AIM
### To perform AC, DC, and Transient analysis in LTspice for a given circuit design.
## cOMPONENTS REQUIRED:
### MOSFET(nmos4 ,pmos4 ), Resistor(1k), voltage supply(1.8V,0.6V) and connecting wires.
## THEORY:
### A MOSFET (Metal-Oxide-Semiconductor Field-Effect Transistor) is a type of transistor used to switch or amplify electronic signals. It has three main parts:
*Gate (controls current flow),
*Source (where current enters),
*Drain (where current exits).
MOSFETs are key components in many electronic devices like microprocessors and memory chips due to their efficiency and versatility.
The drain current

Id = 1/2 kn Vov2 ; Vov=Vgs-Vth and kn=un Cox W/L
## PROCEDURE:
### *BY using the power formula P=V*I 
*we get the drain current as,
*Id=5.55e-005A
## CIRCUIT DIAGRAM:
![2nd ckt](https://github.com/user-attachments/assets/3d01c50d-27c5-4c51-a557-fda3f264ad7d)
## DC ANALYSIS
### Click on simulate and select dc op pnt.
![dcoppnt 1](https://github.com/user-attachments/assets/b61e8a22-3fc6-4117-883b-609504347910)
### figure: showa the output of dc analysis
## TRANSIENT ANALYSIS:
### Click on simulate and select transient.
![1 waveform](https://github.com/user-attachments/assets/3efbf6de-bcfd-4465-9c0d-7259e989fdc0)
### figure:shows the output andt input waveform for transient analysis.
## AC ANALYSIS:
### Go to simulate and select ac analysis:
![2 waveform](https://github.com/user-attachments/assets/eaeb7c03-b942-4f4c-971b-2f20102bf226)
### figure:shows the output of ac analysis.
## RESULT:
*ID:2.7082e-005
*Got all the output waveforms for all DC, AC and transient analysis.
## INFERENCE:
### To perform AC, DC, and Transient analysis in LTspice for a circuit.
*DC Analysis: Set up a DC operating point to determine the biasing conditions of the circuit (voltage, current). Run the DC analysis to find steady-state values.

*AC Analysis: Use an AC source to analyze the frequency response. Set the frequency range, and the simulation will show how the circuit behaves with respect to small-signal variations across frequencies.

*Transient Analysis: Use a time-varying signal (like a pulse or step) to see how the circuit responds over time. It helps visualize the time-dependent behavior of voltages and currents in the circuit.
### Key Steps in LTspice:
*DC Analysis: Choose DC operating point.
*AC Analysis: Set the AC source, define frequency range, and select AC Analysis.
*Transient Analysis: Set a pulse/step signal, define the time parameters, and select Transient analysis.
### These steps allow you to analyze the circuit’s behavior under different conditions, including biasing, frequency response, and time-based responses.


