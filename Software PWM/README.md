# README for Software PWM

Ryan E. Drexel
	
	Created 11 October 2017
	Updated 11 October 2017

Embedded Systems- Dr. Tang and Mr. T.

Software PWM is a C language program designed to run on five MSP430 microprocessors (listed below)
	MSP430G2553
	MSP430FR6989
	MSP430F5529
	MSP430FR2311
	MSP430FR5994
Software PWM uses timer interrupts to modulate the timer pulse. The duty cycle is the amount of time,
relative to the timer period, that the signal is high. If the duty cycle capture compare register is equal to 
CCR0 (or 0), then the duty cycle is full, or on 100% of the time. As duty cycle CCR decreases, so does the "on"
time of the output pin, and the perceived brightness of the LED decreases.