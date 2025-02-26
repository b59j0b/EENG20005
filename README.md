java c
EENG20005 Coursework Script
Overview
Submission
 Summative submission: A technical report in Week 23 accompanied by a package of all simulation models and codes.
 Mid-term formative submission: A technical report for Part 1 and 2 in Week 12.
Laboratory sessions
 3 × 3-hour live sessions in Week 7, 8, 9
 2 × 2-hour drop-in sessions in Week 10, 11
Report elements
A. Description of approach/methodology
B. Mathematical working
C. Simulation waveform.
D. Diagrams - phasor diagram, circuit diagram
E. Results in data points presented in a table or a visualised graph (e.g. curve)
F. Analysis and discussion of results
Part 1. AC power system
Summary
Design and analysis of an AC power system covering power generation, transmission, distribution and load.
Learning outcomes
 Design of ideal transformers
 Electric power systems
 Constant-power load vs. passive load
 Phasor diagrams for analysing phase/amplitude relationships of sinusoidal signals
 Power and impedance triangles
o Power factor and impedance angles
 Measurement and calculation of voltage, current and power quantities
o Real (active), reactive and apparent power
 Power factor correction
 Single-phase vs. three phase system
 Composite and unbalanced load
Tools
Simulink Simscape Power Systems (components in black)
 Part1_Part2_library.slx
 Part1_template.slx
How to use: copy components from Part1_Part2_library.slx into templates.
It is advised to save separate simulation files for each case study.

Case 1A Single-phase AC system
Build a Simulink simulation model of a single-phase AC power system consisting of the power generation, transmission, distribution and a load. The specifications are as below divided into Groups 1~5 determined by the last digit of the student number. Assuming ideal AC sources, transformers and transmission lines.

* Last digit of student number
Task 1.1
Show a circuit diagram of the whole system and describe it. Mark any voltage/current quantities or measurement points that you may refer to later.
Design the ideal transformers as needed in the system analytically. How many transformers are required and what are their turn ratios? Implement these transformers in the simulation model.
Task 1.2
Back to the provided specifications, work out the following currents analytically, assuming ideal conditions.
- Generator current IG
- Transmission line current Iline
- Consumer load current Iload
Provide validation of the results by measuring out the waveforms in simulation.
Task 1.3
What if the generator and transmission voltages are both aligned to the consumer voltage (no step-up or step-down). Observe the currents and compare it against values in Task 1.2. What are the benefits of transmiƫ ng power at a higher voltage?
Case 1B Complex load
While the Consumer 1 continues to draw the active power in Case 1A, it now runs under a 0.75 power factor due to the load being an inductive electric machine. Revise the simulation model starting with an active load block in Simulink which draws a defined active/reactive power..
Task 1.4
Work out the below quantities on paper through analytical formulas. Measure out these quantities in simulation – do the simulation results agree with the analytical results?
- Generator real power PG
-代 写EENG20005 Coursework Script Part 1. AC power systemR
代做程序编程语言 Generator reactive power QG
- Generator current IG
- Transmission line current Iline
- Consumer load current Iload
Compare the currents in Case 1.1 and Case 1.2 - what is the consequence of a load with significant reactive power?
Task 1.5
Can you measure the real, reactive and apparent power only using voltage and current probes? Demonstrate this in the simulation, and compare the result with a power meter. Explain the difference between the two results.
Task 1.6
Replace the constant load block with a passive load formed by R and L components in series, which still satisfies the same power and voltage specifications in this case. Work out the values analytically and validate the design in simulation. Use the power triangle to help your design.
Case 1C Power factor correction (PFC)
For the industrial customer, the national grid imposes a financial penalty unless their power factor can be improved to >0.95 lagging. A passive capacitor bank is used for correcting the power factor from Case 1B to 0.95.
Task 1.7
Show a circuit diagram of just the load with the added capacitor. Mark any voltage/current quantities that you may refer to later.
Calculate the required capacitance value. Draw a power triangle for the power factor correction case. Validate the design in simulation.
Task 1.8
Draw a phasor diagram for the load voltage and current quantities including the PFC capacitor banks on each of the R, L, C components. Use the generator voltage as the reference.
Task 1.9
Observe the grid-side power and currents. What are the benefits of PFC for the grid?
Case 1D (advanced task) Three-phase AC system
Convert the single-phase system in Case 1B to an equivalent three-phase system while satisfying the load specifications with a power factor of 0.75. For simplification, assume the three-phase system is fully balanced without a neutral line. Both the three-phase generator and the load are star-connected. The neutral point of the generator is grounded.
Task 1.10
Draw a circuit diagram of the whole system and describe it. Mark any voltage/current quanties or measurement points that you may refer to later.
Measure the total instantaneous power transmiƩ ed by the three-phase system and compare it against the single-phase case in Case 1B - show waveforms and comment on the difference.
Task 1.11
Measure the phase and line voltages on the load side. Comment on the waveforms and quantities comparing the phase and line voltages. Express the voltages and currents mathematically.
Task 1.12
If the grid frequency is set to 60 Hz, instead of 50 Hz, how would the passive RL load need to be changed to satisfy the same power specifications?
Case 1E (advanced task) Composite load and unbalanced load
Task 1.13
Based on the model in Case 1B, assume there is a second consumer drawing an S of 100 kVA and a power factor of 0.9. Work out the composite power factor of the loads and validate it in simulation.
Task 1.14
Based on the model in Case 1D, add a neutral line into the three-phase system and distribute the load power between Phase A, B, C unequally as 3:2:1 (instead of 1:1:1) representing an unbalanced load. Assume star connections on both ends, work out the neutral line current analytically caused by the unbalanced load and validate it in simulation.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
