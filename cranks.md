# Cranks and Bottom Bracket

## Cranks

The S2 uses a square taper axle with an M10 threaded bolt.

### Removing the Cranks

#### Tools needed

* 8mm Hex Wrench or Socket
*  [Crank Puller](https://www.parktool.com/en-us/product/crank-puller-for-square-taper-cranks-ccp-22)
  
Park Tool has a [guide on removing square taper cranks](https://www.youtube.com/watch?v=uO_GzqqJTXU).

1. Remove the bolts from the left crank with the 8mm hex wrench.
1. Thread the crank puller onto the crank arm. Ensure as many threads are engaged with the crank arm as possible to avoid stripping out the internal threads on the arm.
1. Rotate the crank puller until the crank is removed from the square axle.
1. Unthread the crank puller from the crank arm.
1. Repeat for the right side crank.

## Bottom Bracket

The bottom bracket on the S2 is a Bafang Speed sensor. It uses a hall effects sensor to determine when the cracks of the bike are rotating (need to verify). It uses a 6-Pin Julet Mini Connector to connect to the wiring harness of the bike.

[OEM Manual](https://www.bafang-e.com/uploaded/manual/BF-DM-C-SR%20PA1XX-EN.pdf)

[Replacement Part](https://www.aliexpress.us/item/3256805478774668.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.3.53f1WKh5WKh5Jh&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=13c18982-0647-4d66-a721-780df36c8ce7&_t=gps-id:pcDetailTopMoreOtherSeller,scm-url:1007.40050.354490.0,pvid:13c18982-0647-4d66-a721-780df36c8ce7,tpp_buckets:668%232846%238111%231996&pdp_npi=4%40dis%21USD%2143.39%2123.86%21%21%2143.39%2123.86%21%402101ef5e17120734268176713e9bc5%2112000033943376182%21rec%21US%21%21AB&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A)

### Removing the Bottom Bracket

#### Tools needed

* [Park Tools BBT-32](https://www.parktool.com/product/bottom-bracket-tool-bbt-32?category=Crank%20%26%20Bottom%20Bracket)
* [A Pick or Other Pointed Object](https://www.parktool.com/en-us/product/utility-pick-set-up-set)

Park Tool has a [guide on removing bottom brackets](https://www.youtube.com/watch?v=xUtOeFJJycg).

1. Remove the bottom cover from the battery compartment on the bottom of the downtube.
1. Unplug the connector from the bottom bracket.
1. Follow the steps in [Removing the Cranks](cranks.md#removing-the-cranks)
1. Start on the non-drive side of the bike.
1. Using a pick or other pointed object, remove the rubber dust cover from the internal threads on bottom bracket.
1. Insert the BBT-32 into the internal spines.
1. Rotate the tool counter-clockwise until the cup is removed.
1. Repeat on the drive side.

## Electronics
![cadence_sensor_pinout](https://github.com/Tenkir/vanmoof-s2-user-manual/assets/3649828/1ecce671-f717-409f-9a79-7aba50738b58)


The bottom bracket sensor outputs a +5v square wave when the pedals are turned. The frequency of the square wave increases as the cadence of rotation increases. However, the Vanmoof S2 does not appear to use the frequency for anything, as feeding the controller a 1Hz square wave results in the hub motor spinning at the same RPM as a 70Hz square wave.

![SDS00014](https://user-images.githubusercontent.com/3649828/219869444-4c52f0bc-be28-4c2a-bb6b-ca33cb51ef78.png)
