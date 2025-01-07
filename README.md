# Samsung-RISC-V-Program
Karnataka's RISC-V Skilled Workforce Powered by Samsung Semiconductor India Research ,Kunal Ghosh(VSD) &amp; Co.

##  Basic Details

**Name:** Manish S  
**College:** DAYANANDA SAGAR COLLEGE OF ENGINEERING 
**Email ID:** manishs19022@gmail.com  
**GitHub Profile:** [Manishs19022](https://github.com/Manishs19022)  
**LinkedIN Profile:** [Manish S](https://www.linkedin.com/in/manish-s-06a880261/)

----------------------------------------------------------------------------------------------------------------

# FIRST TASK 
 Install this riscv tool chain on your machine. The labs related to first the above task will be shared over email. Complete this before the inauguration call on 6th Jan, 2025.

![image](https://github.com/user-attachments/assets/14a488f3-d020-40d0-9284-a7e524d1ad50)
 and further steps are attached as pdf.

<details>
<summary><b>Task 1:</b> Task is to install all the essential tools required for this internship such as Ubuntu on VMBox, GNU Toolchain, GTKWave, Yosys and iVerilog simulator</summary>   
<br>

**1. Install Ubuntu 20.04 LTS on Oracle Virtual Machine Box**

![Ubuntu and VMBox Installation](https://github.com/maazm007/vsdsquadron-mini-internship/assets/83294849/11c35aff-f587-40f5-a7d2-683dbf0784d4)

**2. Install RISC-V [GNU ToolChain](https://github.com/riscv-collab/riscv-gnu-toolchain)**

### What is RISC-V GNU Toolchain?
> The RISC-V GNU Compiler Toolchain is a free and open source cross-compiler for C and C++. It supports two build modes: Generic ELF/Newlib and Linux-ELF/glibc. The toolchain can be used to create assembly instructions and sequences for execution in a simulator and target FPGA  

*Use the following command to install GNU Toolchain*
```  
$ sudo apt install git  
$ git clone https://github.com/riscv/riscv-gnu-toolchain
$ sudo apt-get install autoconf automake autotools-dev curl python3 python3-pip libmpc-dev libmpfr-dev libgmp-dev gawk build-essential bison flex texinfo gperf libtool patchutils bc zlib1g-dev libexpat-dev ninja-build git cmake libglib2.0-dev libslirp-dev  
$ mkdir /opt/riscv
$ ./configure --prefix=/opt/riscv --with-arch=rv64i --with-abi=lp64 --enable-multilib
$ sudo make
```
Now add ```/opt/riscv/bin``` to **PATH**  
```
$ gedit ~/.bashrc  
````  
Add the line ```export PATH="$PATH:/opt/riscv/bin"``` in the end of file and save it. After that run the following command:  
```
$ source ~/.bashrc
```

![RISC-V GNU Toolchain Installation](https://github.com/maazm007/vsdsquadron-mini-internship/assets/83294849/2ca2294c-28f5-43dd-bf9d-41abf33c9d02)






 #  INAUGURATION MEET
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


