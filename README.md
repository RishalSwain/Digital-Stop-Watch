# Digital-Stop-Watch
Digital stopwatch using 7490 counters and 7447 decoders with 7-segment display output, designed and simulated in Multisim for Digital Electronics learning.
Digital Stopwatch (DEC Project)
About the Project

This project is a simple digital stopwatch that I designed as part of my 2nd year Digital Electronics subject (EEE). The main idea was to build a working stopwatch using basic digital ICs instead of using any microcontroller, so that the core concepts of counters and display logic become clear.

The entire circuit is designed and tested in Multisim.

How it Works

A function generator is used to give clock pulses to the circuit. These pulses act like the ticking of a clock.

The 7490 counter counts these pulses and generates a BCD output
This BCD output is then given to the 7447 decoder
The decoder converts it into signals required for a 7-segment display
One counter handles the units digit and another handles the tens digit

So basically, the display increases step by step like a stopwatch (00 → 01 → 02 ... up to 99).

An AND gate (7408) is used in the circuit to manage the counting sequence properly.

Components Used
7490 Decade Counter
7447 BCD to 7-Segment Decoder
7408 AND Gate
7-Segment Displays (Common Anode)
Function Generator
5V Power Supply
Why This Approach

Even though this could be easily done using Arduino or any microcontroller, the goal here was different.

This project focuses on understanding:

how counters actually work internally
how BCD values are generated and used
how display decoding is done at hardware level

So instead of using programmable devices, everything is built using basic digital ICs.

Limitations
It only counts from 00 to 99
Accuracy depends on the input clock frequency
No start/stop or reset button is added yet
Possible Improvements
Adding start, stop and reset buttons
Extending it to minutes and hours
Using a stable clock source instead of function generator
What I Learned

While working on this project, I got a much better understanding of:

decade counters
BCD representation
7-segment interfacing
how digital circuits behave in real-time
Tools Used
Multisim (for simulation)
