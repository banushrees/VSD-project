# TASK 4

## Identify the various type of instruction set in RISC V processor

RISC V  processor has various type of instruction set named;
R -Type,I -Type,S - Type,B -Type,U -Type,J-Type

![Screenshot 2024-07-02 200559](https://github.com/banushrees/VSD-project/assets/105593083/fc689370-4260-44b9-9011-416db18d9d3a)

### R -TYPE:
 It is an register type , it works only on the registers.It is primarily used for arithmetic and logical operations.

### I- TYPE:
 It is type of instruction used for operations having immediate value (constant number) and register.

 ### S -TYPE:
  It is type of instruction used for operations involving storing of data from a register to a memory.

 ### B-TYPE :
 It is type of instruction used for conditional branching of a program.it will allow the program to jump to different part of code if a specified condition is met. 

### U- TYPE:
 It is type of instruction used to work with the large numbers. they put large type of number into a specfic part of the register.

### J-TYPE:
  It is used for performing unconditional jumps in a program.

32 Bit instruction code for each instruction
1.ADD r1,r2,r3
  - opcode: 0110011
  - rd: 00001
  - funct3: 000
  - rs1: 00010
  - rs2: 00011
  - funct7 :0000000

32 BIT  INSTRUCTION CODE: `0000000 00011 00010 000 00001 0110011`  

2. SUB r3,r1,r2
  - opcode: 0110011
  - rd: 00011
  - funct3: 000
  - rs1: 00001
  - rs2: 00010
  - funct7 :0100000
    
 32 BIT  INSTRUCTION CODE:`0100000 00010 00001  000 00011 0110011 ` 

 3. ADD r2,r1,r3:
    
  - opcode: 0110011
  - rd: 00010
  - funct3: 111
  - rs1: 00001
  - rs2: 00011
  - funct7 :0000000
    
 32 BIT  INSTRUCTION CODE:`0000000 00011 00001 111 00010 0110011`

 4. OR r8,r2 ,r5:

  - opcode: 0110011
  - rd: 01000
  - funct3: 110
  - rs1: 00010
  - rs2: 00101
  - funct7 :0000000
    
 32 BIT  INSTRUCTION CODE:`0000000 00101 00010 110 01000 0110011 `

5. XOR r8,r1,r4
     
  - opcode: 0110011
  - rd: 01000
  - funct3: 100
  - rs1: 00001
  - rs2: 00100
  - funct7 :0000000
    
 32 BIT  INSTRUCTION CODE:`0000000 00100 00001 01000 0110011`

 6.SLT r10,r2,r4:
   
 - opcode: 0110011
  - rd: 01010
  - funct3: 010
  - rs1: 000010
  - rs2: 00100
  - funct7 :0000000
    
 32 BIT  INSTRUCTION CODE:`0000000 00100 00010 010 01010 0110011 ` 

 7. ADDI r12 ,r3 ,5

  - opcode: 0110011
  - rd: 01100
  - funct3: 000
  - rs1: 00011
  - imm:000000000101

 32 BIT  INSTRUCTION CODE:`000000000101 00011 000 01100 0010011 ` 

 8. SW r3,r1,4
  - opcode: 0110011
  - imm[4:0]:  00100
  - funct3: 010
  - rs1: 00001
  - rs2: 00011
  - imm [11:5] :0000000
    
 32 BIT  INSTRUCTION CODE:`0000000 00011 00001 010 00100 0100011 ` 
 
 9. SRL r16,r11,r2
 
  - opcode: 0110011
  - rd: 10000
  - funct3: 101
  - rs1: 01011
  - rs2: 00010
  - funct7 :0000000
    
 32 BIT  INSTRUCTION CODE:`0000000 00010 01011 101 10000 0110011 ` 

10.BNE r0,r1,20

  - opcode: 1100011
  - imm[12|10:5]: 0000001
  - funct3: 001
  - rs1: 00001
  - rs2: 00000
  - imm[4:1|11] :01000
    
 32 BIT  INSTRUCTION CODE:`0000001  00001 00000 001 0100 01100011 ` 

 11. BEQ r0,r0,15:
     
  - opcode: 1100011
  - funct3: 000
  - rs1: 00000
  - rs2: 00000
  - imm [11:0]:15
    
 32 BIT  INSTRUCTION CODE:`00000000 00001111 00000 00000 000 1100011 `

 12.LW r13,r11,2:

  - opcode: 0000011
  - rd: 01101
  - funct3: 010
  - rs1: 01011
  - imm :00010
    
 32 BIT  INSTRUCTION CODE:`0000000 00010 01011 010 01101 0000011`

 13.SLL r15,r11,r2:

  - opcode: 0110011
  - rd: 01111
  - funct3: 001
  - rs1: 01011
  - rs2: 00010
  - funct7 :0000000

 32 BIT  INSTRUCTION CODE:`0000000 00010 01011 001 01111 0110011 ` 

   


  
  
  


