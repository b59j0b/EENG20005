java c
EENG20005 Electrical Energy Conversion and Supply
Coursework Script
Part 2 DC/AC Power Conversion
Summary
Design, build and evaluate an AC/DC/AC power conversion system for variable speed drive applications sourced by the mains.
Learning outcomes
 RMS and average value
 Pulse Width Modulation
o Principles and implementation
o Quantities to vary
 Ideal vs. semiconductor switches
o Gate signals
 Measure FFT harmonics
o Understand fundamental frequency and switching frequency harmonics
o Impact and source of low-order harmonics to the grid
 Rectifier and inverter circuits
o Power electronics vs. ideal AC sources
o Single-phase vs. three-phase versions
 Sizing and impact of filters
 Muti-quadrant operation
Tools
Simulink Simscape Power Systems
 Part1_Part2_library.slx
 Part2_template.slx
 Part2_template_3_ph.slx
FFT analyser
Case 2A Single-phase full-wave diode bridge rectifier
Build a single-phase full-wave passive rectifier in a Simulink model following the system specifications mimicking a DC load drawing power from the mains. Add a resistive load R.
Mains voltage                                Vmains                            380 Vrms, 50 Hz
Load                                                                   R                                                       10 Ω
Task 2.1
Draw a circuit diagram of a single-phase rectifier and describe its mechanism. Calculate the average (mean) value of the rectified voltage waveform. analytically and validate through simulation.
Task 2.2
Add in and design a DC filtering capacitor to suppress the peak-to-peak voltage ripple to 4% of the average through iterations (trial and error) in Simulation startnig from 1 μF. What is the capacitance value C yielded in your design? Show a waveform. comparison of the DC-link voltage waveform. before/after the filtering.
What happens to the average DC-link voltage if the capacitor was bigger/smaller?
Change the load R to 5 Ω, what happens to the voltage ripple and average value? Explain the differences.
Task 2.3
Observe and describe the AC input current. Perform. Fast Fourier Transform. (FFT) analysis on this current and comment on the harmonics.
Case 2B Single-phase half bridge inverter with passive load
Build a single-phase half-bridge inverter with ideal switches and a passive RL load connected back to the dc-link neutral point (ground). This assumes an ideal dc-link with a fixed neutral point voltage (emulating two modular baƩ ery packs in series with a mid-point tab). Follow the below specifications mimicking the powertrain of an Electric Vehicle.

Task 2.4
Draw a circuit diagram of a single-phase two-switch inverter with and RL load and describe its operating mechanism. Build the PWM block using a comparator and sine/triangular wave sources to control the half bridge. Provide proof of a working system (e.g. load voltage and current).
Measure the RMS value the converter output voltage (between the output node of the half-bridge and ground) and the load current. What is the difference between RMS and true RMS in this case?
Task 2.5
Change the value of the filter inductance to achieve a peak-to-peak load current ripple (near the top of the quasi-sinewave) of less than 10A through iterations (trial and error) in simulation. What is the inductance value?


Before and after changing the inductance value, perform. and plot FFT on the load current - observe and explain the difference.
Task 2.6
Reduce the output voltage RMS to 80V (Spec. 1)/160V (Spec. 2) by changing the modulati代 写EENG20005 Electrical Energy Conversion and Supply Part 2 DC/AC Power ConversionMatlab
代做程序编程语言on index. Use the original L value. Work out how much the modulation index should be analytically. Validate the design in Simulation.
Compare the performance against an equivalent AC source.
Task 2.7
Change the fundamental frequency of the converter output voltage to 100 Hz (Spec. 1)/200 Hz (Spec. 2) in simulation. Demonstrate how and show proof. In real applications, when/why should we change the fundamental frequency?
Task 2.8
Show how to change the switching frequency to 5 kHz while keeping fundamental frequency at 50Hz(Spec. 1)/100 Hz (Spec.2) and the modulation index at 0.8. What happens to the converter output voltage and load current?
To achieve the same current ripple level as Task 2.5 (i.e. ∆Ipk-pk   = 10 A), what value should the L be now? How does the FFT on the load current change compared to Task 2.5?
Task 2.9
Replace ideal switches with IGBT + anti-parallel diodes. What happens if the diodes are removed? Explain what you observe. (hint: observe the current in the anti-paralleled diodes). Set the carrier wave frequency to 5 kHz, and use the L value yielded in Task 2.8.
Task 2.10
Observe the load voltage/current and the apparent power. Demonstrate the multi-quadrant operation of the converter-load system. Please do this with the IGBT and anti-parallel diodes. In what scenario would the converter operate beyond the First Quadrant?
Case 2C (advanced task) Single-phase full bridge inverter
Convert the single-phase version Case 2B into a single-phase full bridge (H-bridge) inverter. Use either ideal switches or IGBT+Diode. Design and build the PWM block for the single-phase H-bridge inverter.
Task 2.11
Show a circuit diagram of the whole system. Mark any voltage/current quantities that you may refer to later. Show a ‘truth table’ of the switching states of the full bridge.
Show proof of the working system in simulation – e.g. converter output voltage and load current.
Task 2.12
Compare the H-bridge against the half-bridge in Case 2B – what are the pros and cons of each system? Explain why an H-bridge inverter has a better DC-link utilization or an extended range of output voltage amplitude. Provide waveforms as necessary for comparison.
Task 2.13
Join the diode rectifier in Case 2A and the H-bridge inverter together to mimic a variable frequency drive drawing power from the grid/mains. The ideal DC source is replaced by the diode rectifier and a buffering capacitor in this case. Show a circuit diagram of this case. 9 Show proof of the working system in simulation. Explain and demonstrate the differences between an ideal DC source and a diode rectifier bridge.
Case 2D (advanced task) Three-phase half bridge inverter with passive load
Convert the single-phase version Case 2C into a three-phase version mimicking a drivetrain for electric vehicles with passive RL loads.
Design and build a PWM block for a three-phase inverter with an initial modulation index of 0.8.
Task 2.14
Show a circuit diagram of the whole system and describe its mechanism. Mark any voltage/current quantities that you may refer to later.
Show proof of the working system in simulation – e.g. phase converter output voltage, line converter output voltage, load line current.
Compare the converter output phase voltage and line voltage waveforms and try to explain the difference on the shape difference between them.
Task 2.15
Monitor the three-phase output power – control the converter output real power to be 10 kW per phase through adjusting the modulation block manually. Demonstrate how and show proof.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
