# A High Speed Low Power Comparator with Composite Cascode Pre amplification for Oversampled ADCs with 28nm technology
## Table of Contents
- [Abstract](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#Abstract)
- [Introduction](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#Introduction)
- [Device Characterization](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#device-characterization)
- [Circuit Design](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#circuit-design)
- [Simulation Results](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#simulation-results)
- [Netlist](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#netlist)
- [Performance Comparison](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#performance-comparison)
- [Conclusion](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#conclusion)
- [Author](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#author) 
- [Acknowledgements](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#acknowledgements)
- [References](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#references)
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

## Performance Comparison

|               |      [1]      |   This work   |
|     :---:     |     :---:     |     :---:     |
|     Vdd (V)   |      1.2      |      1.8      |
|Frequency (GHz)|      4.0      |     0.45      |
|Technology (nm)|      180      |      28       |
|     Gain      |      1.3      |     1.015     |
|  Power (mW)   |      71.5uW      |      65.88uW     |
|Chip Size (mm sq)    0.82      |      -     |
The table presents performance comparison with previously done work in literature. A clear trade off between gain and power can be observed here. The chip area can be determined with post layout measurements and is expected to be smaller than higher technology nodes.
## Conclusion
The repository presents the design and simulation of Gilbert cell based mixer on 28nm technology node. The design consumes  f power at 1.8V and provides nearly unity gain. Future works can include improvement of conversion gain and increase in linearity by using better designs and biasing techniques. 

## Author
Sudarsh Joshi, m.Tech, Thapar Institute of Engineering and Technology Patiala, punjab.
## Acknowledgements
- [Kunal Ghosh, Co-founder, VSD Corp. Pvt Ltd.](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3B0xcWjpLDThSEo6S9UPO9Tw%3D%3D)
- Chinmay Panda, IIT Hyderabad
- [Synopsis Team/Company](synopsys.com/company/contact-synopsys/office-locations/india/about-synopsys-india.html)
- [IIT Hyderabad](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
- Active and vibrant hackathon community

