# PLC_Mixing_Tanks_codesys
PLC_Mixing_Tanks(codesys)


Mixing and Heating of Liquid Components
This project involves the control and management of a technological system that includes two identical tanks for mixing liquid components and temperature control. Additionally, there is a receiving tank (not shown in the task description) with a smaller volume compared to the combined volume of the two mixing tanks.

Start-Stop
The objective is to achieve the following functionality:

Upon pressing the "Start" button, the valve for the first product's intake opens.
After reaching the intermediate level, the valve for the first product closes and the valve for the second product's intake opens.
Upon triggering the high-level alarm, the valve for the second product's intake closes, and the steam valve opens at 100%.
Once the temperature reaches 95 degrees Celsius (within a sensor range of 0-150 degrees Celsius), the steam valve remains open at 20% for an additional 10 seconds.
After the holding time elapses, the liquid is drained from the apparatus.
If the low-level alarm is deactivated, the cycle repeats, unless the "Stop" button is pressed. In the case of pressing the "Stop" button, the drain valve closes.
The PLC receives a signal from a level sensor with a measurement range of 0-5 meters.
Scaling of inputs and outputs should be implemented.
The low-level alarm is triggered when the level exceeds 1. The intermediate-level alarm is triggered when the level exceeds 5000. The high-level alarm is triggered when the level exceeds 9500. The maximum level is set to 10000.
The temperature of the product in the tank follows the formula: T (In the tank) = T (In the tank) * 0.997 + T (Steam) * 0.003.
Please note the requirement for input and output scaling to be implemented to ensure proper operation.

Getting Started
To run the project, follow these steps:

Install CODESYS software on your computer.
Open the project file named "Mixing_Heating_Project" in CODESYS.
Ensure that all necessary hardware components are properly connected to the PLC.
Build and download the project to the PLC.
Press the "Start" button on the control panel to initiate the mixing and heating process.
Monitor the system behavior and verify that the valves open and close as expected, and the temperature is controlled within the desired range.
Press the "Stop" button to halt the process and close the drain valve.
Inputs and Outputs
The project relies on the following inputs and outputs:

Inputs:
Start button signal
Stop button signal
Level sensor signal
Outputs:
Valve control signals
Steam valve control signal
Low-level alarm signal
Intermediate-level alarm signal
High-level alarm signal
Ensure that the inputs and outputs are correctly configured and connected to the PLC.

Scaling
Proper scaling of inputs and outputs is crucial for accurate operation. Ensure that the scaling parameters are appropriately set in the PLC program to match the physical measurement range and desired control range.

For additional information and detailed implementation, refer to the project documentation and source code files.

Enjoy the mixing and heating of liquid components with this automated control system!
