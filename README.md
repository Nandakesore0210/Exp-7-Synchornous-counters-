# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### Developed by:
J.Nandakesore
###Register Number:
23009689
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
1.Create a new project in Quartus2 software .
2.Name the project as uc for upcounter and dc for down counter.
3.Create a new verilog hdl file in the project file.
4.Name the module declare as dc and uc for down counter and upcounter.
5.Within the module declare input and output variables.
6.Create a loop using if-else with condition parameter as reset.
7.End the loop.
8.End the module


### PROGRAM 

Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: J.Nandakesore
RegisterNumber: 23009689 
 ## Upcounter:

 ![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/a4cd694e-a1da-423a-8390-9502aaef5f24)

## Downcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/e03351ea-b3a2-4617-98ee-38ffc5f28c1b)

### RTL LOGIC UP COUNTER AND DOWN COUNTER  

## Upcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/68e39fd6-335a-430b-a814-f74172ab10cb)

## Downcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/55e1c5d0-4312-404d-a601-76e07e0f1c44)

### TIMING DIGRAMS FOR COUNTER  

## Upcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/1c5f5a9c-9729-473e-bf10-4a76f60075e0)

## Downcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/cad43aa5-0d84-4d8f-a255-30951571dbc1)

### TRUTH TABLE

## Upcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/7131031f-c9d8-40ac-a2e6-e1bd0941031c)

## Downcounter:

![image](https://github.com/Nandakesore0210/Exp-7-Synchornous-counters-/assets/149365088/c97ec5c6-59fe-44e8-b723-575db54947ac)

### RESULTS:

Thus Synchornous counters up counter and down counter circuit are studied and the truth table for different logic gates are verified.
