Lab5
====
The purpose of part one of this lab was to simulate in PRISM, adn then connect our ALU to the datapath and have our prism 
simulation run in VHDl adn finally simulate on our FPGA.

The function of program one is that it loads 8 into the computer, adds one to that value, and then outputs 
it to port 3.  Teh program loops back, going from 9 to F, and then ends in an infinite loop.

![alt text](http://i57.tinypic.com/2ztja5c.png)

![alt text](http://i58.tinypic.com/30c9f05.png)

![alt text](http://i61.tinypic.com/zji9uv.png)


GR Questions
====
1.	When the controller’s current state is “FETCH,” what is the status of the following control lines:

a.	PCLd   Answer: high

b.	IRLd   Answer: high

c.	ACCLd  AnswerL low


2.	The current state is Decode LoAddr and the IR contains “OUT.”  What are the control signals are asserted, and what will the next state be?

Answer: Control sigs asserted are MarloLD and PCld and the next stats is Direct Io execute


3.	What are the three status signals sent from the PRISM datapath to the PRISM controller?

Answer: 1, A=0, and A<0



4.	Why is it important that ACCLd signal be active during the execute state for the ADDI instruction?

Answer: To add the value to teh accumualtor, the computer must know what value us already stored in the accumulator,
and thsi is accomplished by Accumulator Load (ACCLd).


5.	What changes are necessary to the PRISM datapath to add another instruction (SUBI, which would subtract an immediate value from the accumulator) to the instruction set?

You must increase the total number of bits in the control signals to be able to add another instruction



