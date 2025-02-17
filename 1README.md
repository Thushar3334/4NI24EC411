# EXPERIMENT-1

## AIM
### To perform AC, DC, and Transient analysis in LTspice for a given circuit design.
## COMPONENTS REQUIRED:
### MOSFET(nmos4 ,pmos4 ), Resistor(1k), voltage supply(1.8V,0.6V) and connecting wires.
## THEORY:
### A MOSFET (Metal-Oxide-Semiconductor Field-Effect Transistor) is a type of transistor used to switch or amplify electronic signals. It has three main parts:
* Gate (controls current flow),
* Source (where current enters),
* Drain (where current exits).
MOSFETs are key components in many electronic devices like microprocessors and memory chips due to their efficiency and versatility.
The drain current

Id = 1/2 kn Vov2 ; Vov=Vgs-Vth and kn=un Cox W/L
## PROCEDURE:
* Create Folder: Make a folder named "project file".
* MOSFET:
NMOS: Name it CMOSN, set L = 180n, W = 3u.
PMOS: Name it CMOSP, set L = 180n, W = 3u.
* DC Analysis:
* Apply Vdd = 1.8V, Vgs = 0.9V.
*Set up DC analysis .op, run to get Vout and Id.
* Transient Analysis:
* Set Vgs = 0.9V, Amplitude = 50mV, Freq = 1kHz.
* AC Analysis:
* Add library path, set .ac dec 20 .1 1T.
* Run to analyze frequency response.
## CIRCUIT DIAGRAM:
![Ckt 1](https://github.com/user-attachments/assets/f9519e8b-bfa9-4177-8720-59d38c2b574c)

## DC ANALYSIS
### Click on simulate and select dc op pnt.
![dcoppnt 1](https://github.com/user-attachments/assets/b61e8a22-3fc6-4117-883b-609504347910)
### figure: shows the output of dc analysis
## TRANSIENT ANALYSIS:
### Click on simulate and select transient.
![1 waveform](https://github.com/user-attachments/assets/3efbf6de-bcfd-4465-9c0d-7259e989fdc0)
### figure: shows the output andt input waveform for transient analysis.
## AC ANALYSIS:
### Go to simulate and select ac analysis:
![2 waveform](https://github.com/user-attachments/assets/eaeb7c03-b942-4f4c-971b-2f20102bf226)
### figure: shows the output of ac analysis.
## RESULT:
* ID:2.7082e-005
* Got all the output waveforms for all DC, AC and transient analysis.
## INFERENCE:
### To perform AC, DC, and Transient analysis in LTspice for a circuit.
* DC Analysis: Set up a DC operating point to determine the biasing conditions of the circuit (voltage, current). Run the DC analysis to find steady-state values.

* AC Analysis: Use an AC source to analyze the frequency response. Set the frequency range, and the simulation will show how the circuit behaves with respect to small-signal variations across frequencies.

* Transient Analysis: Use a time-varying signal (like a pulse or step) to see how the circuit responds over time. It helps visualize the time-dependent behavior of voltages and currents in the circuit.
### Key Steps in LTspice:
* DC Analysis: Choose DC operating point.
* AC Analysis: Set the AC source, define frequency range, and select AC Analysis.
* Transient Analysis: Set a pulse/step signal, define the time parameters, and select Transient analysis.
### These steps allow you to analyze the circuit’s behavior under different conditions, including biasing, frequency response, and time-based responses.


# CIRCUIT-2:
![2nd ckt](https://github.com/user-attachments/assets/bf9c1c48-6551-4cbf-8f35-4d8981e7369d)
## PROCEDURE:
* Create a New Folder and Save LTSpice File
Create a folder named Project File.
In LTSpice, save your schematic in this folder.
* Set MOSFETs (CMOSN & CMOSP)
CMOSN (N-Channel MOSFET):
Name it CMOSN, set L = 180nm, W = 1.08µm.
CMOSP (P-Channel MOSFET):
Name it CMOSP, set L = 180nm, W = 134µm.
* DC Analysis
Connect the MOSFETs as per the circuit (PMOS to Vdd, NMOS to GND, Gate to input signal).
Apply Vdd = 1.8V and Vgs = 0.3V.
Go to Simulate → Edit Simulation Cmd, select DC Analysis (.op), click OK, and run to get Vout and Id.
* Transient Analysis
Apply Vgs = 0.3V with a 50mV amplitude and 1kHz frequency sine wave.
Go to Simulate → Edit Simulation Cmd, select Transient Analysis, and click OK. Run to observe the time-domain response.
* AC Analysis
Add the library file path in the spice directive.
Go to Simulate → Edit Simulation Cmd, select AC Analysis, and click OK. Run to analyze gain and frequency response.
## DC ANAALYSIS:
![DCOPPNT2](https://github.com/user-attachments/assets/8f48b476-5d11-42fe-8d82-86ac8afe5959)
###figure: shows the output of dc analysis
## TRANSIENT ANALYSIS:
![tran op 2nd](https://github.com/user-attachments/assets/8f18ade5-a82e-49e2-b6de-3e5e5c4f6360)
### figure: shows the output for transient analysis.
![tran ip 2nd](https://github.com/user-attachments/assets/502f9520-8611-43d2-b1a5-fb26dab65f8b)
### figure: shows the input for transient analysis.
## AC ANALYSIS:
![Ac ana 2nd](https://github.com/user-attachments/assets/2aabfa2d-cd23-4d26-b54e-f0c991bcc7f9)
### figure:shows the output of ac analysis.
## inference:
* Id vs. Width: The drain current (Id) depends on the width (W) of the MOSFET. As W increases, Id increases, assuming other factors remain constant.

* DC Analysis: Ensures proper biasing so that the MOSFET operates in saturation, stabilizing the Q-point for reliable performance.

* Transient Analysis: Shows how the circuit responds to time-varying signals, essential for high-speed applications where quick responses are critical.

* AC Analysis: Focuses on the circuit's frequency response, gain, and impedance, helping in designing circuits with desired performance and small-signal behavior.

* Combined Analyses: All these analyses work together to design and optimize amplifiers, ensuring proper operation under both steady-state (DC) and dynamic (AC) conditions.






