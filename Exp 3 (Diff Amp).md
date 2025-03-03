# BASIC DIFFERENTIAL AMPLIFIER

## Aim:
To design and analyse the MOS Differential Amplifier

## COMPONENTS REQUIRED:
* N Channel Mosfet (nmos4)
* Resistor (1.14k, 327.8)
* Voltage source
* Current source
* Signal Generator

# THEORY:
A MOS differential amplifier amplifies the difference between two input signals while rejecting common-mode signals. It uses two MOSFETs biased in the saturation region, acting as controlled current sources.
* Differential Mode: The output voltage is proportional to the difference in input voltages, given by Vout= gm x (Vin1 - Vin2) where gm is transconductance and Rd is the load resistance.
* Common-Mode: If the inputs are the same, the output ideally is zero, rejecting common-mode signals.
This amplifier is used in applications like operational amplifiers, where noise rejection and differential signal amplification are needed.

# PROCEDURE:
1. Open LTspice and Create a New Schematic
2. Place MOSFETs
3. Place Resistors
4. Add Input Voltage Sources
5. Biasing the MOSFETs
6. Set up Power Supply
7. Connect Ground
8. Define the Parameters
9. Add Simulation Command
10. Run the Simulation
11. View the Results

# CIRCUIT 1:
![1st ckt](https://github.com/user-attachments/assets/9676b152-10d7-4abd-9192-5c5a2207030e)
## DC Analysis:
![1st ckt dc](https://github.com/user-attachments/assets/f7fc240c-3ec2-4bb1-b818-e28492e6e11f)
ID1 : 0.61mA
ID2 : 0.61mA
Iss : 1.2mA
Vocm : 1.1V
Vicm : 0.95v
## Transient Analysis:
### Input:
![1st ckt tran inp](https://github.com/user-attachments/assets/f4301aaa-5d7a-4278-b8f2-9ac4f25bf54f)
Vin = 1-0.90
### Output:
![1st ckt tran out](https://github.com/user-attachments/assets/9e07e2e1-a271-4ca1-bbde-08c814312ab1)
Vout = 1.52-0.65
### Input and Output:
![1st ckt tran in out](https://github.com/user-attachments/assets/935a347e-eadf-48d2-b0e1-46490301e981)
Gain = Vout/Vin
     = 0.87/0.1
     = 8.7
Gain in dB = 20 log (8.7)
           = 18.79 dB
## AC Analysis:
![1st ckt ac out](https://github.com/user-attachments/assets/bd44c756-783e-42ba-9781-613fd8192f29)

# CIRCUIT 2:
![2nd ckt](https://github.com/user-attachments/assets/50941e26-da4d-4906-a72b-fb7f1013a191)
## DC Analysis:
![2nd ckt dc](https://github.com/user-attachments/assets/15b50f56-ecd5-46e1-8c4d-52e8f0732417)
ID1 : 0.61mA
ID2 : 0.61mA
Iss : 1.22mA
Vocm : 1.1V
Vicm : 0.95V
## Transient Analysis:
### Input:
![2nd ckt tran inp](https://github.com/user-attachments/assets/e3ec1281-4fb3-4097-9d52-fd72c58a0cf3)
Vin = 1-0.90
### Output:
![2nd ckt tran out](https://github.com/user-attachments/assets/44136496-fa7e-41c5-8ce8-d0535e783d9f)
Vout = 1.53-0.67
### Input and Output:
![2nd ckt tran in out](https://github.com/user-attachments/assets/d9325f5d-badb-4cc5-8940-4a4e9333ab95)
Gain = Vout/Vin
     = 0.86/0.1
     = 8.6
Gain in dB = 20 log (8.6)
           = 18.689 dB
## AC Analysis:
![2nd ckt ac out](https://github.com/user-attachments/assets/ecb74773-afda-4017-bacb-db16b6d49aee)

# Circuit 3:
![3rd ckt](https://github.com/user-attachments/assets/449c730c-273d-425e-8e47-d02d9a6500ff)
## DC Analysis:
![3rd ckt dc](https://github.com/user-attachments/assets/36942042-fa40-49a1-a70a-cc7b96df31aa)
ID1 : 0.61mA
ID2 : 0.61mA
Iss : 1.2mA
Vocm : 1.1V
Vicm : 0.95v
## Transient Analysis:
### Input:
![3rd ckt tran inp](https://github.com/user-attachments/assets/fe3d907f-127b-45a7-9647-8827625a81df)
Vin = 1-0.90
### Output:
![3rd ckt tran out](https://github.com/user-attachments/assets/0d8bfbba-d463-4755-aab8-a03d10a04f23)
Vout = 1.53-0.66
### Input and Output:
![3rd ckt tran in out](https://github.com/user-attachments/assets/cd3c347c-5e1a-4f1e-aaa3-a3d8e47977e3)
Gain = Vout/Vin
     = 0.87/0.1
     = 8.7
Gain in dB = 20 log (8.7)
           = 18.790 dB
## AC Analysis:
![3rd ckt ac out](https://github.com/user-attachments/assets/0ccc3796-58f9-406d-9ecf-ca01f4060f81)

# INFERENCE:
*DC Analysis:
Drain currents (ID1, ID2) are 0.61mA, indicating even current sharing.
The supply current (ISS) is about 1.2mA.
Common-mode voltages (Vocm and Vicm) are around 1.1V and 0.95V, showing effective rejection of common-mode signals.
* Transient Analysis:
The input signal varies between 1V and 0.9V.
The output voltage ranges from 1.52V to 0.65V, with a voltage gain of 8.7 (18.79 dB in Circuit 1 and 18.69 dB in Circuit 2).
* AC Analysis:
The amplifier operates well with minimal distortion, amplifying the differential signal.














