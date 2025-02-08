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



 C-Based Lab
 ----
Install leafpad editor for C programming using command

 ```
         sudo apt  install leafpad
 ```
 ![install leafpad](https://github.com/user-attachments/assets/69a4702e-69e4-494d-8bb0-4a9f347eee5b)

Write a program that gives the sum of n numbers using C in leafpad editor."sum1ton.c" is the filename

 ![overleaf sum1ton](https://github.com/user-attachments/assets/9b683e34-7296-4785-889d-fc1b85038656)




  Run the program and check the results using commands
 ````
gcc sum1ton.c
./a.out 
````
./a.out is used for result

result :

![c result ](https://github.com/user-attachments/assets/78b285ae-7b20-4409-acd1-4d8e9ebccf8c)

RISC -V Based Lab
----
Now we are compiling the same code in RISCV 
compiling using command ```cat sum1ton.c```

![risc1](https://github.com/user-attachments/assets/5e31f14d-e508-4d95-bd6d-167a52d6333a)

For compiling the above C code in RISCV use command 
```
 riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
```

# SECOND TASK

Spike Simulation:
--------- 
`Spike` is the official RISC-V ISA (Instruction Set Architecture) simulator. It allows developers to simulate RISC-V programs and applications, providing an environment to run, test, and debug code designed for RISC-V-based processors. Spike is commonly used in the context of development and research related to RISC-V architecture.

`GCC (GNU Compiler Collection)` is a popular set of compilers that supports a variety of programming languages, including C and C++. In the context of RISC-V, GCC can be used to compile code for RISC-V targets, and Spike can then simulate the execution of that code on a virtual RISC-V machine.

Now we use the command `spike pk sum1ton.o` give the output of the C code and verifies the instructions are correct

![Screenshot from 2024-11-25 11-42-08](https://github.com/user-attachments/assets/e369d5bb-0bb3-4ec5-92a7-fdf1847afa2e)

Debugg Assembly Language Program using ``spike -d pk sum1ton.o`` 

Assembly Language Program :

![assemblylang](https://github.com/user-attachments/assets/75bdb822-76cd-4b17-8913-4f573dcbfdd4)

Debugger:

![match sp](https://github.com/user-attachments/assets/1d6583a8-e92a-4ae1-a792-40461e99a1e4)

-O1 and -Ofast 
-

The `-O1` and `-Ofast` options in the context of compiling C code with RISC-V (or any GCC-compatible compiler) control the level and type of optimizations applied during the compilation process

In the case of `-O1` it  focus  A moderate level of optimization that aims to improve code performance while keeping compilation times and memory usage reasonable.

In the case of `-Ofast` it focus  Aggressively optimizes for maximum performance, often at the expense of strict adherence to the language standard and longer compilation times.

Application:
--


C-program using Leafpad :
-

![counterdown leafpad](https://github.com/user-attachments/assets/5eb13062-6041-481f-9971-946d5169e903)

output of C code is :

![c out counterdown](https://github.com/user-attachments/assets/9753cb5a-5902-45a3-959a-8a3c3c8ac925)

compilation using gcc :

![counterdown using gcc](https://github.com/user-attachments/assets/6c1c059b-38ec-45b6-98ee-10562faaaff7)

Assembly Language program for the above C code: 


![Assembly language counterdown](https://github.com/user-attachments/assets/e42643af-fc6c-4bcb-9d62-acd4bdd7d234)

Debugging all the instructions in the Assembly language program using spike 

![debug using spike](https://github.com/user-attachments/assets/421d1e4f-ab7c-42fe-8ca9-2897a80975da)


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

2.ld a5,88(a0)
-
I-Type (Load, RV64I)

imm[11:0] | rs1 | funct3 | rd | opcode

- *opcode* = 0000011

- *funct3* = 011 (ld)

- *rd* = x15 (a5)

- *rs1* = x10 (a0)

- *imm* = 88 (000000010110)

32 - bit representation:

``00000001011001010 |011 |   01111 |   0000011``

3.jalr a5
-
I-Type (Jump Register)

imm[11:0] | rs1 | funct3 | rd | opcode

- *opcode* = 1100111

- *funct3* = 000 (jalr)

- *rd* = x15 (a5)

- *rs1* = x15 (a5)

- *imm* = 0

32 - bit-representation:

``00000000000001111 | 000  |   01111  | 1100111``
4.sd a6, 80(sp)
-
S-Type Instruction

- *imm[11:5]*	0000001

- *rs2*	00110 (a6)

- *rs1*	00001 (sp)

- *funct3*	011 (sd)

- *imm[4:0]*	01000

- *opcode*	0100011

32- bit representation:

``00000010011000001 | 011 | 00001 | 0100011``

5.lui a3, 0xffff
-
U-Type Instruction

*imm[31:12]*	111111111111

- *rd*	00011 (a3)

- *opcode*	0110111

32- bit representation:

``111111111111 | 00011 | 0110111``


6.srai s2,s2,0x3
-
I-Type Instruction

imm[11:0] | rs1 | funct3 | rd | opcode

- *imm[11:5]*	0100000

- *imm[4:0]*	00011 (shift amount = 3)

- *rs1*	10010 (s2)

- *funct3*	101 (srai)

- *rd*	10010 (s2)

- *opcode*	0010011

32 - bit representation:

``01000000001110010 | 101 | 10010 | 0010011``

7.bne s2, s1, 10330
-
B-Type (Conditional Branch)

imm[12|10:5] | rs2 | rs1 | funct3 | imm[4:1|11] | opcode

- *opcode* = 1100011


- *funct3* = 001 (bne)

- *rs1* = x18 (s2)

- *rs2* = x9 (s1)

- *imm* = 10330, split as:

- *imm[12]* = 1

- *imm[10:5]* = 100011

- *imm[4:1]* = 0101

- *imm[11]* = 0

32 - bit representation:

``1| 100011   |   01001  |10010 |  001  |  0101| 0  | 1100011``

8.auipc a5, 0xfffff0
---------
U-Type (Upper Immediate)

imm[31:12] | rd | opcode

- *opcode* = 0010111

- *rd* = x15 (a5)

- *imm* = 0xfffff0 (11111111111100000)

32 - bit representation:

``11111111111100000 | 01111 | 0010111``

9.beqz a5, 100c8 <register_fini+0x18>
-
beqz is a pseudo-instruction for beq a5, x0, offset.
It checks if a5 is equal to 0 (x0) and branches to the offset 100c8.

- *imm[12]*	1

- *imm[10:5]*	000110

- *rs2*	00000

- *rs1*	01111

- *funct3*	000

- *imm[4:1]*	1010

- *imm[11]*	1

- *opcode*	1100011

32-bit representation:

``10001000000011110 | 000 | 01010 | 1100011``

10.li a0, 0
-
I-Type Instruction

- *imm[11:0]*	000000000000 (0)

- *rs1*	00000 (zero)

- *funct3*	000 (addi)

- *rd*	01010 (a0)

- *opcode*	0010011

32-bit representation:

``00000000000000000 | 000 | 01010 | 0010011``

11.bnez s1, 102a0
-
B-Type Instruction

- *imm[12]*	0

- *imm[10:5]*	100010

- *rs2*	00000 (zero)

- *rs1*	01001 (s1)

- *funct3*	001 (bne)

- *imm[4:1]*	0001

- *imm[11]*	1

- *opcode*	1100011

32 - bit representation:

``00001000101010001 | 001 | 00101 | 1100011``


12.or a2, a4, -4(a4)
-
R-Type Instruction

- *rs2*	00100 (a4)

- *rs1*	00100 (a4)

- *funct3*	000 (or)

- *rd*	00010 (a2)

- *funct7*	0000000

- *opcode*	0110011

32- bit representation:

``000000000100 | 00100 | 000 | 00010 | 0110011 ``

13.lbu a2,-4(a4)
-
I-Type  Instruction:

- *imm[11:0]*	111111111100

- *rs1*	01000 (a4)

- *funct3*	100 (lbu)

- *rd*	00010 (a2)

- *opcode*	0000011

32- bit reprsentation:

``111111111100 | 01000 | 100 | 00010 | 0000011``

14 . addi sp,sp -32
-
I-Type Instruction

imm[11:0] | rs1 | funct3 | rd | opcode

- *opcode* = 0010011

- *funct3* = 000 (addi)

- *rd* = x2 (sp)

- *rs1* = x2 (sp)

- *imm* = -32 (signed 12-bit: 111111111110)

32 - bit representation:

``11111111111000010 |  000  |   00010 |  0010011``

15.lw a5,12(sp)
-
I-Type Instruction

imm[11:0]  | rs1   | funct3 | rd    | opcode

- *imm[11:0]*	000000001100 (12)

- *rs1*	00010 (sp)

- *funct3*	010 (lw)

- *rd*	01111 (a5)

- *opcode*	0000011

32-bit representation:

``00000000110000010 | 010 | 01111 | 0000011``


# FOURTH TASK 

In this task, we will perform functional simulation of RISC-V instructions modeled as a Verilog netlist and observe the output waveforms

Installing iverilog using command ``sudo apt install iverilog gtkwave``

![iverilog install](https://github.com/user-attachments/assets/9450ad57-a250-4055-bdb8-511628e50a0a)

1.``ADD R6, R2, R1``

![add gtk](https://github.com/user-attachments/assets/19a0d4f4-a836-4880-8fbc-0b359449b384)

2.``SUB R7, R1, R2``

![sub gtkwave](https://github.com/user-attachments/assets/0aa6192b-4f81-4604-b09d-e1f1d7617324)

3.``AND R8, R1, R3``

![and gtkwave](https://github.com/user-attachments/assets/fac6962c-000a-4f88-b7ba-61d542f1087c)

4.``OR R9, R2, R5``

![or gtkwave](https://github.com/user-attachments/assets/f1bad13c-7453-48cf-b5c8-89fecd460315)

5.``XOR R10, R1, R4``

![xor gtkwave](https://github.com/user-attachments/assets/159a1b56-4811-4261-9102-7cf9d3819b69)



# FIFTH TASK

Countdown counter:
--
Countdown counter application is designed for an embedded system using a 4x4 matrix keypad and an I2C-based LCD display. It allows users to set a countdown timer in seconds, display the time remaining on the LCD.

Users can input a countdown time (up to 4 digits, in seconds) using the numeric keys (0-9) on the keypad. After entering the desired countdown time, the user presses the` #` key to start the countdown.The LCD shows the time remaining in seconds, which updates every second during the countdown.Users can press the `*` key to reset the timer back to zero. The LCD will display a "Time reset" message.
When the countdown reaches zero, the LCD displays "Time's Up!" to indicate that the timer has finished.After the countdown finishes, users can enter a new time for another countdown cycle. The system continuously waits for input.

Components requried for Application:
-
1.VSDSquadron Mini

2.4x4 Matrix keypad

3.I2c Lcd display

4.Jumper Wires

5.VS Code 

6.PlatformIO IDE

Vsd_Squadronmini:
--

![image-removebg-preview (5)](https://github.com/user-attachments/assets/a63ce851-c985-4a77-88ce-3f7c9678e50d)

Hardware connections:
--
## **Matrix Keypad Connections**

| **Keypad Wire** | **Function** | **VSD Squadron Mini Pin** | **Description**       |
|------------------|--------------|---------------------------|-----------------------|
| Wire 8          | Row 1        | PD7                       | Connects to GPIO PD7  |
| Wire 7          | Row 2        | PD2                       | Connects to GPIO PD2  |
| Wire 6          | Row 3        | PD3                       | Connects to GPIO PD3  |
| Wire 5          | Row 4        | PD4                       | Connects to GPIO PD4  |
| Wire 4          | Column 1     | PC4                       | Connects to GPIO PC4  |
| Wire 3          | Column 2     | PC5                       | Connects to GPIO PC5  |
| Wire 2          | Column 3     | PC6                       | Connects to GPIO PC6  |
| Wire 1          | Column 4     | PC7                       | Connects to GPIO PC7  |

---

## **I2C LCD Display Connections**

| **Pin** | **Function**  | **VSD Squadron Mini Pin** | **Description**        |
|---------|---------------|----------------------------|------------------------|
| GND (1) | Ground        | GND                       | Ground connection      |
| VCC (2) | Power         | 5V                        | Power supply (5V)      |
| SDA (3) | I2C Data Line | PC1                       | Connects to GPIO PC1   |
| SCL (4) | I2C Clock Line| PC2                       | Connects to GPIO PC2   |

Circuit Diagram:
--

![countdown counter](https://github.com/user-attachments/assets/33100501-6150-45bd-a0d1-32319e365b23)



Implemtation of Countdown Counter using Vsdsquadron-Mini , I2c Lcd display and Keypad    
-

Application overview :
-
-  keypad allows the user to input a 4-digit number for the countdown timer.
-  When the user presses the # key, the 4-digit input is converted into a countdown value (in seconds), and the timer starts counting down , the remaining time is displayed on the LCD.
-  User can press the * key at any time to restart the application, clearing the display and prompting the user to enter a new 4-digit countdown value.
-  I2C protocol is used to control the LCD, allowing for clear and dynamic updates during the countdown process.

Code:
-

 
```
#include <ch32v00x.h>
#include <ch32v00x_gpio.h>
#include <stdio.h>  // For sprintf

// Define Keypad pins
#define R1 GPIO_Pin_5 // PD7
#define R2 GPIO_Pin_2 // PD2
#define R3 GPIO_Pin_3 // PD3
#define R4 GPIO_Pin_4 // PD4
#define C1 GPIO_Pin_4 // PC4
#define C2 GPIO_Pin_5 // PC5
#define C3 GPIO_Pin_6 // PC6
#define C4 GPIO_Pin_7 // PC7

// Onboard LED pin (PD6)
#define LED_PIN GPIO_Pin_6

// Define the SDA and SCL Pins for I2C Communication
#define SDA_PIN GPIO_Pin_1
#define SCL_PIN GPIO_Pin_2

// LCD I2C Address
#define LCD_Address 0x27

// Function Prototypes
void GPIO_INIT(void);
char keypad_get_key(void);
void delay_ms(uint32_t ms);
void i2c_start(void);
void i2c_stop(void);
void i2c_write(unsigned char data);
void i2c_ACK(void);
void lcd_send_cmd(unsigned char cmd);
void lcd_send_data(unsigned char data);
void lcd_send_string(const char *str);
void lcd_init(void);
void restart_application(void);

// GPIO Initialization for Keypad and LCD
void GPIO_INIT(void) {
    GPIO_InitTypeDef GPIO_InitStructure;

    // Enable clocks for GPIO ports C and D
    RCC_APB2PeriphClockCmd(RCC_APB2Periph_GPIOC | RCC_APB2Periph_GPIOD, ENABLE);

    // Initialize rows (R1-R4 on PD) as output
    GPIO_InitStructure.GPIO_Pin = R1 | R2 | R3 | R4;
    GPIO_InitStructure.GPIO_Mode = GPIO_Mode_Out_PP;
    GPIO_InitStructure.GPIO_Speed = GPIO_Speed_50MHz;
    GPIO_Init(GPIOD, &GPIO_InitStructure);

    // Initialize columns (C1-C4 on PC) as input pull-up
    GPIO_InitStructure.GPIO_Pin = C1 | C2 | C3 | C4;
    GPIO_InitStructure.GPIO_Mode = GPIO_Mode_IPU;
    GPIO_Init(GPIOC, &GPIO_InitStructure);

    // Initialize LED pin (PD6) as output push-pull
    GPIO_InitStructure.GPIO_Pin = LED_PIN;
    GPIO_InitStructure.GPIO_Mode = GPIO_Mode_Out_PP;
    GPIO_InitStructure.GPIO_Speed = GPIO_Speed_50MHz;
    GPIO_Init(GPIOD, &GPIO_InitStructure);

    // Initialize I2C Pins
    RCC_APB2PeriphClockCmd(RCC_APB2Periph_GPIOC, ENABLE);
    GPIO_InitStructure.GPIO_Pin = SDA_PIN | SCL_PIN;
    GPIO_InitStructure.GPIO_Mode = GPIO_Mode_Out_OD;
    GPIO_InitStructure.GPIO_Speed = GPIO_Speed_50MHz;
    GPIO_Init(GPIOC, &GPIO_InitStructure);

    // Initialize LCD
    lcd_init();
}

// Delay Function
void delay_ms(uint32_t ms) {
    while (ms--) {
        for (uint32_t i = 0; i < 4000; i++) {
            __NOP(); // No operation, just a delay
        }
    }
}

// Keypad scan function
char keypad_get_key(void) {
    const char keys[4][4] = {
        {'1', '2', '3', 'A'},
        {'4', '5', '6', 'B'},
        {'7', '8', '9', 'C'},
        {'*', '0', '#', 'D'}
    };

    // Row pins array
    GPIO_TypeDef* row_ports[] = {GPIOD, GPIOD, GPIOD, GPIOD};
    uint16_t rows[] = {R1, R2, R3, R4};

    // Column pins array
    GPIO_TypeDef* col_ports[] = {GPIOC, GPIOC, GPIOC, GPIOC};
    uint16_t cols[] = {C1, C2, C3, C4};

    // Scan rows
    for (int row = 0; row < 4; row++) {
        // Set all rows high
        for (int r = 0; r < 4; r++) {
            GPIO_WriteBit(row_ports[r], rows[r], Bit_SET);
        }

        // Pull current row low
        GPIO_WriteBit(row_ports[row], rows[row], Bit_RESET);

        // Check each column
        for (int col = 0; col < 4; col++) {
            if (GPIO_ReadInputDataBit(col_ports[col], cols[col]) == RESET) {
                return keys[row][col]; // Return pressed key
            }
        }
    }
    return '\0'; // No key pressed
}

// I2C Start Condition
void i2c_start(void) {
    GPIO_SetBits(GPIOC, SDA_PIN);
    GPIO_SetBits(GPIOC, SCL_PIN);
    delay_ms(1);
    GPIO_ResetBits(GPIOC, SDA_PIN);
    delay_ms(1);
    GPIO_ResetBits(GPIOC, SCL_PIN);
    delay_ms(1);
}

// I2C Stop Condition
void i2c_stop(void) {
    GPIO_ResetBits(GPIOC, SDA_PIN);
    delay_ms(1);
    GPIO_SetBits(GPIOC, SCL_PIN);
    delay_ms(1);
    GPIO_SetBits(GPIOC, SDA_PIN);
    delay_ms(1);
}

// I2C Write Byte
void i2c_write(unsigned char data) {
    for (int i = 0; i < 8; i++) {
        if (data & 0x80) {
            GPIO_SetBits(GPIOC, SDA_PIN);
        } else {
            GPIO_ResetBits(GPIOC, SDA_PIN);
        }
        delay_ms(1);
        GPIO_SetBits(GPIOC, SCL_PIN);
        delay_ms(1);
        GPIO_ResetBits(GPIOC, SCL_PIN);
        data <<= 1;
    }
    // Release SDA for ACK
    GPIO_SetBits(GPIOC, SDA_PIN);
    delay_ms(1);
    GPIO_SetBits(GPIOC, SCL_PIN);
    delay_ms(1);
    GPIO_ResetBits(GPIOC, SCL_PIN);
    delay_ms(1);
}

// LCD Initialization
void lcd_init(void) {
    lcd_send_cmd(0x02); // Initialize in 4-bit mode
    lcd_send_cmd(0x28); // Function set: 4-bit, 2 lines, 5x7 font
    lcd_send_cmd(0x0C); // Display ON, Cursor OFF
    lcd_send_cmd(0x06); // Entry mode set: Increment cursor
    lcd_send_cmd(0x01); // Clear display
    delay_ms(20);       // Wait for the clear command
}

// Send Command to LCD
void lcd_send_cmd(unsigned char cmd) {
    unsigned char cmd_u = (cmd & 0xF0);
    unsigned char cmd_l = ((cmd << 4) & 0xF0);

    i2c_start();
    i2c_write(LCD_Address << 1);
    i2c_write(cmd_u | 0x0C); // Enable, RS = 0
    i2c_write(cmd_u | 0x08); // Disable, RS = 0
    i2c_write(cmd_l | 0x0C); // Enable, RS = 0
    i2c_write(cmd_l | 0x08); // Disable, RS = 0
    i2c_stop();
    delay_ms(2);
}

// Send Data to LCD
void lcd_send_data(unsigned char data) {
    unsigned char data_u = (data & 0xF0);
    unsigned char data_l = ((data << 4) & 0xF0);

    i2c_start();
    i2c_write(LCD_Address << 1);
    i2c_write(data_u | 0x0D); // Enable, RS = 1
    i2c_write(data_u | 0x09); // Disable, RS = 1
    i2c_write(data_l | 0x0D); // Enable, RS = 1
    i2c_write(data_l | 0x09); // Disable, RS = 1
    i2c_stop();
    delay_ms(2);
}

// Send String to LCD
void lcd_send_string(const char *str) {
    while (*str) {
        lcd_send_data(*str++);
    }
}

// Restart Application
void restart_application(void) {
    // Reinitialize all GPIOs and LCD
    GPIO_INIT();

    // Clear the digits array
    char digits[4] = {' ', ' ', ' ', ' '};

    lcd_send_cmd(0x80); // Move cursor to first row, first column
    lcd_send_string("Start Timer!");
    delay_ms(2000);  // Display for 2 seconds

    lcd_send_cmd(0x80); // Move cursor to first row, first column
    lcd_send_string("Enter 4 Digits:");
}

// Main Function
int main(void) {
    GPIO_INIT();

    lcd_send_cmd(0x80); // Move cursor to first row, first column
    lcd_send_string("Start Timer!");

    delay_ms(2000);  // Display for 2 seconds

    lcd_send_cmd(0x80); // Move cursor to first row, first column
    lcd_send_string("Enter 4 Digits:");

    char digits[4] = {' ', ' ', ' ', ' '};  // Array to store the last 4 digits
    int digit_count = 0;

    while (1) {
        char key = keypad_get_key();

        // If any key is pressed
        if (key != '\0') {
            // If # is pressed, convert the digits to integer and count down
            if (key == '#') {
                // Convert the digits array to an integer
                int num = (digits[0] - '0') * 1000 + (digits[1] - '0') * 100 + 
                          (digits[2] - '0') * 10 + (digits[3] - '0');

                // Countdown from the number to 0
                for (int i = num; i >= 0; i--) {
                    if (i == 0) {
                        lcd_send_cmd(0xC0); // Move cursor to second row
                        lcd_send_string("Time left: 0 sec");
                        delay_ms(500);  // Wait before updating the LCD
                        lcd_send_cmd(0x01); // Clear display
                        lcd_send_cmd(0x80); // Move cursor to top row
                        lcd_send_string("Time's Up!");
                        delay_ms(2000);  // Display "Time's Up!" for 2 seconds
                        // Clear display
                        lcd_send_cmd(0x01); // Clear display
                        // Show restart message
                        lcd_send_cmd(0x80); // Move cursor to top row
                        lcd_send_string("* to restart");
                        break;
                    } else {
                        char buffer[16];
                        sprintf(buffer, "Time left:%d sec", i); // Format countdown as "Time left: <value> sec"
                        lcd_send_cmd(0xC0); // Move cursor to second row
                        lcd_send_string(buffer);
                        delay_ms(500);  // Wait before updating the LCD
                        lcd_send_cmd(0x01); // Clear display
                    }
                }
            } else {
                // Shift the digits to the left and add the new key
                for (int i = 0; i < 3; i++) {
                    digits[i] = digits[i + 1];
                }
                digits[3] = key;

                // Display the digits on the LCD
                lcd_send_cmd(0xC0); // Move cursor to second row
                lcd_send_data(digits[0]);
                lcd_send_data(digits[1]);
                lcd_send_data(digits[2]);
                lcd_send_data(digits[3]);

                delay_ms(200);  // Small delay to avoid bouncing
            }
        }

        // Check for "*" to restart
        if (key == '*') {
            restart_application();
        }
    }
}
```

# REFFERENCE 

https://docs.cirkitdesigner.com/component/fba59254-fd55-44ac-b7e5-3f30f07ff53f/vsdsquadron-mini
