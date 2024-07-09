# TASK -5
 ##  Use this RISC-V Core Verilog netlist and testbench for functional simulation experiment. Upload waveform snapshots for the commands for the given instuction sets.

 ### steps to get the waveform for the given instructions:
 
 
  1.create the directory ( task 6) and write the  veroilog code and testbench in indivitual folders(task_rv32i.v & task_rv32i_tb.v)
  
   2. run the code with iverilog command 
     `iverilog -o task_rv32i task_rv32i.v task_rv32i_tb.v`
     
   3. A dumpfile withthe vcd format will be created (iiitb_rv32i.vcd)
     
   4. open the gtkwave for opening the waveform
      `gtkwave iiitb_rv32i.vcd`

select the instruction set from EX_MEM_IR[31:0]  
  ### INTRCTIONS AND ITS WAVEFORMS:

  ADD r6,r1,r2

  ![addr r6,r1,r2](https://github.com/banushrees/VSD-project/assets/105593083/c0cce9a3-20fe-4f47-9018-7bab1cefef5d)

  SUB r3,r1,r2

  ![sub r3,r1,r2](https://github.com/banushrees/VSD-project/assets/105593083/9a71b052-b76e-4ca9-acb1-0ceea0c25efe)

  AND r2,r1,r3

  ![and r2,r1,r3](https://github.com/banushrees/VSD-project/assets/105593083/900388fe-ba30-46ce-8c49-ff44a912c5f6)

  OR r8,r1,r4
  
   ![or r8,r1,r4](https://github.com/banushrees/VSD-project/assets/105593083/36795868-1135-4992-ac3a-c5b2e5f9735f)

   XOR r8,r1,r4

   ![xor r8 ,r1,r4](https://github.com/banushrees/VSD-project/assets/105593083/2211bc6a-0b32-42fa-91da-c7107b789dbb)

   SLT r10,r2,r4

  ![SLT r10,r2,r4](https://github.com/banushrees/VSD-project/assets/105593083/5f512e0d-aae4-45bd-b428-629134cd12aa)

  ADDL r12,r3,5
  
   ![addl r12,r3,5](https://github.com/banushrees/VSD-project/assets/105593083/681dbb7d-116b-4a8e-a3fe-5af8848d13c2)

   SW r3,r1,4

   ![SW ,r3,r1,4](https://github.com/banushrees/VSD-project/assets/105593083/66c46611-7fdd-4801-9f7b-5dafc9c52801)

   SLL r15,r11,r2

  ![SLL r15,r11,r2](https://github.com/banushrees/VSD-project/assets/105593083/b6612d4e-3659-400d-a5e8-25954851ed8d)


    



     
  

