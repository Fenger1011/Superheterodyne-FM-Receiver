# Superheterodyne FM Receiver

## Block Diagram of superheterodyne receiver
![Superheterodyne receiver block diagram](data/images/superhet_blockdiagram.png)

## System Level Design and Calculations
- The FM broadcast frequency band is $f_{FM} \in \left[88-108\right]~\text{MHz}$.
- FM stations have bandwidth of $B = 200 \text{kHz}$.

## Antenna
The antenna is assumed to be broadband 50 ohms.

## Preselector Band Pass Filter
The BPF was designed with 50 ohm source and load terminations in mind. <br>
It was a 3rd order Butterworth BPF since this ...

## Low Noise Amplifier
The low noise amplifier (LNA) was made from a BFP420 in class A operation. <br>

## Mixer
The mixer was chosen to be a double balanced diode ring mixer. <br>
The toroid was a Fair rite material 61 ferrite toroid with trifilar wire turns. <br>

## Local Oscillator
The local oscillator was a modified circuit, originally found in *Complete Wireless Design* by Cotter W. Sayre. 
To not load the oscillator, a buffer (common emitter) was added for isolation and then a common emitter amplifier to provide the needed LO drive for the mixer LO input. <br>

## Intermediate Frequency Band Pass Filter
The IF BPF was chosen to be a SAW filter. This has a nice 50 ohm broadband termination and helps reject image frequencies, which lie at $\pm 2f_{LO}$. <br>

## Intermediate Frequency Amplifier
Class A amp or OPAMP? <br>

## Demodulator
Discriminator? <br>
