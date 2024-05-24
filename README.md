EXP-6

DATE:

                      SCHEMATIC ENTRY AND CIRCUIT SIMULATION OF A CMOS INVERTER
                          TWO INPUT NAND GATE  AND TWO INPUT NOR GATE

**AIM:**
To create,simulate the design of CMOS inverter,NAND,NOR from schematic using cadence.

**APPARATUS REQUIRED:**

cadence

PROCEDURE:
## Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
          i)	tcsh
          ii)	source /home/install/cshrc
          iii)	virtuoso 
## Procedure for Schematic simulation using Cadence
1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
          i)	Create a New Library
          ii)	Create Schematic Cell view.
          iii)	Create the Symbol for schematic Cell view.
          iv)	Create the test Cell view.
          v)	Analog simulation by spectre
## Procedure for Creating New Library.
a)	File –New – Library
b)	Name : Give name for ur library Ex: VLSILAB , Enable Attach to an existing technology library, Click OK
c)	Attach the library to the technology library gpdk045.Click OK
## Create Schematic Cell view.
a)	Go to 1st window i.e virtuoso(CIW)
b)	File-New-Cell view
c)	Setup the new file form, Library: Select the one you a created. Cell : Give the experiment name Ex: Inverter View: Schematic
d)	Type: Schematic press OK
e)	Add the required components from the libraries and make the connections.
f)	Go to instance fixed menu or use shortcut key “I” from keypad to go instances Click on browse. This opens the library browser ow select the appropriate library for components like Gpdk045,nmos, pmos
g)	Analog library	Vdd, Gnd, Vcc, Vpulse, Vsin
h)	Make the connections by using fixed narrow wire key
i)	Click Check and Save button


## Creating the Symbol for schematic Cell view
a.	In the schematic window, execute
          Crate – Cell view – From Cell view
          The cell view from cell view window appears
          Check Lib Name, Cell Name, From View name must be schematic Press ok
b.	Now Symbol generation form appears. Click Ok If No changes required
c.	A new window with with default symbol is created.
d.	Edit the symbol if you want to give actual symbol shape else continue.
          i.	Execute Create-Cell view-from cell view
          ii.	Library Name and Cell Name must be same which you have used for schematic. Press OK
          iii.	Check for the position of pin side.Prss OK
          iv.	Edit for the shape by Create-Shape-Choose required options to edit.
## Creating the new test cell view

a)	Go to CIW window, Execute File-New-Cell view
b)	Setup the new file form
Library: Select the one you a created.
          Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
          View: Schematic
          Type: Schematic  press OK
## Analog simulation by SPECTRE.
a.	In test cell view window
i.	Launch – ADE L(Analog Design Environment)
b.	Execute Setup—Simulation/directory/Host A new window opens
c.	Set the simulation window to spectre and click ok
d.	Execute Setup-Model Library. Anew window opens, Check of gpdk.scs as lib and section type as stat then press OK.
e.	Execute Analysis – Choose. A window opens.
f.	Select the type and set the specifications and press OK
g.	Execute Output s—to be plotted – Select on Schematic
h.	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
i.	Execute Simulation -- Net list and Run

**INVERTER SCHEMATIC:**

![331879318-3edfea85-b1df-471a-847c-93f6a49c6fa8](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/e64ab051-f7af-4d32-8192-b9b54c145200)

![331879335-9ec65ffa-19e2-4f01-bf93-5e4b8e68c8e8](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/c6e585f8-a492-4a8f-b292-2b450d618718)


**Specifications:**
Vpulse 

    V1 = 0	       
   
    V2 = 1
    
    td = 0,tr=tf=1 n, ton= 100n ,T=200n
    
    Vdc = 1

Simulation Settings

Setup for transient analysis:

   Stop time =400n

Setup for D.C analysis

Component to be selected in schematic is for d.c analysis

    Start = -1 Stop = 1 resp.

Expected Waveform:

**Transient Analysis:**

![331879349-ab6959dd-7665-4d0a-9095-33e48ccfc268](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/140d7b53-c95c-4fcc-bd71-d1fd27b1d584)

**DC Analysis:**

![331879364-9eaed32b-b678-42b5-aec0-1b1b56f62cfd](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/814f0505-3fbe-4828-be68-e9a42e002371)

**NAND SCHEMATIC :**

![331879375-a43a7f87-68ba-4801-b31f-3a8d9aed6a9c](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/fe5fb0d1-bca1-4765-8434-e98c95e0874c)


![331879383-eaf9ee08-67c9-4ac4-9f5c-b16cd1759be5](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/a9a23d0f-1e47-4d62-92d9-11d0fa9286be)




**Specifications:**

Vpulse 

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns

Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns

Vdc = 1

Expected Waveform:

**Transient Analysis:**

![331879489-e38efb30-e0dd-4b65-ab6e-8f8b3330a38a](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/75f10d01-726a-4a62-9433-18fd478487bb)


**NOR SCHEMATIC:**

![331879506-a06c51a1-0934-4dbf-aab5-15a09969b5cd](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/1b97ae24-d09e-4252-a744-d943311ae581)

![331879516-d7ca0d0d-c6f5-45cb-8e9e-9afb599ec96d](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/b2cd7e18-e631-4cc6-8131-177f888f75a8)


**Specifications:**

Vpulse 

Va1 = 0 Va2 = 1 tr=tf=50ps, period=20ns pulse width = 10ns

Vb1 = 0 Vb2 = 1 tr=tf=50ps, period=40ns pulse width = 20ns

Vdc = 1

Expected Waveform:

**Transient Analysis:**

![331879529-d93d42de-64f6-4381-b22b-00256b8b9406](https://github.com/jaggu654/VLSI-LAB-EXP-6/assets/167850134/90f0bf21-fa4f-4a10-8398-92b8a5f31f06)


**RESULT:**

Thus, the design,simulation and verification of the CMOS inverter,NAND,NOR from schematic using cadence was successfully completed.
