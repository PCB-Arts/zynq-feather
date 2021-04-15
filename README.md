# Zynq Feather r0.2 16.04.2021
This is the second revision of the Zynq-Feather project. This project is currently still under development. It is not recommended to copy the project in this release state.

![grafik](https://user-images.githubusercontent.com/63359549/114945997-a781c400-9e4a-11eb-81fe-fdaec2c6c07d.png)


Things that are on the ToDo list:
-	Layerstack: (The current layerstack is not optimized and ready for production. The prototypes were produced with a default pool layerstack without impedance control. Due to the short trace lengths this works for prototypes but isn´t recommended)
-	board-board interface: Will be re-routed to support the zynq RGMII Interface.
-	USB current limit: The USB current limit can be bypassed with a MOSFET controlled by the FPGA. This will be reworked in future revisions
-	PCB Designrules: The current PCB Fab designrules required by the layout are 80um trace clearance and thickness. This will be reworked (if possible) in future revisions.
-	Input buffers: the analog input buffers are there to support high impedance sensors. The chosen resistance values are just placeholders right now. We choose discrete buffers for every channel to get rid of charge injection through a MUX which would be especially bad for high impedance sensors. Currently the input pins of the FPGA adds a parasitic resistance to the analog nodes. We will rework that in future revisions.
