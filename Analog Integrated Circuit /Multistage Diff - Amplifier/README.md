# Abstract
This project aims to design a Multistage Differential Amplifier. The project requires a cutoff frequency (or -3dB frequency) greater than 200 MHz, a Common-Mode Rejection Ratio (CMRR) of at least 100, and one percent linearity. 
To achieve these requirements, a two-stage OTA is used. The gain is about 24 dB, and the -3 dB frequency is 240 MHz. The common-mode gain is about -13 dB; thus, the CMRR is over 100. One percent linearity is also achieved after doing FFT analysis over a few frequencies.
A two-stage OTA design meets the requirements.
# Introduction
An operational transconductance amplifier, or OTA, is an operational amplifier that has high gain, high input impedance, and high output impedance. OTA's output is a current source. A two-stage amplifier allows for higher gain without reducing the output swing. The first stage is a differential amplifier, and the second stage is typically configured as a simple common-source amplifier.
The gain formula is: $A_{v} = A_{V1}A_{V2} = (-\frac{g_{m2}}{g_{o2}+g_{o4}})(-\frac{g_{m8}}{g_{o8}+g_{o7}})= \frac{g_{m2}g_{m8}}{(g_{o2}+g_{o4})(g_{o8}+g_{o7})} $
The cutoff frequency is where the gain decreases by -3 dB from the DC gain. The dB gain formula is: $dB = 20 \log A_{v}$. Common Mode Rejection Ratio, or CMRR, is the ratio between differential-mode to common-mode gain. 1% linearity is calculated with following formula:
$linearity percentatge = \frac{\sqrt{V_{2}^2+V_{3}^2+V_{4}^2}}{V_{1}} \cdot 100 \%$
# Design Considerations
# Simulation Results \& Discussion
# Conclusion
