
# Create a New Project

- A project in Quartus is a collection of sources (Schematic or Hardware Description Language (HDL) files), testbenches, and simulation outputs. The project information specifies to Quartus what FPGA model you are working with and which synthesis tool to use, as well as some other parameters. Each project will compile all of its contained source files together, so you will create a new project for every lab section.

1.	Click File $\longrightarrow$ New Project Wizard 

2.	Click Next to advance. 

3.	Select a work directory where your project will be stored, and name your project. It is recommended that you create a ECE 272 folder in your Documents folder and separate folders for each lab within the ECE272 folder. Select your Lab1 folder as your directory for this project and click next.

4.	In Project Type, select an Empty project and click next

5.	For this lab, add no files, just click next.

6.	The device Family is Max 10. Under Available devices, select 10M50DAF484C7G, and click next.

7.	For this lab do not edit the EDA Tool settings, just click next.

8.	Review the Project Information and click Finish. If prompted, select “allow trusted source.” 

---

# Schematic Entry

Digital logic schematics are one type of source file in a project, which show the logic gates required to implement each block in the block diagram. A project may have several schematic source files, which will be explored in later labs. Digital logic schematics are not to be confused with circuit schematics, a lower level of abstraction showing electrical components such as resistors and capacitors. Outside the context of Quartus and consequently this course, digital logic schematics are more often referred to as digital logic diagrams. Standard design generally has inputs on the top left, and the outputs on the bottom right. 

### Create a Blank Schematic Source File:

1.	To add a source, Click File → New.
2.	In the New window under Design Files, select Block Diagram/Schematic File and press the OK button.
3.	The Quartus project screen will now be showing the blank schematic file.

---

# Define Inputs and Outputs:

Labeling the inputs and outputs on the schematic allows Quartus to create a ’netlist’ (stands for a ’list of electrical networks’) during the synthesis process, in which the graphical circuit designed in the schematic file is translated into a list of all inputs, outputs, logic gates, and the connections between them. Quartus can then use this netlist to map out the design onto logic circuits used in the FPGA for prototyping, a physical hardware test of the design. A netlist can also be used for simulation, which is a software test of a circuit’s behavior.

1.	Click the dropdown arrow on the Pin Tool, and select “Input.”

2.	Place 3 input markers named A, B, and C by left clicking on the dotted grid in the schematic window.

3.	Use the esc key or click the Selection Tool (the mouse arrow icon, 5 icons to the left from the Pin Tool) to exit the Pin Tool. Right click each of the inputs to rotate and rename. To rotate, hover over “rotate by degrees” after right clicking and select “rotate left 270.” To rename, select “properties” after right clicking and change the “pin name.” Select “OK” to save the new name.   

4.	Following a similar process, add an Output marker named Z. 

---

# Add Symbols:

1.	Click the Symbol button. 

2.	Select the installation directory → primitives →logic library


3.	Select the and2 gate and click the OK button. Place the and2 gate in the middle of the schematic. Note, The '2' in the and2 gate means it is a two input and gate.

4.	Repeat step 2, but select the xor and place it. 

5.	Repeat step 2, but select the or2 and place it.

6.	Reference Figure 1.23 to create your schematic.

---

# Connect the Symbols:

1.	Click the Orthogonal Node Tool button

2.	Wire all the symbols together as shown in Figure 1.27 below. Hold left click to draw wire connections. Start with vertical trace lines under each input pin, then connect the XOR and OR2 gates to the appropriate wires. Finally, connect the AND2 gate with the other gates and output Z.

3.	Save the schematic (Ctrl-S). For this lab, the schematic can have the same name as the project. We will discuss file naming more in future labs that require multiple schematic files.

- **Warning:** Nodes may sometimes appear to be connected when they aren’t. An X signifies a floating end to a wire. It may help to zoom in on any connections obscured by text to verify that wires connect where you want them to. Always check for broken connections in your schematics!

---

# Compile Design

- Click the blue play button to Compile, or go to the Processing tab and click Start compilation.  

- You must recompile your design any time you change source files for the project! This includes editing assignments.

- If you encounter “Error 114005: can’t find database file”, check that your project is saved in a path without spaces (for example, the “My Documents” folder has a space). The file path may be shown with the error, or you can navigate to the project through your file manager. Generally, a shorter file path works best if you encounter this error (i.e. fewer nested folders). If you continue to have issues compiling, try closing Quartus, deleting the “db” folder from the project folder, then reopening the project in Quartus and compiling.

---

#Assigning Pins

The Assignment Editor and Pin Planner in Quartus are where you set which pins the inputs and outputs are connected to. Pin names can be found in the DE10-Lite user manual. Assign Output Z to one of the LEDs on the FPGA, shown on page 27 of the user manual. Assign the Inputs A,B, and C to switches, shown on page 26. 

1.	Click Assignments → Pin Planner. A window will open with several panes showing a Top View grid of the MAX 10 FPGA pins as letters and symbols, a Pin Legend, and Tasks. Your inputs and outputs can be found listed as Node Names in the All Pins pane on the bottom of this window.

2.	Under Location, the third column from the left, enter the Name of the Pin you wish to connect that node to. EG: PIN_A8.  Typing A8 would be enough for auto complete to finish the full name.

3.	Start typing in the I/O Standard column, a selection menu will appear. Select from the I/O standard drop down menu each pin to be the same value as the one listed in the manual.  A8 would be a 3.3 V LVTTL.

4.	Repeat this process for each input and output.

5.	Save the pin assignments (Ctrl-S).

6.	Compile your design again.

---

# Test The Design

Fill in the truth table below in Figure 1.28 with the expected Z output for every combination of the A, B, and C inputs. Then, using ModelSim, run a simulation that uses all inputs listed in Figure 1.5 and record the Z output for each combination. If testing on the FPGA, test each combination of inputs and record the output on the LED. 

---

# Simulation

- Simulating allows for testing digital logic designs without the need to upload the design onto hardware. The simulation takes different user selected values, typically for inputs, and shows how outputs or other values change in response.

- Your schematic must be turned into a Hardware Description Language (HDL) for ModelSim to simulate it. To do this in Quartus, have the schematic file open, click File → Create/Update → Create HDL Design File from Current  File → Verilog.  A dialogue box will pop up, select “Verilog HDL” and press OK.

- This .v file will be what you compile and simulate in ModelSim. 

1.	The window shown below in figure 1.29 will pop up when you first open ModelSim. Click Jumpstart, then Create a Project to begin working on a project. If this window does not appear, you can also select File → New → Project.

2.	When prompted, as seen below in figure 1.31, name your project, avoiding symbols, spaces, and dashes, and change the project location to the Lab1 file you created for your Quartus files.

3.	Next, choose Add Existing File and locate the .v file you created in Quartus.

4.	Select Compile → Compile All to compile the .v file. A green check mark should replace the question mark next to the file name once it has successfully compiled.

5.	Select Simulate → Start Simulation and click the + next to “work” in the pop up to find the .v file. Select the .v to simulate and press OK. If you do not see the dark blue Objects pane or gray and black Wave pane as shown below in figure 1.37, select View → Objects or View → Wave to add those panes.

6.	Select File → New → Source → Do to create a .do file. 


a.	For the first line of the .do file, use the “vsim -gui work.filenamehere” command that appeared in the transcript pane when you first started the simulation. 

b.	On the second line, type “add wave \*”, which will add all inputs and outputs to the simulation. 

c.	Use the “force” command to set values for your inputs at different times following the format: “force INPUT VALUE @ TIME”. For example, “force B 1 @ 20” sets the B input to 1 (or HIGH) at time = 20 picoseconds. 

d.	The “run” command is then used at the end of the .do file to determine how long the simulation runs.


7.	Select File → Save to save the .do file, then in the transcript pane type “do NameOfDoFile”. If the .do file was named “272sim.do”, you would type “do 272sim”. If this does not work, try “do 272sim.do”.

8.	After running the .do file, you should see green lines appear in the Wave pane. If they do not extend the full length of the pane, you can zoom in by selecting the blue magnifying glass in the toolbar. The green lines show the level of the inputs and outputs chronologically from left to right as the inputs change with time, with a higher line representing 1 or HIGH and a lower line representing 0 or LOW.

---

# Program The FPGA

1.	Plug the DE10-Lite into the computer with the provided USB cable.

2.	In Quartus, click Tools → Programmer. 

3.	Click Hardware Setup and under “Currently selected hardware” select the USB Blaster. If it does not show up, make sure you correctly installed the USB drivers. Find more information on troubleshooting USB drivers here.

4.	Press close.

5.	In the dialogue box you will see “File” “Device” “Checksum” etc. In the File column, output_files/lab1.sof should already be there. 

6.	Make sure the correct device is selected (double check the model number is the FPGA you are using). 

7.	Click Start.

