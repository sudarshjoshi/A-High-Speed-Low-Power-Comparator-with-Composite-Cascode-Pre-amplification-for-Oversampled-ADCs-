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

## circuit design
<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126708-30cda077-2d68-44e8-add2-c5de61fa3ba9.JPG">
 <img src="https://user-images.githubusercontent.com/100463400/156126712-0ce353a7-5aad-408f-a43e-3d6e772ca81f.JPG">
</p>


![finalcircit](https://user-images.githubusercontent.com/100463400/156126713-08c196e0-fa73-41ef-b5d4-4f350c7aaf46.JPG)
![latchschematic](https://user-images.githubusercontent.com/100463400/156126719-226b17bd-1490-473d-be0a-7b2ebc25b04f.JPG)
![latchsymbol](https://user-images.githubusercontent.com/100463400/156126721-128e2d70-b2c0-4bb6-a85d-c6628c9b0352.JPG)
![power wave forms](https://user-images.githubusercontent.com/100463400/156126725-435c6ece-1d1e-4149-b5eb-f4c728e17fad.JPG)
![powercalclations](https://user-images.githubusercontent.com/100463400/156126726-205e01a7-ae32-4577-a4d4-20b1fdbba13a.JPG)
![preampschematic](https://user-images.githubusercontent.com/100463400/156126729-b264500f-b4ce-4526-9625-697168610245.JPG)
![preampsymbol](https://user-images.githubusercontent.com/100463400/156126731-0d9065ac-85a2-4e53-90af-a32cf278dd0c.JPG)
![proposed](https://user-images.githubusercontent.com/100463400/156126733-8a740808-9668-469a-ba08-25098269c638.JPG)
![proposed3](https://user-images.githubusercontent.com/100463400/156126735-3e199e03-a49b-4715-92b0-799f52f25e27.JPG)
![pushpullsymbol](https://user-images.githubusercontent.com/100463400/156126737-717e705d-2641-4333-9a45-a788c9f09973.JPG)
![pushpuullschematic](https://user-images.githubusercontent.com/100463400/156126739-d7a0658e-8392-4537-9d6f-8c0d3a5ae268.JPG)

![Capture3](https://user-images.githubusercontent.com/100463400/156126744-a60986a6-c5a6-4bae-af84-c82b322c4424.JPG)
![Capture4](https://user-images.githubusercontent.com/100463400/156126745-bef7a2ca-7ffd-4726-b557-705ffc34550f.JPG)
![currentforpower](https://user-images.githubusercontent.com/100463400/156126749-917fdb5e-e82a-4efc-90ce-7df82060e5ef.JPG)
![dccharacterstics]()



## Simulation Results
<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126741-eba4f177-cf38-4fb5-8ce1-5b2a75dcb742.JPG">
</p>
<p align="center">
Fig 6. Mixer simulation input and output waveforms
</p>
The simulation of mixer was performed using specifications as presented in [1]. Fig 6. shows the mixer output waveform obtained by applying f_RF = 50MHz and f_LO = 450MHz. The resulting output signal has a frequency IF_1 = 400MHz and IF_2  = 500MHz. Note that the mixer provides almost unity gain or a conversion gain of 0.131dB precisely.
<br/>
<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126750-3a359606-f9f6-46d1-bb0f-0dfbefe133bb.JPG">
</p>
<p align="center">
Fig 7. DFT of output waveform
</p>
Fig 7. shows the output signal's DFT normalized wrt to peak frequency component. As can be observed, the spectrum peaks around f = 400MHz and f = 500MHz confirming the multiplying property. Intrestingly figure also shows presence of a 50MHz component as some of the RF signal gets leaked to the output.
<br/>
<p align="center">
<img src="https://user-images.githubusercontent.com/41693726/155829965-e9b49c90-fa84-4958-9092-fc9c61f89e83.png">
</p>
<p align="center">
Fig 8. Testbench used to determine -3dB point
</p>
Fig 8. shows the testbench setup used to determine -3dB point for the mixer. A "vsource" element is used to provide the RF and LO signal of amplitude 100mV. AC analysis was performed by using the default frequency as sweep variable and the magnitude of output differential signal was set as output. Note that the output signals are terminated with two NMOS source follower circuits to simulate the effect of connecting the mixer to further stages in an IC. 
<br/>
<p align="center">
<img src="https://user-images.githubusercontent.com/41693726/155829961-13622c5c-7f77-4aa9-aea0-61ac9921b12e.png">
</p>
<p align="center">
Fig 9. Magnitude plot of output signal
</p>
Fig 9. shows that the -3dB point for the mixer is achieved at a frequency of 7.14GHz. Hence the mixer can be easily used for ISM band between 902MHz and 928MHz as well.
<br/>
<br/>
<p align="center">
<img src="https://user-images.githubusercontent.com/41693726/155830279-15d2d7ff-7a21-42c6-bea2-0e55e32a6a5f.png">
</p>
<p align="center">
Fig 10. DC transfer curves of the mixer
</p>
Finally, Fig 10. presents the DC transfer curves of the designed mixer. The mixer lacks linearity especially for higher voltage levels of RF signal, this is evident from the unevenly spaced transfer curves which bunch up for higher RF voltage.

## Performance Comparison

|               |      [1]      |   This work   |
|     :---:     |     :---:     |     :---:     |
|     Vdd (V)   |      1.2      |      1.8      |
|Technology (nm)|      180      |      28       |
|  Power (mW)   |      71.5uW      |      65.88uW     |
|Chip Size (mm sq)    0.82      |      -    |
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

