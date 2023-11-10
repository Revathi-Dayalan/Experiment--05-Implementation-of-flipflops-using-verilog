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
Program for flipflops and verify its truth table in quartus using Verilog programming.

Developed by: Sabari Akash A

RegisterNumber: 212222230124

SR Flipflop
module flipflop(s,r,Q,Qbar,clk);
input s,r,clk;
output reg Q,Qbar;
initial Q=0;
initial Qbar=1;
always @(posedge clk)
begin
Q=s|(Q&(~r));
Qbar=r|(Qbar&(~s));
end
endmodule
JK Flipflop
module jkflipflop(k,clk,j,Q,Qbar);
input k,clk,j;
output reg Q;
output reg Qbar;
initial Q=0;
initial Qbar=1;
always @(posedge clk)
begin
Q=((~Q)&j)|(Q&~k);
Qbar=(~Qbar&k)|(Qbar&~j);
end
endmodule
D Flipflop
module dflipflop(d,clk,q,qbar);
input d,clk;
output q,qbar;
reg q,qbar;
initial q=0;
initial qbar=1;
always @(posedge clk)
begin 
q<=d;
qbar<=~d;
end
endmodule
T Flipflop
module tflipflop(t,clk,q,qbar);
input t,clk;
output q,qbar;
reg q,qbar;
initial q=0;
initial qbar=0;
always @(posedge clk)
begin 
q<=(t&~q)|(~t&q);
qbar<=~q;
end
endmodule
RTL LOGIC FOR SR FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/93ee2a90-fcfd-4583-a612-ce679561bbe3)


RTL LOGIC FOR JK FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/5a566c52-4003-4b5e-846b-e6d95847c261)


RTL LOGIC FOR D FLIPFLOPS
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/6d600d07-cb6a-44dd-bea7-c46e31f2fb73)


RTL LOGIC FOR T FLIPFLOPS:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/0a082ce5-7c16-496a-9eef-ed70a83b3930)


Waveform Output For SR:
Screenshot 2023-09-15 093155

Waveform Output For JK:
image

Waveform Output For D:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/243740ba-da35-4866-a8c8-584869d3a6d5)


Waveform Output For T:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/9905ca30-000a-4518-b5c6-bae3c662aa54)


Truth table For SR:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/9aeeb60a-efbb-42d8-ad28-d3a8088ca12a)


Truth table For JK:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/a4a4a815-62d9-470f-b59c-44b0c6bfdbf4)


Truth table for D:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/ba95da91-fbd9-4050-805b-cfc1a63b1bf2)


Truth table for T:
![image](https://github.com/Revathi-Dayalan/Experiment--05-Implementation-of-flipflops-using-verilog/assets/96000574/738cba17-7c8e-4312-a479-0cc22c9a38d5)


RESULTS
Thus the flipflops circuits are designed and the truth tables is verified using quartus software.

