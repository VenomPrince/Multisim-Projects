# Multisim-Projects
These are just some fun stuffs i did. 
# For PrinceHighPassFilter File
The aim was to achieve an output of 11 dB at a frequency of 3 kHz. The 4th order filter was designed as follows: starting from the first amplifier (CA3140M) and the second amplifier (CA3140M), the configuration was arranged to provide an output of approximately 8 dB.

Since this is a high-pass filter (HPF), the non-inverting input of the amplifiers was connected through capacitors of 10 µF. The inverting input was connected to a resistor divider network with a default ratio R3/R4, where R4 was grounded and R3 was connected to the output of the first amplifier. Similarly, the feedback resistor was connected between the output and the inverting input. The same configuration was used for the second amplifier.

The resistor values R1, R2, R5, and R11 were calculated using the formula:
f=1/2πRC

where
f=3kHz and C=10×10−9 F

The values of R3 and R4were determined using the ratios provided in a Butterworth response table for a 4th order filter.

In this setup, the two amplifiers connected in series gave a total gain of 8 dB. However, since the required output was 11 dB, an additional amplifier stage was designed to add the remaining 3 dB.

For the final amplifier, a non-inverting configuration was used, and the gain was calculated using the formula:
Av=1+Rup/Rground

To achieve 3 dB, the dB value was converted to a linear value and substituted into the gain formula to calculate the resistor values. These resistors were then placed as shown in the schematic.

Please note that the values used in the schematic might differ slightly due to the availability of practical components in the lab. Minor modifications were made to optimize performance. If you prefer, you can simulate the circuit using exact theoretical values. The circuit works in both cases.

The calculations and response graphs were performed using an AC sweep. To verify, label the final output as "Out" in the AC sweep, run the simulation, and observe the output. This process should also be repeated for the first two amplifiers to confirm their dB contribution and determine how much gain is still needed.

If you have any confusion, feel free to ask!
