# README for Debouncing

Ryan E. Drexel
	
	Created 11 October 2017
	Updated 11 October 2017

Embedded Systems- Dr. Tang and Mr. T.

Debouncing is a C language program designed to run on five MSP430 microprocessors (listed below)
	MSP430G2553
	MSP430FR6989
	MSP430F5529
	MSP430FR2311
	MSP430FR5994
Debouncing is a simple code that solves the problem of bouncing on a button. Bouncing is when a hardware
button is depressed and released, it bounces up and down a few times for a few miliseconds.

A hardware method to debouncing is a simple low pass filter. The high frequencies will be filtered out so
only the initial press will go through. A cutoff frequency under 1000 Hz should work.

This code is a software debounce. When the initial button press occurs, an interrupt is triggered. The
ISR in this case uses a timer based delay. During this delay, inputs will be ignored.