java c
EEET2097 Electronic Circuits
Workshop 2 (Weeks 5-6)
CURRENT SOURCES AND CURRENT MIRRORS
General Information
Special Note: there are two options in this lab manual:
• In the Option 1, measurement video and results are provided.
• In the Option 2, instructions for physical circuit measurement are provided.
Please select one out of the two options. Please note the Option 2 is the recommended option, as you will have the opportunity to gain more hands-on skills.
If you select the Option 1:
• Please complete lab tasks either during the lab session or during your preferred time at home (i.e., attending the lab session is not mandatory). Lab tasks are individual.
• You may also attend any lab session (listed in the Canvas Workshop 2 page) each week for questions and help.
• Please read through the General Information part and then follow the instructions on Page 3 to Page 8 of this lab manual
If you select the Option 2:
• Please complete the lab tasks during your timetabled on-campus lab session. You will conduct physical experiments and measurements in groups (i.e., group tasks)
• Please attend your timetabled session to make sure you have access to the hardware.
• You may also attend other lab sessions (listed in the Canvas Workshop 2 page) for questions and help.
• Please read through the General Information part and then follow the instructions on Page 9 to Page 13 of this lab manual.
Individual lab report is required for both options. Please provide your answers to the questions
(start with “Q”) based on your selection (using provided measurements or your own measurements).
1. AIMS
(i)     Investigate the operation of BJT current sources
(ii)    Understand the output resistance of BJT current sources
(iii)   Investigate the use of BJT current mirrors as the active load
2. INTRODUCTION
Current sources and current mirrors are very important parts of analogue IC designs. The  active current sources and mirrors provide biasing currents for amplifier stages and save valuable real estate on the chip compared with discrete element designs. The current mirror can also be used as the active load in electronic circuits.
A BJT based current mirror circuit is shown in Figure 1.
The output current Io  is related to the reference current IREF  by:
where β is the current amplification factor of the BJT. Assume VA2  is the Early voltage of transistor Q2, the output resistance (taken from Q2) can be described as:Figure 1 BJT current mirror.
3. ASSESSMENT
By lab report (individual report).
Due at 11:59pm, 13 September 2024 (i.e., the Friday of Week 7).
Provide your answers to the questions asked in this lab manual (starting with “Q”).
Include key calculation steps, equivalent circuit schematics, simulation circuit schematics, simulation results, plots, measurement results (if applicable), comparisons and discussions in the report.
•    If you select Option  1:  please include screenshots of your simulation circuit schematics and key simulation results.
•    If you select Option 2:  please  include  photos of the circuit you built and key measurement results.
Please refer to the Marking Rubric for detailed report format and requirements.
4. SESSION TASK ALLOCATION SUGGESTION
If you select Option 1, you may consider allocating the lab tasks to 2 sessions as follows:
•    Watch the general guidance video and complete 5.1 in the first session.
•    Complete 5.2 and 5.3 in the second session.
If you select Option 2, you may consider allocating the lab tasks to 2 sessions as follows:
•    Watch the general guidance video and complete 6.1 in the first session.
•    Complete 6.2 and 6.3 in the second session.
Option 1
Please note this is the first option, where you will be provided with measurement videos and data. All tasks in Option 1 are individual tasks.
5.  WORKSHOP PROCEDURE (OPTION 1)In this workshop, we will use the pre-designed differential amplifier card. Current mirror and current source are part of the card. The circuit schematic is shown in Figure 2. The solid lines in the figure represent existing circuit connections, and the dashed lines represent possible circuit connections that are not connected yet.Figure 2 Laboratory differential amplifier circuit schematic.The  differential  amplifier  card  needs  to  be  installed  in  a  card  frame. to  use  (please  refer  to  the measurement video). The numbers with a circle around them in Figure 2 correspond to the numbered sockets at the base of the card frame. We will refer to these numbers as “socket X” .
5.1 DC Biasing
In this part, we will focus on the DC biasing of the current source. Note the inclusion of:
•    The link A1;
• The 1 MΩ resistor E2.
As shown in the measurement video (video Part 1-1), we connect socket 10 in Fig. 2 to ground (thereby setting VB1 = 0V) and connect a DC current meter between sockets 6 and 7. We also connect DC supply voltages V+ (+10 Volts) and V- (–10 Volts) as marked (i.e., sockets 16 and 1, respectively). Note that we use the dual DC supply on the workbench to generate ±10V supply voltages.
We then adjust the 500 KΩ potentiometer in the circuit to set the emitter current IE of the transistor Q1 to IE = 1 mA.5.1.1 Q: What is the resulting equivalent circuit with the connections mentioned above (please
draw the circuit diagram)? What are the functions of the two BJTs currently utilized (Q1 and Q5)?5.1.2 Q: Theoretically,  how does the 500 KΩ potentiometer in the circuit control the emitter
current of transistor Q1 and why?After adjusting the emitter current IE of Q1, as shown in the measurement video (video Part 1-2) We measure the DC emitter and collector voltages of transistor Q1. The results are shown in Table 1. We also measure the DC voltages of transistor Q5. The results are also shown in Table 1.
Table 1
BJT Transistor
Base Voltage
Collector Voltage
Emitter Voltage
Q1
0 V
5.34 V
-0.747 V
Q5
-9.23 V
-0.747 V
-10 V5.1.3 Q: Is the BJT Q1 in the active operation mode? Also explain why the Q1 emitter voltage is
approximately -0.7V.
5.1.4 Q: Is the BJT Q5 in the active operation mode? Brief explain its working principle. NI Multisim Simulation:Build the equivalent circuit obtained in 5.1.1 in NI Multisim. For the BJTs in the 3086 array (e.g., Q1 and Q5), they are general purpose NPN transistors, and you can use BJT model 2N3904 instead in the simulation (you will notice that there are multiple manufacturers and packages of 2N3904 available, and you can use any of them). Similar with the measurement, adjust the 500 kΩ potentiometer to set the emitter current IE of Q1 to IE = 1 mA in the simulation. If yourIE current is below 1 mA, replace the 1 MΩ resistor (E2 in Figure 2) with any resistor between 560 kΩ and 1.5 MΩ to set it to 1 mA.
5.1.5 Q: What is your simulation circuit schematic? Also show that yourIE current is 1 mA. Simulate the emitter, base and collector voltages of transistors Q1 and Q5.
5.1.6 Q: What are the simulated voltages? Show the screenshots of simulation results.5.1.7 Q: Compare the simulation results with the measurement results shown in Table 1. Are
they similar and why?Note: Since we are analysing the bias of the circuit, the DC Operating Point analysis mode can be used  in this  part  of  circuit  simulation.  For  the  potentiometer,  in  simulation  you  can  use  the component “POTENTIOMETER_RATED”, and for the Zener diode, you can use “ZENER” .
5.2 Current Source Output ResistanceAs shown in the measurement video (video Part 2), we connect a number of 1kΩ resistors between socket 6 and the input to the current meter (the current mirror is connected between sockets 6 and 7, as described in 5.1). We change the resistor connections for 5 different settings (i.e., 5 different resistances), and measure the corresponding collector-emitter voltage of the transistor Q5 (i.e., the voltage difference between socket 7 and socket 1) and the collector current (i.e., output current of Q5). The results are shown in Table 2.
Table 2
Resistance
200 Ω
250 Ω
333 Ω
500 Ω
1 kΩ
VCE
9.118 V
9.064 V
8.968 V
8.791 V
8.352 V
IC
0.996 mA
0.995 mA
0.993 mA
0.990 mA
0.984 mA5.2.1 Q: Theoretically, how does the resistor connected between socket 6 and the input to the
current meter allow us to change the output voltage from the current source transistor Q5?5.2.2 Q: Plot the transistor Q5 output current versus the collector-emitter voltage curve basedon the measurement results shown in Table 2 (you may consider use Excel or Matlab) . Include the plot in your lab report. What is the output resistance of the current source transistor?
Hint: The slope of the I-V curve is the output conductance of the current source.5.2.3 Q: If we analyse the circuit theoretically, what is the value of the output resistance of the
current source? (the Early Voltage of transistor Q5 according to the datasheet is 60 V).5.2.4 Q: Compare and discuss your calculation result with your measurement result: are they
similar and why?
NI Multisim Simulation:Similar with the measurement above, adjust the simulation circuit used in 5.1 by connecting a resistor R between the emitter of Q1 and the collector of Q5. Change the Early voltage of the transistor 2N3904 used  in the simulation to 60 V.  Keep other  parts of the simulation  circuit  unchanged. Adjust the resistance of R to the values shown in Tab代 写EEET2097 Electronic CircuitsMatlab
代做程序编程语言le 2.5.2.5 Q: Under  different  settings  of R, what  are  the  simulated  collector-emitter  voltage  of
transistor Q5 (VCE) and and the collector current (i.e., output current IC of Q5)?5.2.6 Q: Plot the transistor Q5 output current versus the collector-emitter voltage curve based
on the simulation results. Include the plot in your lab report. What is the simulated output resistance of the current source transistor?5.2.7 Q: Compare   and  discuss  your  simulation   result  with  your  calculation  (5.2.3)  and
measurement (5.2.2) results.
Note: Since we are still dealing with DC analysis, the DC Operating Point analysis mode can be used in this part of circuit simulation.
5.3 Current Mirror OperationThe differential amplifier card contains a current mirror comprising two PNP transistors (type 2N3638) that can be connected as a load to replace the 4.7kΩ collector resistors. In this part, we will connect two common-emitter amplifiers in parallel as a differential pair (Q1 and Q2 in Figure 3) and use the current mirror as the collector load for each amplifier.To configure the circuit, we remove link A1, and insert link F and link G, as highlighted in Figure 3. E2 remains the same with 1 MΩ resistor connected. These links connect the PNP current mirror (i.e., Q3 and Q4) to the collectors of the two NPN transistors Q1 and Q2 which form. the differential pair. We then connect socket 10 and socket 13 to ground to set the two base voltages to 0, and connect the DC current  meter  between sockets 6 and 7. Afterwards, we adjust the 500  kΩ  potentiometer  in the current source transistor Q5 to get a current flow of 1 mA.If we now use the current meter to measure the collector currents of the current mirror, as shown in the measurement results (Fig. 4), we can obtain about 0.5 mA current for each of the transistors (i.e., Q3 and Q4) in the current mirror.Figure 3 Current mirror configuration.5.3.1 Q: What   is  the   resulting  equivalent  circuit?  Why  the  current  through  each  of  the
transistors in the current mirror is about 0.5 mA?

Figure 4 (a) collector current of transistor Q3; and (b) collector current of transistor Q4.Now we connect an AC small signal to the input of transistor Q1 of the differential pair (i.e., socket 10). We set the signal frequency to 1 kHz, the amplitude (peak-to-peak) to 10 mV, and the signal waveform. to sinusoidal, as shown in Fig. 5(a). The measured signal waveform. at socket 4 (i.e., the output port of the circuit even when the input signal is connected to the left half circuit, which will be discussed in detail in Topic 5) is shown in Figure 5(b). The measured AC current through the link F is 0.0933 mA (AC peak current).Figure 5 (a) input signal to the differential amplifier (socket 10); and (b) output signal of the differential amplifier (socket 4).5.3.2 Q: The measured voltage at socket 4 is equal to the AC collector-emitter in the current
mirror. Explain why this is so.5.3.3 Q: Based on the results, calculate the small signal output resistance of the left half circuit
(including the current mirror transistor Q3 and the amplifier transistor Q1).
Hint: The small signal output resistance can be calculated as Rout   = vac,4 /iac.    5.3.4 Q: Calculate the expected output resistance of the left half circuit theoretically.For the transistor Q1 (or Q2) in the amplifier part, the Early Voltage, which is typically referred as the “Collector-Emitter Breakdown Voltage” in a datasheet, is 60 V. For the transistor Q3 (or Q4) in the current mirror, the Early Voltage is 25 V.
Hint: The output resistance of the left half circuit here includes two parts connected in parallel: the ro  of Q1 and the ro  of Q3.
5.3.5 Q: Compare  and  discuss  your calculation  result  (5.3.3) with the  measurement  result
(5.3.4).We now connect the AC small signal to the input of transistor Q2 in the differential pair (i.e., socket 13). The measured signal waveform. at socket 4 is shown in Figure 6. The measured AC current (rms current) through the link G is 0.0938 mA (AC peak current).Figure 6 Output signal of the differential amplifier (socket 4).5.3.6 Q: Based on the results, calculate the small signal output resistance of the right half circuit
(including the current mirror transistor Q4 and the amplifier transistor Q2).
5.3.7 Q: Calculate the expected output resistance of the right half circuit theoretically.
Hint: Transistor Q2 is identical to Q1, and transistor Q4 is identical to Q3.5.3.8 Q: Compare  and  discuss  your  calculation  result  (5.3.6)  with  the  measurement  result
(5.3.7).5.3.9 Q: Compare the output resistances of the right circuit (i.e., Q2 + Q4) and the left circuit
(i.e., Q1 + Q3). Explain the difference on the output resistance.
Option 2Please note this is the second option (no simulation required), you will be provided with measurement guides. The measurement tasks in Option 2 can be completed in groups (however, individual  lab reports are still required). Option 2 is the recommended option to gain more hands-on skills.
6.  WORKSHOP PROCEDURE (OPTION 2)Obtain a differential amplifier card from the cupboard and install it in a card frame. Current mirror and current source are part of the card. Connect the circuit as shown in Figure 7. Note the inclusion of:
• The link A1.
• The 1 MΩ resistor E2.The differential amplifier needs to be installed to a card frame. to use. The  numbers with a circle around them in Figure 7 correspond to the numbered sockets at the base of the card frame. We will refer to these numbers as “socket X” . Please note that Figure 7 is identical to Figure 2 in Option 1.Figure 7 Laboratory differential amplifier circuit schematic.
6.1 DC Biasing
Step 1: Connect socket 10 in Fig. 7 to ground (thereby setting VB1 = 0V) and connect a DC current meter between sockets 6 and 7 (make sure the multimeter is set to current mode and that socket 6   is connected to the current input terminal on the meter). Connect DC supply voltages V+ (+10 Volts)  and V- (–10 Volts) as marked (i.e., sockets 16 and 1, respectively). You can use the dual DC supply on your workbench in tracking mode to generate ±10V supply voltages (please refer to Appendix I).
NOTE: If you are not sure if the circuit connection or the dual power supply connection is correct, please ask your lab tutor to have a quick check before powering the circuit.6.1.1 Q: What is the resulting equivalent circuit (please draw the circuit diagram)? What are the
functions of the two BJTs currently utilized (Q1 and Q5)? Step 2: Measure the emitter current IE of the CE amplifier (i.e., Q1).
Step 3: Adjust the 500 kΩ potentiometer on the card to set IE = 1 mA. If your maximum current is below 1 mA, replace the 1MΩ resistor with any resistor between 560kΩ to 1.5MΩ .6.1.2 Q: Theoretically,  how does the 500  kΩ potentiometer in the circuit control the emitter
current of transistor Q1 and why?
Step 4: Measure the base, emitter and collector voltages of the transistor in the CE amplifier. Step 5: Measure the terminal voltages of the current source transistor (i.e., Q5).6.1.3 Q: What are the base, emitter and collector voltages and currents of the transistor in the
CE amplifier?6.1.4 Q: What are the base, emitter and collector voltages and currents of the current source
transistor?6.1.5 Q: Is the BJT Q1 in the active operation mode? Also explain why the Q1 emitter voltage is
approximately -0.7V.
6.1.6 Q: Is the BJT Q5 in the active operation mode? Brief explain its working principle.
6.2 Current Source Output Resistance
Step 1: Let’s continue with the circuit that you build in 6.1. Add a 1 kΩ resistor between socket 6 and the input to the current meter (i.e., the connection is: socket 6 to the input of the current meter, to   the output of the current meter, and further to socket 7).
Step 2: Measure the collector-emitter voltage of the current source transistor (i.e., the voltage difference between socket 7 and socket 1) and the current delivered by the current source.
Hint: You can use the digital multimeter (DMM) block of the ELVIS II board to measure the collector-emitter voltage (please refer to Appendix II).
Step 3: Change the resistance of the resistor added inStep 1 above to another four different values
(between 0.1 kΩ to 1 kΩ), and repeat Step 2 above (i.e., measure the corresponding collector-
emitter voltage of the current source transistor and the current delivered by the current source).6.2.1 Q: Theoretically, how does the resistor connected between socket 6 and the input to the
current meter allow us to change the output voltage from the current source transistor Q5?6.2.2 Q: Use a table to show the measurement results (you may use a table similar to the Table
2 in Option 1).6.2.3 Q: Based  on  your  measurement  results,  plot  the  output  current versus the collector-emitter voltage curve (you may use Excel or Matlab) and find the output resistance of the current source. Include the plot in your lab report. What is the output resistance of the current source transistor?
Hint: The slope of the I-V curve is the output conductance of the current source.6.2.4 Q: If we analyse the circuit theoretically, what is the value of the output resistance of the
current source? (the Early Voltage of transistor Q5 according to the datasheet is 60 V) .6.2.5 Q: Compare and discuss your calculation result with your measurement result: are they
similar and why?



         
加QQ：99515681  WX：codinghelp
