# Cranks and Bottom Bracket

## Bottom Bracket

The bottom bracket on the S2 is a Bafang Speed sensor. It uses a hall effects sensor to determine when the cracks of the bike are rotating (need to verify). It uses a 6-Pin Julet Mini Connector to connect to the wiring harness of the bike.

[Replacement Part](https://www.aliexpress.com/item/1005002790035485.html)

### Tools needed

* [Park Tools BBT-9](https://www.parktool.com/product/bottom-bracket-tool-bbt-9)
* [Park Tools BBT-32](https://www.parktool.com/product/bottom-bracket-tool-bbt-32?category=Crank%20%26%20Bottom%20Bracket)

## Electronics

The bottom bracket sensor outputs a +5v square wave when the pedals are turned. The frequency of the square wave increases as the cadence of rotation increases. However, the Vanmoof S2 does not appear to use the frequency for anything, as feeding the controller a 1Hz square wave results in the hub motor spinning at the same RPM as a 70Hz square wave.

![SDS00014](https://user-images.githubusercontent.com/3649828/219869444-4c52f0bc-be28-4c2a-bb6b-ca33cb51ef78.png)
