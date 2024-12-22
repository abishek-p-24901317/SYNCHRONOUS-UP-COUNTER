### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram


**TRUTH TABLE**
![397931127-9b984804-3a4d-47ee-a305-ed59b3192154](https://github.com/user-attachments/assets/e973e392-afd3-4313-8576-58383fcedcb2)

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: Abishek P :24901317
*/


![image](https://github.com/user-attachments/assets/ac73b91e-a90a-4fef-a9d4-382ccb65ffd2)


**RTL LOGIC UP COUNTER**
![394725898-8afa3c0a-3495-41a4-b6f7-1e4447466844](https://github.com/user-attachments/assets/e939b08f-921e-4088-a7c2-b1375e972ba1)

**TIMING DIAGRAM FOR IP COUNTER**
![394725924-f594365d-73f6-4b24-9c5a-08ad36de5dc8](https://github.com/user-attachments/assets/9b3ff46c-c081-422e-91b0-ff20d4cebfc8)


**RESULTS**
Thus 4 bit synchronous up counter is implemented and functionality is validated.
