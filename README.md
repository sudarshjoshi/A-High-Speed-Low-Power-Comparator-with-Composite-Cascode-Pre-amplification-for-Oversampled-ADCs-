# Design and Simulation of a Gilbert Cell based Mixer on CMOS 28nm Technology
## Table of Contents
- [Introduction](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#introduction)
- [Device Characterization](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#device-characterization)
- [Circuit Design](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#circuit-design)
- [Simulation Results](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#simulation-results)
- [Netlist](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#netlist)
- [Performance Comparison](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#performance-comparison)
- [Conclusion](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#conclusion)
- [Author](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#author) 
- [Acknowledgements](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#acknowledgements)
- [References](https://github.com/SoumitroV/Design-and-Simulation-of-a-Gilbert-Cell-based-Mixer-on-CMOS-28nm-Technology/edit/main/README.md#references)
## Abstract
Abstract—This paper presents a high speed- low power
CMOS comparator using composite cascode differential
pair as a pre-amplification stage. The purpose of this work
is to design a comparator for oversampled ADC application.
This comparator is designed using 28nm CMOS
technology with a power supply of 1.8V. Pre and post layout
simulation of the proposed circuit is done using synopsys costom compiler tool.
The total power consumption of the comparator is 65.88µW
and unity gain-bandwidth is 1GHz. The DC offset voltage is
12mV, gain is 70dB while total area occupied by comparator
is 684µm2
. This design achieves an OSR (Oversampling
Sampling Ratio) greater than 1000 which corresponds to
SNR improvement of 30dB for Σ-Δ converters.
## Introduction
Analog to digital conversion is a key factor in any
electronic system. The analog data is converted to digital
data so that processing could be easy and storage of data
can be possible. ADC is categorized into Nyquist rate
ADC and oversampled ADC. Conventional Nyquist rate
converters need analog components which must be highly
immune to noise and interface, but oversampling
converters can be designed using simple and high
tolerance analog components.
Comparators play a very important role in analog to
digital conversion for increasing the overall performance
of the system. Usually in any ADC the comparator
consumes most power of the core (e.g., in Flash type
ADC for n bit resolution 2n
-1 number of comparators are
needed). Hence intelligent design methodologies are
highly needed for low power –reduced area design.
With miniaturization of circuit, the design of
comparators for low supply voltages (less than 3.3V) is a
challenging task. The main cause of problem in low
voltage design is that threshold voltage and VDSAT does
not scale down with supply voltage or with smaller size
technologies.
