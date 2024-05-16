# VLSI-LAB-EXP-6
SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL

AIM: To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

APPARATUS REQUIRED:

Laptop with MobaXterm
Cadence tool PROCEDURE SCHEMATIC ENTRY: Creating a new library:
In the library manager, execute File - New library. The new library form appears.
In the new library form, type ‘my design lib’ in the name section.
In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
After creating a new library you can verify it from the library manager.
If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.
Creating a schematic cell view:

In the CIW or library manager, execute file – new – cell viw.
Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
Click ok when done the above setting. A black schematic window for the inverter design appears.
Adding components to schematic:

In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
After you complete the add instance form move your cursor to the schematic window and click left to place a component. LIBRARY NAME CELL NAME gpdk045 PMOS gpdk045 NMOS
This is a table of components for building the inverter schematic.
After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/ed805916-b83a-4ece-97c3-9cf61e126095)
to schematic:
Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin. PIN NAMES DIRECTION Vin,Vdd,Vss Input Vout Output
Select cancel and then the schematic window enter window file or press the f bind key. Adding wires to schematic:
Click the wire (narrow) icon in the schematic window.
In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.
Saving the design: Click the check and save icon in the schematic editor window observe CIW output for any errors.

BUILDING THE INVERTER TEST DESIGN: Creating the inverter test cell view:

In the CIW or library manager, execute file – new – cell view.
Setup the newfile as shown below.
Click ok when done. A blank schematic window for the inverter test design appears.
Using the components list and properties/ comments in this table build the inverter test schematic. LIBRARY NAME CELL VIEW NAME PROPERTIES/COMMENTS My design lib Inverter Symbol Analog lib Vpulse Voltage1 = 0, Voltage2 = 1.8, delay Time = 0, Rise time=Fall time=1ns Period=20ns Analog lib Vdc, gnd Vdc = 1.8v
Add the above components using create – instance or by pressing I.
Click the wire (narrow) icon and wire your schematic.
Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
Click on the check and save icon to save the design. 
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/b425456e-81e6-4997-a2b1-477d4099114e)
SIMULATION WITH SPECTRA: Starting the simulation environment:
In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:
In the simulation window (ADE) execute setup – simulator / directory / host.
In the choosing simulator form, set the simulator field to specra and click ok.
In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:
Click the choose- Analysis icon in the simulation window (ADE).
The choosing analysis form appears.
To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.
To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.
Selecting output for plotting:

Execute the o/p’s to be plotted -select on sschematic in the simulation window.
Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.
Running the simulation:

Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
When the simulation finishes the transient and DC plots automatically will be popped up along with netlist. 
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/d2f9a01e-df2a-4e26-ae16-5fcdb25f5d37)
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/ffc33dc8-7d6f-4d9a-aa30-381a4b8f6f11)
CMOS NAND GATE NAND SCHEMATIC 
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/54a1da79-5f65-4c5a-86f4-11b8527f3a07)
NAND TEST CELL VIEW
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/8b799071-cdee-498c-9d8b-c6a26f6c9e4d)
SIMULATION WITH SPECTRA 
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/35c1c963-c88d-4c24-9f14-e6501c8b0ce4)
CMOS NOR GATE NOR SCHEMATIC
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/d4d78e7e-c2ac-475a-94bd-58ebd267da95)
NOR TEST CELL VIEW
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/78fa6e51-9fe2-464c-a550-3e729deff4c9)
NOR SIMULATION WITH SPECTRA
![image](https://github.com/Kirthana-2004/VLSI-LAB-EXP-6/assets/144320880/fad9531a-31cb-4138-848d-6b9a579161af)











