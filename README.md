[VSDsquadron-Mini-Internship](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/7c6beb5d-c964-4422-902a-b1adec7336e3)
# LIST OF Alloted Tasks (April 20,2024)
## 1. Installation of Linux Operating System through Virtual Box
- The screenshot shows the successful installation of Ubuntu version 22.04, an operating system commonly used for software development and various other tasks.
- Note: Installed Ubuntu 22.04 on dual boot instead of using Virtual Box because of personal requirements.
![Screenshot from 2024-04-23 15-09-12](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/bc779ff4-9dc0-4b9e-b333-5d4a3af6a8ab)
## 2. Installation of RISC-V GNU Toolchain
- The image depicts the installation process and successful setup of the RISC-V GNU Toolchain, which is a collection of tools used for compiling and debugging programs written for the RISC-V architecture.
  
![carbon(5)](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/790da1e0-b409-4489-8dab-93b3ac9c8928)
![Screenshot from 2024-04-23 16-07-14](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/aefb261d-978f-4576-9fb0-cdb8893be0d9)
## 3. Installing Yosys Open SYnthesis Suite
- The screenshot shows the installation of Yosys, an open-source framework for Verilog RTL synthesis. Yosys is commonly used for synthesis, formal verification, and analysis of digital designs. It's a powerful tool for designing and optimizing digital circuits.
  
 ![carbon(2)](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/77c3b616-f85c-4ba3-a6c0-5adf80e93dbe)
![Screenshot from 2024-04-23 15-49-43](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/ebfbbfab-28e4-47dc-8bf0-c4b72f36125b)
## 4. Installing Icarus Verilog
- The screenshot showcases the installation of Iverilog, an open-source Verilog simulation and synthesis tool commonly used for designing and testing digital circuits.
  
![carbon(8)](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/8e0584ca-6603-4773-979d-7c4c57d8874a)
![Screenshot from 2024-04-23 15-52-58](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/81cff073-3d2e-401c-a112-85cf61a44131)
## 5. Installing GTK Waveform Viewer
- The image demonstrates the installation of GTKWave, a waveform viewer that allows users to visualize simulation results from digital design tools like Iverilog. It's commonly used for debugging and analyzing digital circuit designs.

![carbon(6)](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/af87d26e-59c4-4de4-aac0-0c94769f8375)
![Screenshot from 2024-04-23 15-55-11](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/936646c0-74ea-4ab5-9b85-06efe867387e)

# Task:2( April 23,2024)
# RISC-V 32-bit Instruction Set Architecture (ISA)
## Instruction Types:

![r type](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/98b9af23-e23c-456f-9a55-eae7f133a871)

#### R (Register-Register Operations):Instructions that operate on data stored in registers.
-  These instructions work with data stored in registers. It's like doing math with numbers you already have. For example, adding two numbers together or checking if one number is bigger than another.

  ![i](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/1db8c45d-1133-4218-8a36-127fc8f9007c)

#### I (Immediate Operations):Instructions that use an immediate value for computation.
- These instructions use a number that's included right in the instruction itself. It's handy for doing quick calculations or grabbing data from memory. For instance, adding a number to another number or loading a piece of data into memory.
  
 ![ss](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/6965b5d3-80b2-4757-9ba4-c169c66904c8)
#### S (Store Operations):Instructions that store data from a register to memory.
- These instructions move data from a register into memory. It's like taking something from your pocket and putting it into a box. For example, saving the result of a calculation into memory.
  
![U](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/a2e820ba-a5e0-4f66-953f-3d5881a98142)
#### U (Upper Immediate Operations):Instructions that use an immediate value for upper bits of a register.
- These instructions set the high bits of a register to a specific value. It's useful for loading big numbers into registers. Think of it as putting the first part of a big address on an envelope.
  
#### B (Branch Operations):Instructions that perform conditional branching based on comparison results.
- These instructions let the program make decisions and change its direction based on conditions. It's like choosing which path to take at a crossroad. For example, going left if two numbers are equal or going right if they're not.
  
#### J (Jump Operations):Instructions that perform unconditional jumping to a specified address.
- These instructions allow the program to jump to a different part of the code. It's like skipping ahead to a different page in a book. For instance, jumping to a function or looping back to repeat a section of code.
  
# Here's a table categorizing each mentioned instruction  into their respective types:
Sure, here's the table with instructions categorized by their types:

| Type | Instruction | Instruction Encoding |
|------|-------------|----------------------|
| R    | add         | 0000000 rs2 rs1 000 rd 0110011 |
| R    | sub         | 0100000 rs2 rs1 000 rd 0110011 |
| R    | and         | 0000000 rs2 rs1 111 rd 0110011 |
| R    | or          | 0000000 rs2 rs1 110 rd 0110011 |
| R    | xor         | 0000000 rs2 rs1 100 rd 0110011 |
| R    | slt         | 0000000 rs2 rs1 010 rd 0110011 |
| R    | sll         | 0000000 rs2 rs1 001 rd 0110011 |
| R    | srl         | 0000000 rs2 rs1 101 rd 0110011 |
| I    | addi        | imm[11:0] rs1 000 rd 0010011 |
| I    | lw          | imm[11:0] rs1 010 rd 0000011 |
| S    | store       | imm[11:5] rs2 rs1 010 imm[4:0] 0100011 |
| U    | lui         | imm[31:12] rd 0110111 |
| B    | branch      | imm[12] imm[10:5] rs2 rs1 imm[4:1] imm[11] 1100011 |
| B    | beq         | imm[12] imm[10:5] rs2 rs1 imm[4:1] imm[11] 1100011 |
| B    | bne         | imm[12] imm[10:5] rs2 rs1 imm[4:1] imm[11] 1100011 |
| J    | jal         | imm[20] imm[10:1] imm[11] imm[19:12] rd 1101111 |

# Each instruction is categorized in following instruction types:
- R (Register-Register Operations): ADD, SUB, AND, OR, XOR, SLT, SLL, SRL
- I (Immediate Operations): ADDI, LW
- S (Store Operations): STORE
- U (Upper Immediate Operations): LUI
- B (Branch Operations): BRANCH, BEQ, BNE
- J (Jump Operations): JAL
