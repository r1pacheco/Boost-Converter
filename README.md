# Boost-Converter

<h3>This board was designed specifically for the R3 rover and has major restraints that were followed: </h3>

* Maximum dimensions of 42mm x 48mm x 23mm to remain inside the restrictions of the PDB (Power Distribution Board)
* Header space is required so parts do not overlap or bump edges as it is a tight fit within the chasis and the Molex connectors 
* Needs to handle a minimum of 5 amps and increase voltage from 15 to 24 volts minimum (my actual design uses a 5KΩ potentiometer to vary the desired voltage at the output, to make it more flexible for future use if needed)

|Top Side|Bottom Side|
|---|---|
|![boost-board-top](https://user-images.githubusercontent.com/60334970/135769116-7a419783-e0e2-4d9f-b82b-afef222b671e.png)|![boost-board-bot](https://user-images.githubusercontent.com/60334970/135769117-e66f8f99-b769-4a2a-8583-a162a0c1a73b.png)|  

*Click the above photos for a larger view*





<h3>Details and considerations made to improve the boards design and functionality:</h3>

* Thick traces or polygons are used to handle large current as well as act as heat displacers 
* Room for large external heat sinks was needed to help cool down the MOSFET and large diode on the board since they handle the bulk of the current
* Vias were also used to help give direct air flow to the main IC and fuse holder 
* a physical cutout (notch) was placed in the PCB beside the horizontal fuse holder, making it easier to set/remove the fuses (they can be tight sometimes)
* Large polygons were used where the most current would travel to make sure traces did not burn up and can disipate as much heat as possible
* all large capacitors/inductors were kept to one side of the board so they would not interfere with external Molex connectors on the PDB board. This is needed since the right side of the board will be overlapping pre-existing components and we needed the compensated space
* LED indication tells the user if the board is being used and is working properly
* overall board size was given tolerances of 1mm x 1mm x 1mm so they did not interfere with other external boards. Chamfers were also added for the same reason

