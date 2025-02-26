java c
EENG20005 Coursework Script
Overview 
Submission 
•         Summative submission: A technical   report   in Week   23 accompanied   by   a   package   of   all simulation   models and   codes.
Laboratory sessions 
Report elements 
A.       Description of   approach/methodology
B.         Mathematical working
C.       Simulation   waveform.
D.       Diagrams -   phasor diagram,   circuit   diagram
E.         Results   in data   points   presented   in   a table or   a visualised graph   (e.g.   curve)
F.         Analysis and   discussion of   results
Part 3.   Ferromagnetic Actuator 
Summary 
Numerical and   analytical   modelling and simulation of   a   linear ferromagnetic   actuator.
Learning outcomes 
1.       Learning   how to   use   FEA techniques   (such   as   FEMM) to   model   a   linear   ferromagnetic   actuator and   simulate   its electromagnetic characteristics.
2.       Learning   how to   build   analytical   models for   the   linear   ferromagnetic   actuator.
3.       Learning   how to   calculate the   inductance   of   the   actuator   by   using   both   the   FEA   technique   and the   analytical   method.
4.       Learning   how to   calculate the   electromagnetic   force   by   using   the   energy   method.
Tools 
FEMM and   MATLAB   2024a.
Learning   materials 
1.       An   incomplete   FEA   model   draft   in the   EMLab file   named “   Draft_construct_actuator   ”.   (students   need to   build   a   FEA   model   based on   it.)
2.       FEMM   Programming   Manual – a guide to   MATLAB   Codes   for   FEMM.
3.       A guidebook for   MATLAB   - “   Matlab_primer   ”.
4.       Lab Scripts   (Part   A   and   Part   B)   as   asupplementary   guidebook.
Case   3A   FEA   modelling   of   the   ferromagnetic   actuator. 
Build   a   Finite   Element Analysis   (FEA)   model of a   linear ferromagnetic actuator. The   schematic   view   is shown   as   below. The   specifications can   be found   in the   EMLab file:   named “coil1p”, “coil2p”, “coil3p”, “coil4p”, “corep”,   and “   moverp”.   Lab Script. “   Part A”   can   be   used   as a detailed guidebook to assist your   FEA   modelling   based   on   FEMM software.   In order   to support your   learning of the   FEA   modelling technique, two tutorial sessions will   be   provided:
(1) Tutorial   1 –   Introduction   of   FEA   modelling technique   based on   FEMM software.
(2) Tutorial   2 –   How to   use   MATLAB code to assist   FEMM   modelling   (including   how to   use   the   Programming   Manual to search for suitable   MATLAB codes   for   FEMM   modelling).

Fig.   1: Schematic of concentrated   and distributed   e-machine   windings   with   round   and rectangular conductors.

Fig.2: A draft   FEMM   model - “   Draft_construct_actuator   ” will   be   provided   as shown   above.
Task 3.1
Open the   incomplete   FEA   model   (FEMM   model) “   Draft_construct_actuator   ”, go through the   MATLAB codes for the   FEMM draft   model which   is   currently   incomplete.   You   will   need   to build the   rest of the   FEA   model   (FEMM   model)   and   complete the   model   before   proceeding   with the   rest of   the   tasks. 
The   learning   materials and   resources   provided,   including “   Programming   Manual   Book”   and         “   Lab Scripts -   Part A and   Part   B”, will   assist   you   in   completing   the   build   of the   model.   The   lab   scripts   provided   also give   instruction on   building the sections   of   model that   have   already been   provided.   It   is   recommended that you   read the   lab script. to   understand   how   FEMM   modelling works.
Task 3.2 
In your technical   report, show the completed   FEMM   model,   its   mesh   result   plot,   number of   elements after the   mesh, and describe    discuss these   results   briefly.
Case   3B   Analytical   modelling   of   the   ferromagnetic   actuator. 
Build 代 写EENG20005 Coursework Script Part 3. Ferromagnetic ActuatorMatlab
代做程序编程语言  an   analytical   model   of the same ferromagnetic actuator   based   on   its   Magnetic   Equivalent circuit.   Below   are some suggested tasks to   help   complete   the   task   3.2.
Task 3.3 
Draw the circuit diagram of the magnetic equivalent circuit of the ferromagnetic actuator. Calculate the magnetic reluctance (R) of each component and the total magnetic reluctance of the actuator (∑R).
Task 3.4 
Work out the analytical equation of the inductance of the ferromagnetic actuator. Note: The airgap will change when the “mover” iron core moves linearly (forwards or backwards). Discuss how the inductance changes when the airgap changes. If there is any assumption in your analytical equation of inductance, please describe and justify it or explain how the assumption(s) impact the accuracy of the inductance equation.
Task 3.5 
Write a MATLAB code to present the analytical equation of the inductance of the ferromagnetic actuator in Task 3.4. These codes can be used to calculate the inductance quickly through code rather than hand-written calculation, especially when the airgap changes (i.e.,the airgap has a set of different values when the “mover” iron core moves).
Case   3C   Calculating   the   inductance   of   the   ferromagnetic   actuator. 
Calculate the   inductance of the ferromagnetic actuator   by   using   both FEA technique (Case 3A) and analytical methods (Case   3B).
Task 3.6 
Calculate the inductance values of the ferromagnetic actuator when the airgap increases from 0.1mm to 5.0 mm with a step of 0.1mm, using the analytical modelling method in Case 3B.
In your technical report, show the plot of inductance with the airgap on the x-axis and the inductance on the y-axis. Discuss the inductance results and the plot.
Task 3.7 
FEA techniques (FEMM model) can help simulate and calculate many useful results. Among these results, flux linkage (Ψ) and winding current (I) are useful for calculating the inductance of the actuator.
In your technical report, please write down the equation showing the relation of the inductance of the actuator with the flux linkage (Ψ) and winding current (I).
Task 3.8 
Calculate the inductance values of the ferromagnetic actuator when the airgap increases from 0.1mm to 5.0 mm with a step of 0.1mm, using the FEA (FEMM) modelling method in Case 3A. Show a plot of the same (airgap on the x-axis, inductance on the y-axis). To make a good comparison with analytical calculation results, it is recommended that the inductance values of the ferromagnetic actuator are calculated when the airgap increases from 0.1mm to 5.0 mm with the same step of 0.1mm.
Task 3.9 
Are there are any assumptions or limitations in your analytical method and FEA numerical method? Explain how the assumption(s) impact the accuracy of the inductance results.
Case 3D Calculate the electromagnetic force of the ferromagnetic actuator. 
Calculate the electromagnetic force based on energy methods. Use both methods: FEA technique based on FEMM and Analytical Methods based on MATLAB codes.
Task 3.10 
Explain the energy balance law and how the energy methods are used to calculate the electromagnetic force of the linear ferromagnetic actuator. Show the equations to aid your explanations.
Task 3.11 
Plot the Ψ − I curves of the ferromagnetic actuator. By using the Ψ − I curves, calculate the energy, such as electrical energy and magnetic energy. Both FEA methods and analytical methods should be used in this task. You can provide a comparison of the results obtained through both methods.
Task 3.12 (Advanced Task) 
Calculate the electromagnetic force   based on   energy   methods as   descripted   in   task   3.10   and   the   Ψ − I curve   in task 3.11.   Plot   the   force-airgap   curve   to   show   how   the   force   changes   with      the   airgap.   Discuss the   results.   Note that   both   FEA   methods and analytical   methods should be   used   in this task. 



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
