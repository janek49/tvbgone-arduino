# Arduino TV-B-Gone
I created this improved version of the TV-B-Gone for Arduino, since the one on the Internet is outdated (from 2010), 
only works for some AVRs (Atmega328P) and uses a poorly coded method to send IR signals. Also all IR codes are saved
in a RAW format (on/off pulses) which doesnt make it easy to add new codes.

My version uses z3t0's Arduino-IRremote library ([Arduino-IRremote](https://github.com/z3t0/Arduino-IRremote)) which can be compiled
for a lot of AVRs and can send many codes as a HEX value, so you don't need the RAW code (which would take a lot of space).

You can use the IRrecvDump project example from the library to dump codes from the remote.
I provide a modified version of the IRrecvDump which has some improvements like more remote types and better readability.

