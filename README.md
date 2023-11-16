Experiment-05 Implementation of flipflops using verilog
AIM: To implement all the flipflops using verilog and validating their functionality using their functional tables
HARDWARE REQUIRED: – PC, Cyclone II , USB flasher
SOFTWARE REQUIRED: Quartus prime
THEORY
SR Flip-Flop SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/e599aec4-b727-4435-b275-704d736f37a2)


This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/c5c80c66-f9b5-4794-b6f0-41921c12b70b)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/72ed767a-623f-412c-b3c2-122214759556)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/2eda95b5-d7c0-445e-b5e0-c40da336efca)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

D Flip-Flop
D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop. image

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/380f45de-da78-4aa2-9c59-38303ab6def5)
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/6ddc8fe6-b1f8-4833-9b54-040862cedd5b)


Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/d8d3db50-31f6-4182-918d-effb1c9e5082)


Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

JK Flip-Flop
JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure. ![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/6fc1904b-caea-4928-acaf-2b89f1f5955a)


This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/48017871-43f9-41f2-8b8c-633cfbbc5415)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/ef197fa7-7bfe-466b-a544-9a116980cbc5)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/e1f2c5b6-14db-4d95-b5aa-492a551acbb5)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

T Flip-Flop
T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/33651e25-4f59-44d4-be66-6be554be8788)


This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State

![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/2bc0748a-60e3-4578-9b88-040540d0969f)


From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

Procedure:
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.

PROGRAM :
SR FLIPFLOP:
PROGRAM 1
```
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: Revathi.D
RegisterNumber: 212221240045

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
RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/7d431d19-2d5c-4fc1-99e0-1825cdf7faf7)
TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/ff66125c-0eac-4b95-885d-bf31b7cc3830)
```
JK FLIPFLOP
PROGRAM 2

Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: Revathi.D
RegisterNumber: 212221240045

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
RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/83b2c677-de23-46ca-b2a7-8a4aa5deab14)
TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/074829c1-d64c-45ac-bf9d-cf4d1983cab2)
JK FLIPFLOP
PROGRAM 2
```
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by:Revathi.D
RegisterNumber: 212221240045 

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
RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/d70f18d1-5627-4091-aa06-d99e098e17d6)
TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/ce57e9d2-a3cc-4d97-a93b-6727297b82fb)
D FLIPFLOP
PROGRAM 3
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by:Revathi.D
RegisterNumber: 212221240045

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
RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/a307fd2a-457e-456c-9147-dad37b86554e)
TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/4268c477-dd96-44e1-96ee-a77c49911596)
T FLIPFLOP
PROGRAM 4
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by:Revathi.D
RegisterNumber: 212221240045
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
RTL LOGIC FOR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/2c50bff4-d883-4f9d-8be3-e84ff466d123)
TIMING DIGRAMS FOR FLIP FLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/dc246cd6-b86a-4ed9-8550-84757dd6f84d)

RESULTS
Thus implementation of SR,JK,D and T flipflops using nand gates are done sucessfully.


