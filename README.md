# EXPERIMENT-03-DEVELOPING-COUNTER-LADDER-LOGIC-FOR-PLC-
## NAME: KANAGAVEL R
## REGISTER NUMBER: 212223040085
## DEPARTMENT: CSE
## YEAR: 3RD

### Aim:
To understand and implement various counter operations in Programmable Logic Controller (PLC) ladder logic.

### Apparatus Required:
Programmable Logic Controller (PLC): A PLC that supports counter functions.
PLC Programming Software: Software such as RSLogix, TIA Portal, or CX-Programmer.
Computer System: For programming and simulating the PLC ladder logic.
Input Devices: Push buttons or switches to trigger the counter operations.
Output Devices: LEDs or other indicators to visualize the counter outputs.
Wires and Connectors: For interfacing input/output devices with the PLC.
Power Supply: Appropriate power supply for the PLC and peripherals.

### Theory:
Counters in PLCs are used to count events or occurrences, such as the number of items passing on a conveyor belt, the number of cycles a machine runs, or how many times a process has started or stopped. Counters are commonly used in automation to perform tasks like stopping a machine after a set number of products or signaling a notification when a count reaches a specific value.

### Types of Counters:
Up Counter (CTU) Functionality:

The up counter counts every time the input condition becomes TRUE (ON). When the accumulated value reaches the preset value, the counter output becomes TRUE. If the reset input is triggered, the counter resets to zero.
Down Counter (CTD) Functionality:

The down counter decreases the count every time the input condition becomes TRUE (ON). When the count reaches zero, the counter output becomes TRUE. The counter can be reset by a reset input to the preset value.
Up/Down Counter (CTUD) Functionality:

The up/down counter can increment or decrement the count based on two different inputs. One input increments the count, while the other decrements it. When the count reaches the preset value or zero, the respective outputs become TRUE. The counter can be reset as required.


### Procedure:
Setup the PLC Programming Environment:
Connect the PLC to the computer and launch the PLC programming software.
Ensure all input and output devices are connected to the PLC’s I/O modules.
Create Ladder Logic for Counters:
Up Counter (CTU):

Create a rung with an input (e.g., a push button) linked to a CTU instruction.
Set the preset value (e.g., 10 counts). Assign an output to indicate when the preset value is reached.
Down Counter (CTD):

Create a rung with an input linked to a CTD instruction.
Set the preset value (e.g., 5 counts). Assign an output to indicate when the counter reaches zero.
Up/Down Counter (CTUD):

Create a rung with separate inputs for counting up and counting down.
Set the preset value (e.g., 8 counts). Assign outputs for when the count reaches the preset value or zero.
Simulate the Ladder Logic:
Up Counter (CTU):

Run the simulation in the PLC software. Press the input button repeatedly and observe the counter increment until the preset value is reached, at which point the output activates.
Down Counter (CTD):

Run the simulation, press the input button repeatedly, and observe the counter decrement. When the counter reaches zero, the output activates.
Up/Down Counter (CTUD):

Simulate both the up and down counting inputs. Observe how the counter increments or decrements and how the output is activated when the count reaches the preset value or zero.
Download and Execute:
Download the ladder logic program to the PLC if available and run it.
Test the counters with the physical push buttons and observe the LEDs or other output devices.
### Outputs:
Up Counter (CTU): The output LED or indicator should activate when the preset count (e.g., 10) is reached.
Down Counter (CTD): The output should activate when the count reaches zero.
Up/Down Counter (CTUD): The output should activate when the count reaches the preset value or zero, depending on the inputs.

### Simulation Screenshots:

### Counter:

<img width="1752" height="925" alt="Screenshot 2025-11-19 181459" src="https://github.com/user-attachments/assets/5199e8f6-334d-476f-abdc-54964885ab8c" />

<img width="1732" height="862" alt="Screenshot 2025-11-19 181514" src="https://github.com/user-attachments/assets/0a325ab7-16d2-47fd-8272-91f0c48cbd2f" />

<img width="1741" height="867" alt="Screenshot 2025-11-19 181528" src="https://github.com/user-attachments/assets/d0bc2f4e-ebf3-482a-9c4a-15e0c9511586" />

<img width="1739" height="866" alt="Screenshot 2025-11-19 181544" src="https://github.com/user-attachments/assets/7fe0874c-d5f0-46d7-b772-a332a1480fb1" />

<img width="1736" height="864" alt="Screenshot 2025-11-19 181559" src="https://github.com/user-attachments/assets/986703a9-f10e-47b3-b53f-cbc4e00a971b" />

<img width="1747" height="865" alt="Screenshot 2025-11-19 181612" src="https://github.com/user-attachments/assets/4e13abc6-b57a-4edb-a054-a96999b3072a" />

### Up Counter:

<img width="1744" height="923" alt="Screenshot 2025-11-19 181839" src="https://github.com/user-attachments/assets/50b55745-0b36-4927-b0db-f5fd1e7c6c0f" />

<img width="1647" height="353" alt="Screenshot 2025-11-19 181939" src="https://github.com/user-attachments/assets/31bca990-d54e-4d2c-bb36-431c6781b9f9" />

<img width="1869" height="255" alt="Screenshot 2025-11-19 181853" src="https://github.com/user-attachments/assets/df386615-fb00-4384-a6ac-91923202049f" />

### Down Counter:

<img width="1567" height="707" alt="Screenshot 2025-11-19 182041" src="https://github.com/user-attachments/assets/1ea5696f-b1da-4e83-9da7-490127feadaf" />

<img width="1559" height="419" alt="Screenshot 2025-11-19 182053" src="https://github.com/user-attachments/assets/5e66aadc-0ed0-4a95-bc6c-64da6f5ef267" />

<img width="1578" height="241" alt="Screenshot 2025-11-19 182105" src="https://github.com/user-attachments/assets/3f8449f2-4533-4417-9c72-d2b5845b8fc2" />

<img width="1568" height="229" alt="Screenshot 2025-11-19 182114" src="https://github.com/user-attachments/assets/3464de65-52d2-4fc0-8564-20d8314d0c86" />

<img width="1573" height="219" alt="Screenshot 2025-11-19 182125" src="https://github.com/user-attachments/assets/ddc74935-f5f7-464b-9f66-4244b4c91ac4" />

### Up/Down Counter-1:

<img width="1205" height="545" alt="Screenshot 2025-11-19 182232" src="https://github.com/user-attachments/assets/ec5d6d20-07f5-441b-8f2e-e104eef1cdce" />

<img width="1215" height="466" alt="Screenshot 2025-11-19 182240" src="https://github.com/user-attachments/assets/5773e02f-39e8-4948-b947-74bb5c4d8a46" />

<img width="1321" height="197" alt="Screenshot 2025-11-19 182251" src="https://github.com/user-attachments/assets/217a9498-ba56-43d8-8c76-13c0e1e68085" />

<img width="1324" height="175" alt="Screenshot 2025-11-19 182259" src="https://github.com/user-attachments/assets/82869245-3ab2-4903-9484-9beff4e5d7a3" />

<img width="1323" height="702" alt="Screenshot 2025-11-19 182314" src="https://github.com/user-attachments/assets/4880ce5c-50c2-4b33-b2ee-2acb1d676de6" />

<img width="1327" height="677" alt="Screenshot 2025-11-19 182325" src="https://github.com/user-attachments/assets/a827be23-3086-42c3-996f-1c89eca206a8" />

### Up/Down Counter-2:

<img width="1320" height="699" alt="Screenshot 2025-11-19 182443" src="https://github.com/user-attachments/assets/04ac5cc1-f160-4bd2-9f92-a0da6f4c8e92" />

<img width="1321" height="700" alt="Screenshot 2025-11-19 182456" src="https://github.com/user-attachments/assets/9b9facd9-e0d0-4203-83f1-480453ab3520" />

<img width="1323" height="696" alt="Screenshot 2025-11-19 182515" src="https://github.com/user-attachments/assets/4ae1facb-7bd4-46bd-87cb-5c1e329ea562" />

### Results:
The ladder logic programs for Up Counter (CTU), Down Counter (CTD), and Up/Down Counter (CTUD) were successfully implemented and tested. The outputs behaved as expected, indicating correct counting operations. The experiment demonstrated how counters are essential in automation for counting events and managing process sequences.
