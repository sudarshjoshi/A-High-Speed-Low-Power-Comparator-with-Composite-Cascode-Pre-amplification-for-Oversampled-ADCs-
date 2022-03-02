# A High Speed Low Power Comparator with Composite Cascode Pre amplification for Oversampled ADCs with 28nm technology
This repository presents the design of a High speed and low power comparator with composite cascode preamplification for oer sampled ADCs. It was implemented on synopsys custom compiler tool using 28nm technology.
## Table of Contents
- [Abstract](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#Abstract)
- [Introduction](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#Introduction)
- [Circuit Design](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#circuit-design)
- [Simulation Results](https://github.com/sudarshjoshi/A-High-Speed-Low-Power-Comparator-with-Composite-Cascode-Pre-amplification-for-Oversampled-ADCs-/edit/main/README.md#simulation-results)
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
The total power consumption of the comparator is 65.88µW and the total approximated area occupied by comparator
is 29.16µm2.

## Introduction
Comparators play a very important role in analog to
digital conversion for increasing the overall performance
of the system. Usually in any ADC the comparator
consumes most power of the core (e.g., in Flash type
ADC for n bit resolution 2n
-1 number of comparators are
needed). Hence intelligent design methodologies are
highly needed for low power –reduced area design.
With miniaturization of circuit, the design of
comparators for low supply voltages is a
challenging task. The main cause of problem in low
voltage design is that threshold voltage and VDSAT does
not scale down with supply voltage or with smaller size
technologies. This work presents a high speed uncompensated
comparator with reduced area and power.

## Circuit design

1.The first stage of the comparator circuit consist of a composite cascode preamplifier.This composite cascode stage has the following
advantages over conventional cascode. First it reduces the
bias headroom voltage required and second it provides
higher output impedance at low bias current hence being
more power efficient. 

<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126729-b264500f-b4ce-4526-9625-697168610245.JPG">
 <img src="https://user-images.githubusercontent.com/100463400/156126731-0d9065ac-85a2-4e53-90af-a32cf278dd0c.JPG">
</p>
<br>
<p align="center">
Fig 1 . Schematic and symbol Composite cascode preamplifier
</p>
<br>
2. The second stage is a latch circuit formed by
the cross coupled NMOS pair. The output
of preamplifier acts as input of latch.
<br>


<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126719-226b17bd-1490-473d-be0a-7b2ebc25b04f.JPG">
 <img src="https://user-images.githubusercontent.com/100463400/156126721-128e2d70-b2c0-4bb6-a85d-c6628c9b0352.JPG">
</p>
<br>
<p align="center">
Fig 3 . Schematic and symbol of Latch
</p>
<br>
3. The outputs of latch goes to the inputs of third stage which is a diffrential amplifier. The differential ampplifier compares the voltage difference of othe the inputs and returns the corresponding high and low values to the input of next stage. 
<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126708-30cda077-2d68-44e8-add2-c5de61fa3ba9.JPG">
 <img src="https://user-images.githubusercontent.com/100463400/156126712-0ce353a7-5aad-408f-a43e-3d6e772ca81f.JPG">
</p>
<br>
<p align="center">
Fig 2 . Schematic and symbol of Self biased diffrential amplifier
</p><br>
4. The last stage is a pushpull driver. This driver is a cmos logic that drives the output to vdd and gnd(higgh and low) depending on the corresponding inputs.
 <br>
<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126739-d7a0658e-8392-4537-9d6f-8c0d3a5ae268.JPG">
 <img src="https://user-images.githubusercontent.com/100463400/156126737-717e705d-2641-4333-9a45-a788c9f09973.JPG">
</p>
<p align="center">
Fig 4 . Schematic and symbol of Pushpull driver
</p> 
5. After connecting all the blocks as shown in the figure 5 we get the final design of the compparator. Two sine voltages phase shifted by 90 degrees and of magnitude 0.8V are applied to the inputs of cascode amplifier. Vdd is taken 1.8V and outpt is taken from puushpull driver.

<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126713-08c196e0-fa73-41ef-b5d4-4f350c7aaf46.JPG">
<p align="center">
Fig 5 . Schematic and symbol of final circuit.
</p>


## Simulation Results

The transient analysis of the composite cascode comparator is shown in figure 6. The comparator output is high whenever the input signals are same and greater than zerro and the comparator outpput is low wheneer the input signals are equal and less than zerro. because of the pushpull driver the high and low vvalues of comparrator is 1.8V and 0V(vdd and gnd).

<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126741-eba4f177-cf38-4fb5-8ce1-5b2a75dcb742.JPG">
</p>
<p align="center">
Fig 6. Transient response of comparator
</p>
The DC characterstics atte presented in figure 7. The DC characterstics are otained by keeping one input signal to ground and sweeping another source linearly.
<br/>
<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126750-3a359606-f9f6-46d1-bb0f-0dfbefe133bb.JPG">
</p>
<p align="center">
Fig 7. The DC characteristic of comparator
</p>
To test the power consumed by the design we will check the maximum value of current offered y the supply vdd. TThe product of maximum current and spply voltage will provide power consumed by the circuit.

<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126726-205e01a7-ae32-4577-a4d4-20b1fdbba13a.JPG">
</p>

<p align="center">
Fig 8. Testing final design for power calculations.
</p>


<p align="center">
<img src="https://user-images.githubusercontent.com/100463400/156126749-917fdb5e-e82a-4efc-90ce-7df82060e5ef.JPG">
</p>

<p align="center">
Fig 9. Current wave form through vdd.
</p>

<b>Power calculation</b><br>
Power=Imax*VDD<br>
     =36.6u*1.8<br>
     =65.88uW



<b>Area calculation</b><br>
area of the chip can be calculated by:- <br>
W/L raito of one transistor 1.5u/0.6u.<br>
since w=1.5u and l=0.6u, area=(numer of transistors used*(w*l))+(20% of wire length)<br>
Area = 27*(1.5u)*(0.6u) + (27*(1.5u)*(0.6u))*20/100<br>
Area=29.16um2

      



## Performance Comparison

|               |      [1]      |   This work   |
|     :---:     |     :---:     |     :---:     |
|     Vdd (V)   |      1.2      |      1.8      |
|Technology (nm)|      180      |      28       |
|  Power (mW)   |      71.5uW      |      65.88uW     |
|Chip Size (um sq) |   694um2      |      29.16um2    |
<br>
The table presents performance comparison with previously done work in literature. It is clearly observed that we have significant reduction in the chip size(Area). We were also ale to reduce the the power 5.62uW even after using supply of 1.8V.

## Conclusion
The repository presents the design and simulation of Composite cascode comparator with 28nm technology node. The design consumes 65.88uW power at 1.8V and area reduced to 29.16um2 from 694um2.

## Author
Sudarsh Joshi, m.Tech, Thapar Institute of Engineering and Technology Patiala, punjab.
## Acknowledgements
- [Kunal Ghosh, Co-founder, VSD Corp. Pvt Ltd.](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3B0xcWjpLDThSEo6S9UPO9Tw%3D%3D)
- Chinmay Panda, IIT Hyderabad
- [Synopsis Team/Company](synopsys.com/company/contact-synopsys/office-locations/india/about-synopsys-india.html)
- [IIT Hyderabad](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)

## References
1. P. E. Allen and D. R. Holberg, CMOS Analog Circuit Design, IInd
Ed., New York: Oxford University Press, 2004..
2. R. He and L. Zhang, “Evalutation of modern MOSFET models
for bulk driven applications,” in Proc. IEEE 51st Midwest Symp.
on Circuits and Systems, 2008, pp. 105-108.
3. S. S. Rajput and S. S. Jamuar, “Low voltage, low power, high
performance current mirror for portable analogue and mixed mode
applications,” in Proc. IEEE Circuits, Devices and Systems, vol.
148, 2002, pp. 273-278.
4. C. G. Yu and R. L. Geiger, “Very low voltage operational
amplifiers usign floating gate MOS transistor,” in IEEE Int. Symp.
on Ciruits and Systems, vol. 2, 1993, pp. 1152-1155.
5. D. J. Comer, D. T. Comer, and C. Petrie, “The utillity of
composite cascode on analog CMOS design,” Int. J.of Electronics,
vol. 91, no. 8, pp. 491-502, 2004. 


