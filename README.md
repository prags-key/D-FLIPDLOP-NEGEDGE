# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement  D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

**Procedure**

```
1.Type the program in quartus software
2.Compile and run the program
3.Generate the RTL schematic and save the logic diagram
4.Create nodes for inputs and outputs to generate the things diagram
5.For different input combinations generate the timing diagram
```

**PROGRAM**

```
 module exp8(D,clk,Q,Qbar);
 input D,clk;
 output reg Q;
 output reg Qbar;
 initial Q=0;
 initial Qbar=1;
 always @(posedge clk)
 begin
 Q=D;
 Qbar=~D;
 end
 endmodule
 Program for flipflops and verify its truth table in quartus using Verilog programming.
 Developed by:PRAGATHI KUMAR
 RegisterNumber:24006285
```

**RTL LOGIC FOR FLIPFLOPS**
![Screenshot 2024-12-17 222106](https://github.com/user-attachments/assets/5149c7f5-09d7-460a-90fc-d2d57c58b447)
**TIMING DIGRAMS FOR FLIP FLOPS**
![Screenshot 2024-12-17 222140](https://github.com/user-attachments/assets/0909810a-4c42-4a68-b929-fc73f8e296a0)
**RESULTS**
 ```
Thus D flipflop using verilog was implemented and validated their functionality using their function table
```
