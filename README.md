[VSDsquadron-Mini-Internship]
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

![b](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/a9039abb-1ab2-46bd-b0d1-f31db5b07f9b)  

#### B (Branch Operations):Instructions that perform conditional branching based on comparison results.
- These instructions let the program make decisions and change its direction based on conditions. It's like choosing which path to take at a crossroad. For example, going left if two numbers are equal or going right if they're not.

![j](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/e254f337-b25f-4393-a103-021a3241ad45)
  
#### J (Jump Operations):Instructions that perform unconditional jumping to a specified address.
- These instructions allow the program to jump to a different part of the code. It's like skipping ahead to a different page in a book. For instance, jumping to a function or looping back to repeat a section of code.
  
# Here's a table categorizing each mentioned instruction  into their respective types:

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
- 
# Task:3( April 27,2024)
## Checking out C-lab videos and running a simple c program to print sum of numbers.
This sample code prints the sum of integer numbers from 1 to n .
### #include <stdio.h>

### int main() {
### int i, sum=0, n=1606;
### for (i=1; i <= n; ++i) {
### sum += i;
###	}
### printf("Sum of numbers from 1 to %d is %d\n", n, sum);
### return 0;
### }
![Screenshot from 2024-05-05 01-45-43](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/37401937-1ef0-4042-bdd7-ba2861f77044)


## Checking out RISCV based lab videos and instructing the exact commands as shown to see the contents of main and compare output with object file.
In this task we tried out two type of instructions and saw the difference between them.
## First Instruction
# riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=riscv64i -o sum1ton.o sum1ton.c
## Second Instruction
![Screenshot from 2024-05-05 04-22-41](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/ece6fb58-e15c-4de0-802d-5ae935671f5b)

#  riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv641 -o sum1ton.o sum1ton.c
![2024-05-04 21_35_58-vsdworkshop  Running  - Oracle VM VirtualBox](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/81fca535-50d8-4eaa-8803-9ad780eb64cd)
![2024-05-04 21_40_34-vsdworkshop  Running  - Oracle VM VirtualBox](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/ceda3f47-22b4-4db3-a4ea-f553cfa0eee0)
# Task:4( May 05,2024)
The task 4 involves debugging the generated c output with the help of spike and pk. 
## Note: As there were issues in my system i used the virtual system provided by the vsd which had the required tools pre-installed .
Note:![Screenshot from 2024-05-05 04-24-21](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/d2eb4422-e977-4235-bb83-8691ac803fd4)

# Task:5( May 09,2024 )
## Task 5 included the 
### 1. creation of a directory in my own name for performing the assigned labs for this task.  
### 2. usage of open-source tools like Iverilog and GTKWave to analyze the provided Verilog Code.
### Both these tools were successfully installed in the Task:1 and here are there snapshots .
## GTK Waveform Viewer
![Screenshot from 2024-05-09 17-42-09](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/58d68657-457f-4d49-a8f8-292d48c7a56f)
## Icarus Verilog
 ![Screenshot from 2024-05-09 17-43-18](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/518bdcad-1e7c-4774-b72c-94d04bd09395)
## Running the simulations in GTK Waveform Viewer
![Screenshot from 2024-05-09 18-34-35](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/7c7fc76d-55d0-446d-8b35-b5defa143d15)
## Waveforms for various instruction set are shown below with their instructions:-

Instruction (a): ADD R6, R2, R1
![Screenshot from 2024-05-09 18-58-08](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/c9bcc2fc-ead0-4c2a-b32a-7b6205b801cd)
Instruction (b): SUB R7, R1, R2
![Screenshot from 2024-05-09 19-02-08](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/3e599299-8eca-40eb-9d08-8903ee5291ed)

Instruction (c): AND R8, R1, R3
![Screenshot from 2024-05-09 19-04-13](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/907ba9b9-3284-447f-8ee7-933d2b69851e)

Instruction (d): OR R9, R2, R5
![Screenshot from 2024-05-09 19-05-29](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/7499cc67-3c50-4f91-b0bc-ed6eb69a14df)
# Task:6(May 15,2024)
This task involved applying the knowledge and things that we got to know in above performed tasks. 
So, i tried to implement the LEDs brightness control using the VSD Squadron Mini.
The list of required components are as follows:-
| S.No. | Component                           | Quantity |
|-------|------------------------------------|----------|
| 1     | VSD Squadron Mini                  | 1        |
| 2     | Mini Breadboard                    | 1        |
| 3     | Connecting Wires                   | As needed|
| 4     | White 5mm LED                      | 1        |
| 5     | Blue 5mm LED                       | 1        |
| 6     | Green 5mm LED                      | 1        |
| 7     | Yellow 5mm LED                     | 1        |
| 8     | Orange 5mm LED                     | 1        |
| 9     | 330 Ohm Resistor                   | 5        |

# The hardware set-up is as shown in the below picture
![Setup for Led brightness control](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/ac441e1a-b9ed-4519-9353-294aab74b557)

| S.No. | Software             | Description                                        |
|-------|----------------------|----------------------------------------------------|
| 1     | MountRiver Studio    | Integrated development environment (IDE)          |
| 2     | CH32V003 Processor  | Microcontroller used for development               |
| 3     | RISC-V Architecture | Instruction set architecture used by the processor |

#  The development environment for the same is showing using the MounRiver Studio.
![IDE Setup](https://github.com/Savvian/VSD-Squadron-Mini-Internship/assets/90250807/2c54c91b-b8cc-4607-8bec-fc8fde98faa1)
