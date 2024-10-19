# Smart Cartridge

## Opening the cartridge

![smart cartridge opened](https://github.com/Silly105/vanmoof-s2-user-manual/assets/9697253/8a848530-7ca0-48d1-8916-73eab73de488)

### Adhesive sealings

To seal the smart cartrige against moisture, Vanmoof used self adhesive sealings, which glue the case parts together. It is challenging to remove components or opening the casing without damaging that sealings. To regain an airtight seal after opening, these parts have to be sealed of, for instance with using silicone or 2mm wide sealing tape from smartphone repair kits. 
This are the are all sealings in the cartridge:

![sealings](https://github.com/Silly105/vanmoof-s2-user-manual/assets/9697253/47ecb095-8c34-4625-b74d-b72336cdc1c1)

### Accessing the cartidge battery

The cartridge is equipped with an own li-ion battery independent from the battery back. It can be charged without opening the cartridge (see Error Resolution). If the battery needs replacement or needs to be checked for damages, use the following steps to expose it.

WARNING: Opening the smart cartridge and exposing the circuit boards can damage/destroy the components. Do not open if you have other options of repairing.

![accessing cartridge battery 1](https://github.com/Silly105/vanmoof-s2-user-manual/assets/9697253/1f041e01-cbf6-453d-9b7f-aa94f35cb634)
![accessing cartridge battery 2](https://github.com/Silly105/vanmoof-s2-user-manual/assets/9697253/0e34abf1-5330-4493-9916-09bb4b79a64d)

1. Open the small separate compartment, the edges are glued, opening will need mild force. There is a plugged connection inside. When lifting the case top, that plug has to be carefully pushed inside the cartridge so the wires are not damaged.

2. The matrix display has to be removed. The contacts are protected by a glued seal, too. Carefully use some force, ideally with levering close to the contacts.

3. To finally open the cartidge enclosure, again some force is needed after unscrewing. Most of the casing is glued, but can be opened without destroying the case parts by carefully levering with a thin but sturdy object. Most knives will do. The sealing will probably be damaged and needs replacement.
   
4. The battery is soldered under this board. Unscrew here.

5. Now you can reach the battery contacts for measuring voltage etc. If you need to unsolder it, the plugged connections to the board need to be unplugged.


## MCU

The core of the Smart Cartridge is a  [tm4c123gh6pmi7](https://octopart.com/tm4c123gh6pmi7-texas+instruments-47641106) microprocessor.

## Scortched Charger Connector

![image](https://github.com/user-attachments/assets/a6deee61-beff-4f20-b883-10536af30d02)

A common issue with the charging system of the Vanmoof is the connector from the charging port to the main board arcs and scorches. This can often manifest as the bike not charging.

There are two solutions for this: replace the connector with a higher quality name-brand part, or solder the wires directly to the header.

### Replacement with Higher Quality Components

The OEM connectors used are knock off Molex connectors, which seem to be unable to handle the required load. Replacement with name-brand Molex connectors seem to perform much better in this application, and I have not received any reports of this issue reoccuring after replacement with higher quality components.

Per the [datasheet for the Molex connector](https://www.molex.com/en-us/products/part-detail/09503021?display=pdf), these connectors are rated for up to 600V DC @ 4.00-5.00A (depending on wire guage), which is well within the 42v DC @ 2.3A the Vanmoof charger puts out.

[Headers](https://www.mouser.com/ProductDetail/538-171814-0002)

[Housing](https://www.mouser.com/ProductDetail/538-09-50-3021)

[Crimp Pins](https://www.mouser.com/ProductDetail/538-08-50-0106)

Cut off the existing wire housing and crimp pins, strip the wires, and crimp on the new pins. Insert them into the housing, ensuring the polarity remains the same as the original connector. Then reinsert the connector.

Desolder the existing header pins from the PCB and solder the placement headers in the same location.

### Soldering The Wires Directly

Some users may prefer to solder the wires directly and avoid the connector entirely. [iFixit has a guide on soldering the wires directly.](https://www.ifixit.com/Guide/Fix+for+Vanmoof+S2+Not+Charging/157499#s329204)

## Error Resolution

### Reset the Smart Cartridge

The first step in resolving an error or issue with the Smart Cartridge is to reset it with the small reset button. Vanmoof has a guide on this (note, the guide is for the S3, but it's the same process for the S2).

https://support.vanmoof.com/en/support/solutions/articles/44002069054-how-do-i-reset-the-vanmoof-s3-x3-

### Charge the Smart Cartridge

If resetting the Smart Cartridge did not resolve the issue, or the bike is completely non-responsive after charging for 5 or more hours, attempt to charge the Smart Cartridge iself.

1. Remove the Smart Cartridge from the bike.
2. On the right side of the Smart Cartridge, remove the small rubber flap.
3. Plug a mini-USB charger into the mini-USB port under the rubber flap.
4. Charge for 1hr
5. Return the Smart Cartridge to the bike, ensuring it's pressed firmly back into place.
6. Turn on the bike.

## Error 29

Error 29 indicates a communication issue with the battery.

## Error 27

Error 27 indicates a communication issue with the battery.
