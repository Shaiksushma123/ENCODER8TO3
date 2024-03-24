# ENCODER8TO3

# Aim:
To simulate and synthesis 8 to 3 encoder using vivado.

# Apparatus Required:
vivado software.

# Procedure:
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed. 

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it. 

STEP:5 Select the run simulation adn then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table. 

STEP:7 Select the Implementation in the Sources Window and select the required file in the Processes Window.

STEP:8 Select Check Syntax from the Synthesize XST Process. Double Click in the Floorplan Area/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained. 

STEP:9 In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu.

STEP:10 Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here.

STEP:12 Load the Bit file into the SPARTAN 6 FPGA. 

STEP:11 On the board, by giving required input, the LEDs starts to glow light, indicating the output.

![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/824226c8-c767-44b5-ab35-26fed65b195e)
# Truth Table

![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/e228c14b-b814-40c8-92eb-748d48570c04)
# Circuit Diagram

![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/6fa5fe84-fe6f-472d-b9c0-e6dfa17413d3)
![image](https://github.com/RESMIRNAIR/ENCODER3TO8/assets/154305926/7d147e2a-ba03-4714-baee-17615c9c50c1)

# Program
module encoder(d,a,b,c) ;

input [7:0]d;

output a,b,c;

or g1(a,d[1],d[3],d[5],d[7]);

or g2(b,d[2],d[3],d[6],d[7]);

or g3(c,d[4],d[5],d[6],d[7]);

endmodule

# Output
![Screenshot 2024-03-24 225506](https://github.com/Shaiksushma123/ENCODER8TO3/assets/159005642/faad5fb1-e808-463c-8f7c-708b2890df08)

# Result:
Thus the verilog program for 8 to 3 encoder has been simulated and verified successfully using logic truth table.
