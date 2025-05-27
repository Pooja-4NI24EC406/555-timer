# 555-timer
<h2>INTRODUCTION TO 555</h2>
#The 555 timer IC is an integral part of electronics projects. Be it a simple project involving a single 8-bit microcontroller and some peripherals or a complex one involving system on chips (SoCs), a 555 timer is involved. These provide time delays, as an oscillator and as a flip-flop element among other applications.<br>

Introduced in 1971 by the American company Signetics, the 555 is still in widespread use due to its low price, ease of use, and stability. It is made by many companies in the original bipolar and low-power CMOS types. According to an estimate, a billion units were manufactured back in the year 2003 alone. <br>


<h2>555 Timer IC Internal Circuit</h2>

![image](https://github.com/user-attachments/assets/9912bdfd-1c38-421f-a8d3-82d9152837e2)


Depending on the manufacturer, the standard 555 timer package includes 25 transistors, 2 diodes, and 15 resistors on a silicon chip installed in an 8-pin mini dual-in-line package (DIP-8). Variants consist of combining multiple chips on one board. However, 555 is still the most popular.

<h2>555 Timer IC Pin Diagram</h2>

![image](https://github.com/user-attachments/assets/9221e491-6394-42fb-81c2-90d821a21383)

![image](https://github.com/user-attachments/assets/cd5a3eb0-129b-4812-a250-bf6429958e45)

<h2> 555 Timer Specification</h2>
555 timer is used in almost every electronic circuit today. A 555 timer works as a flip-flop or as a multi-vibrator, it has a particular set of configurations. Some of the major features of the 555 timers would be,<br>

It operates from a wide range of power ranging from +5 Volts to +18 Volts supply voltage.<br>
Sinking or sourcing 200 mA of load current.<br>
The external components should be selected properly so that the timing intervals can be made into several minutes along with the frequencies exceeding several hundred kilohertz.<br>
The output pin of a 555 timer can drive a transistor-transistor logic (TTL) due to its high current output.<br>
It has a temperature stability of 50 parts per million (ppm) per degree Celsius change in temperature which is equivalent to 0.005 %/ °C.<br>
The duty cycle of the timer is adjustable.<br>
Also, the maximum power dissipation per package is 600 mW, and its trigger pulse and reset inputs have logic compatibility.<br>

<h2>555 Timer Working</h2>
The Multivibrator 555 timer IC generally operates in 3 modes:<br>

1.Astable Multivibrator.<br>
2.Monostable Multivibrator.<br>
3.Bistable Multivibrator.<br>

<h2>Astable Mode</h2>
This means there will be no stable level of output. So the output will be swinging between high and low. This character of unstable output is used as a clock or square wave output for many applications.<br>
It produces a continuous series of pulses with a predetermined frequency and duty cycle.<br>
It has no stable state, hence the name astable.<br>

![image](https://github.com/user-attachments/assets/6f6d9b75-65d0-463f-9246-9c4a7bd2b0ff)

![image](https://github.com/user-attachments/assets/52fc1757-64aa-426c-a41a-d941a93f476e)

![image](https://github.com/user-attachments/assets/a329fd5c-a828-46db-a3c6-d7ee9a9cce70)

50% duty cycle<br>
Duty cycle=R1/R1+R2



<h2> Monostable Mode</h2>
This configuration consists of one stable and one unstable state. The stable state can be chosen as either high or low by the user. If the stable output is set at high (1), the output of the timer is high (1).<br>

At the application of an interrupt, the timer output turns low (0). Since the low state is unstable it goes to high (1) automatically after the interrupt passes. Similar is the case for a low stable monostable mode.<br>

![image](https://github.com/user-attachments/assets/fa1d7ad4-ada3-427b-acc2-35ac58e6fbbe)

<h2> Bistable Mode</h2>

![Image](https://github.com/user-attachments/assets/2b76c0fe-aea8-4602-a517-bfecab0075dd) <br><br>

In bistable mode, both the output states are stable. At each interrupt, the output changes from low (0) to high (1) and vice versa, and stays there. For example, if we have a high (1) output, it will go low(0) once it receives an interrupt and stays low (0) till the next interrupt changes the status.
It requires two transistors, two capacitors, and a few resistors.
It is commonly used in digital circuits as a memory element, latch, or flip-flop.

<h2>Monostable multivibrator working:</h2>

A monostable multivibrator produces a single pulse of fixed duration in response to a trigger signal. 

- *Triggering*: The circuit is triggered by a short pulse or edge, causing it to switch from its stable state.
- *Quasi-stable state*: The output goes high (or low) and remains in this state for a predetermined time period determined by the RC timing circuit.
- *Timing*: The capacitor in the RC circuit charges or discharges, controlling the duration of the quasi-stable state.
- *Return to stable state*: Once the timing period ends, the circuit returns to its stable state, and the output goes back to its original state.
- *Fixed pulse width*: The duration of the output pulse is fixed and independent of the trigger signal duration.

<h2>Astable multivibrator working:</h2>

An astable multivibrator is a type of electronic circuit that produces a continuous square wave output without any external trigger. Its working can be summarized as follows:

- *Oscillations*: The circuit continuously switches between two quasi-stable states, producing a square wave output.
- *Charging and discharging*: The capacitor in the RC circuit charges and discharges, controlling the frequency of the oscillations.
- *Feedback loop*: The feedback loop in the circuit causes the output to switch between high and low states.
- *No stable state*: Unlike monostable or bistable multivibrators, an astable multivibrator has no stable state and continuously oscillates.
- *Frequency determination*: The frequency of the output square wave is determined by the values of the resistors and capacitors in the circuit.

<h2>DESIGN QUESTION:</h2>
1. GENERATE THE WAVEFORM WITH PULSE WIDTH OF 0.5ms USING 555 IC<br>
2. DESIGN ASTABLE MULTIVIBRATOR IN WHICH TIME PERIOD CAN VARIED EXTERNALLY<br>

<h3>Monostable multivibrator: CASE01</h3>
## Calculation:
Given that T=0.5ms and assume c=.1uF.

T=1.1RC









<h3>CASE 02</h3>








<h3>CASE 03</h3>




<h3>Astable multivibrator: CASE01</h3>






<h3>CASE 02</h3>







<h3>CASE 03</h3>









<h2> Result</h2>

- A monostable multivibrator circuit using 555 IC was designed and simulated to generate a pulse width of 0.5ms.
- An astable multivibrator circuit using 555 IC was designed and simulated to generate a continuous square wave output with variable frequency.
1. Monostable Multivibrator:
    - A pulse width of 0.5ms was successfully generated using the 555 IC in monostable mode.
    - The output waveform was a single pulse with a precise duration, demonstrating the IC's ability to generate accurate timing signals.
2. Astable Multivibrator:
    - A continuous square wave output was generated using the 555 IC in astable mode.
    - The frequency of the output waveform was varied externally, demonstrating the IC's ability to produce variable frequency signals.



<h2> Inference</h2>

- The 555 IC can be used to generate a single pulse of fixed duration in monostable mode.<br>
- The pulse width can be precisely controlled using external components.<br>
- In astable mode, the 555 IC can generate a continuous square wave output with variable frequency.<br>
- The frequency of the output waveform can be varied externally using potentiometers or variable resistors.<br>
- The experiment demonstrates the versatility and functionality of the 555 IC in different modes.<br>


<h2> Conclusion</h2>
The experiment successfully demonstrated the functionality of the 555 IC in monostable and astable modes, highlighting its versatility and applications in pulse generation, timing circuits, and oscillators. The results show that the 555 IC can be used to generate precise pulses and variable frequency waveforms, making it a valuable component in various electronic circuits.
