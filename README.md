# Samsung-RISC-V-Program
Karnataka's RISC-V Skilled Workforce Powered by Samsung Semiconductor India Research ,Kunal Ghosh(VSD) &amp; Co.

##  Basic Details

**Name:** Manish S  
**College:** DAYANANDA SAGAR COLLEGE OF ENGINEERING 

**Email ID:** manishs19022@gmail.com
**Phone :** 8867143816
**GitHub Profile:** [Manishs19022](https://github.com/Manishs19022)  
**LinkedIN Profile:** [Manish S](https://www.linkedin.com/in/manish-s-06a880261/)

----------------------------------------------------------------------------------------------------------------
##  INAUGURATION MEET
Inauguration meet on 6th Jan,2025.
Event Summary:

RISC-V Mission 2025 Powered by Samsung Semiconductor India Research in Collaboration with VLSI System Design

I am pleased and delighted to announce that we students of KARNATAKA are part of this remarkable initiative by Samsung Semiconductor India Research (SSIR) and VLSI System Design (VSD) under the RISC-V Mission 2025. This nation-building effort aims to create a skilled workforce of 1,000 RISC-V engineers across Karnataka, contributing to the vision of Digital India.

Here’s what makes this program a game-changer:
 1. 6-Week Training Program: A focused, hands-on cohort designed to equip participants with practical knowledge in RISC-V and semiconductor technologies.
 2. Perfect for Campus Aspirants: Specifically tailored for engineering students preparing for interviews, with a passion for entering the semiconductor industry.
3. FREE RISC-V Development Boards: VSD provides all participants with the right tools to empower innovation.

I sincerely thank Samsung Semiconductor India Research and VLSI System Design for giving us this incredible opportunity to explore and excel. This initiative inspires innovation and builds a strong foundation for students to become leaders in the semiconductor industry.

It’s an honour to contribute to this transformative mission and take a step toward becoming future RISC-V innovators.


# FIRST TASK 
 Install this riscv tool chain on your machine. The labs related to first the above task will be shared over email. Complete this before the inauguration call on 6th Jan, 2025.

![image](https://github.com/user-attachments/assets/14a488f3-d020-40d0-9284-a7e524d1ad50)

 and further steps are attached as pdf.


**1. Install Ubuntu 20.04 LTS on Oracle Virtual Machine Box**

![image](https://github.com/user-attachments/assets/817643ac-f806-4a34-8786-b82df2f8c123)


![VirtualBox_vsdworkshop_07_01_2025_15_27_37](https://github.com/user-attachments/assets/a2f619ff-83cb-4bd5-916b-5b38c4d24181)



![risc](https://github.com/user-attachments/assets/68059e43-e90e-4055-ae0a-a41eca6b8b4d)

![image](https://github.com/user-attachments/assets/94142f25-b461-4f32-9cb6-ea314285bc2f)


![image](https://github.com/user-attachments/assets/312f05f9-1147-473a-a2b9-d05292c0b76d)

# THIRD TASK

RISCV Instruction types
--

There are 6 types of instruction types in RISC-V types
 1.  R-Type (Register Type)
 2.  I-Type (Immediate Type)
 3.  S-Type (Store Type)
 4.  U-Type (Branch Type)
 5.  B-Type (Upper Immediate Type)
 6.  J-Type (Jump Type)

In the base RV32I ISA, there are four core instruction formats (R/I/S/U), as shown in Base instruction formats. All are a fixed 32 bits in length.

![image](https://github.com/user-attachments/assets/47b33518-df07-42ce-9922-4530c16492e9)

1.R-Type:
--
![image](https://github.com/user-attachments/assets/6bcad23c-667d-4fa1-ba98-e5c6d82f3b12)

  This diagram represents the R-Type instruction format in the RISC-V Instruction Set       
    Architecture (ISA). R-Type instructions are typically used for register-to-register operations
    Examples for R Type operation.  

| **funct7**  | **funct3** | **Operation**                        |
|-------------|------------|--------------------------------------|
| `0000000`   | `000`      | Add                                 |
| `0100000`   | `000`      | Sub                                 |
| `0000000`   | `001`      | Shift Left Logical (SLL)            |
| `0000000`   | `010`      | Set Less Than (SLT)                 |
| `0000000`   | `011`      | Set Less Than Unsigned (SLTU)       |
| `0000000`   | `100`      | XOR                                 |
| `0000000`   | `101`      | Shift Right Logical (SRL)           |
| `0100000`   | `101`      | Shift Right Arithmetic (SRA)        |
| `0000000`   | `110`      | OR                                  |
| `0000000`   | `111`      | AND                                 |

2.I-Type :
--
![image](https://github.com/user-attachments/assets/291e132c-afb6-46c2-a34c-9e46c2a845de)


I-Type instructions are used for operations involving immediate values, such as arithmetic with constants, memory access (e.g., loads), and control flow (e.g., jumps).

Common I -Type instructions :
-
| **Instruction** | **opcode** | **funct3** | **Description**                       |
|-----------------|------------|------------|---------------------------------------|
| `addi`          | `0010011`  | `000`      | Add immediate to register (`rd = rs1 + imm`). |
| `slti`          | `0010011`  | `010`      | Set if less than immediate (signed). |
| `andi`          | `0010011`  | `111`      | Bitwise AND with immediate.          |
| `lw`            | `0000011`  | `010`      | Load word from memory.               |
| `lh`            | `0000011`  | `001`      | Load halfword from memory.           |
| `jalr`          | `1100111`  | `000`      | Jump and link register (indirect jump). |

3.S-Type:
-
![image](https://github.com/user-attachments/assets/e69f40bc-c431-4334-b77a-a5f1286a4431)

 S-Type instructions are primarily used for store operations, where data from a register is stored into memory at a specified address.

Common S-Type Instructions
-
| **Instruction** | **opcode**  | **funct3** | **Description**                      |
|-----------------|-------------|------------|--------------------------------------|
| `sw`           | `0100011`   | `010`      | Store Word (32-bit).                |
| `sh`           | `0100011`   | `001`      | Store Halfword (16-bit).            |
| `sb`           | `0100011`   | `000`      | Store Byte (8-bit).                 |

4.U-Type :
-
![image](https://github.com/user-attachments/assets/fca113b5-0577-4955-a24f-d5454a9aa0a6)

U-Type format is used for instructions like LUI (Load Upper Immediate) and AUIPC (Add Upper Immediate to PC)

5.B-Type:
-
![image](https://github.com/user-attachments/assets/f332980d-bbbd-47aa-9635-fdc77de1d97f)

B-Type instructions enable branching (jumping) to another location in the code, determined by the offset in the instruction.These instructions check specific conditions and branch (jump) to a target address if the condition is satisfied. If the condition is not met, the program continues with the next sequential instruction.

Examples in B-Type:

| **Instruction** | **`funct3` Value** | **Condition**                   |
|------------------|---------------------|----------------------------------|
| `BEQ`           | `000`              | Branch if `rs1 == rs2`.         |
| `BNE`           | `001`              | Branch if `rs1 != rs2`.         |
| `BLT`           | `100`              | Branch if `rs1 < rs2` (signed). |
| `BGE`           | `101`              | Branch if `rs1 >= rs2` (signed).|
| `BLTU`          | `110`              | Branch if `rs1 < rs2` (unsigned).|
| `BGEU`          | `111`              | Branch if `rs1 >= rs2` (unsigned).|

6.J-Type:
-
![image](https://github.com/user-attachments/assets/5fa4d127-0de3-45e7-8305-d116a979ebae)

J-Type instructions are used for unconditional jumps ,these are also  used for control flow, such as implementing function calls or jumping to a specific instruction.

Common J-Type instructions:
-

| **Instruction** | **Opcode (Bits 6–0)** | **Registers** | **Description**                           |
|------------------|-----------------------|---------------|-------------------------------------------|
| `JAL`           | `1101111`            | `rd`          | Jump and Link: Save return address and jump to target address |


## 32-bit instructions from application (counterdown clock):

![15 instr](https://github.com/user-attachments/assets/025ed997-7162-426f-aa1a-eaac5449bad6)

1.jal ra,10184
-
J-Type (Jump)

imm[20|10:1|11|19:12] | rd | opcode

- *opcode* = 1101111

- *rd* = x1 (ra)

- *imm* = 10184

- *imm[20]* = 0

- *imm[10:1]* = 1111101000

- *imm[11]* = 1

- *imm[19:12]* = 1100
32-bit representation:

``000000110011001001 | 00001 | 1101111``

