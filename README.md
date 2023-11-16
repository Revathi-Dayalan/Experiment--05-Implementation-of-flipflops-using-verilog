### Experiment--05-Implementation-of-flipflops-using-verilog
### AIM: To implement all the flipflops using verilog and validating their functionality using their functional tables
### HARDWARE REQUIRED: – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED: Quartus prime
# THEORY
## SR Flip-Flop
SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/3abaacf4-219c-4b47-9d04-e5a944fa29ad)


This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/bc76a12c-2dd5-4adf-84a2-07ec70395959)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/e9e6a0e3-be91-47dd-97b9-4ae6408ea7e3)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/80173dbf-a511-48e4-b478-c4d635ae5549)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

# D Flip-Flop
D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop. 
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/54b523ce-89d4-4332-8e21-8aeea0e0bd48)
following table shows the state table of D flip-flop
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/6c905839-b605-4bb4-94c3-ca2f643dc4bb)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/f09f791e-8eb6-49d8-8a0a-72c3b06be728)


Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

# JK Flip-Flop
JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure. 
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/0ae0831c-e718-4fee-ba15-e680193d4beb)


This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/b653fb78-1383-4de6-ab66-e037816a66b5)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/be01cede-2487-474b-b7ba-dea581bc9f0e)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/06aa140d-e849-47f3-88f7-84e30ae4c8a1)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

# T Flip-Flop
T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/f5df7fe1-41e7-4f31-a031-249012d8474a)


This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/229b28ab-a21c-4030-b709-74af1d632f54)


From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

# Procedure
1.Using nand gates and wires construct sr flip flop.

2.Repeat same steps to construct JK,D,T flipflops.

3.Find Rtl logic and timing diagram for all flipflops.

4.end the program.

# SR FLIPFLOP:
# PROGRAM 1

# Program for flipflops  and verify its truth table in quartus using Verilog programming.
```
Developed by: REVATHI.D
RegisterNumber: 212221240045
```
```
module sr (q,qbar,s,r,clk);
input s,r,clk;
output q,qbar;
wire nand1_out;
wire nand2_out;
nand(nand1_out,clk,s);
nand(nand2_out,clk,r);
nand(q,nand1_out,qbar);
nand(qbar,nand2_out,q);
endmodule
```
# RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/95fb70ce-74b2-4f91-8460-f5c00754ebfa)


# TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/aa0493e1-03fd-45a9-a6e6-8a1508294285)


# JK FLIPFLOP
# PROGRAM 2

# Program for flipflops  and verify its truth table in quartus using Verilog programming.
```
Developed by: REVATHI.D
RegisterNumber: 212221240045
```
```
module jk(q,qbar,k,j,clk);
input j,k,clk;
output q,qbar;
wire nand1_out;
wire nand2_out;
nand(nand1_out,j,clk,qbar);
nand(nand2_out,k,clk,q);
nand(q,nand1_out,qbar,qbar);
nand(qbar,nand2_out,q);
endmodule
```

## RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/63472b91-a00f-4653-b4af-bdab39ffbf0e)


## TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/c75ebf4b-9270-4859-bbbd-148163898de4)


# D FLIPFLOP
# PROGRAM 3
# Program for flipflops  and verify its truth table in quartus using Verilog programming.
```
Developed by: REVATHI.D
RegisterNumber: 212221240045
```

```
module d(q,qbar,d1,clk);
input d1,clk;
output q,qbar;
wire n1;
wire n2;
not(x,d1);
nand(n1,clk,d1);
nand(n2,clk,x);
nand(q,n2,qbar);
nand(qbar,n1,q);
endmodule
```
# RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/5b0bc2ca-7e0d-46f9-89b9-b01ea5225651)


# TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/cdb94659-5d0b-4edd-b4c1-b04fe161b8fd)


# T FLIPFLOP
# PROGRAM 4
# Program for flipflops  and verify its truth table in quartus using Verilog programming.
```
Developed by: REVATHI.D
RegisterNumber: 212221240045
```
```
module tff(t,qbar,q,clk);
input t,clk;
output q,qbar;
wire n1,n2;
nand(n1,t,clk,qbar);
nand(n2,clk,t,q);
nand(q,n1,qbar);
nand(qbar,n2,q);
endmodule
```
## RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/80c4f688-edaa-41a0-8b8e-cdfb2a19cf2e)


## TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/c89a549f-76aa-4210-8e58-89a8e91b9dec)


# RESULTS
Thus implementation of SR,JK,D and T flipflops using nand gates are done sucessfully
