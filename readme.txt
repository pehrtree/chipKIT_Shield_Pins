Comparing pin conflicts between the chipKIT Basic I/O shield and Network+USB Shield when used on chipKIT Max32

I noticed at least one possible correction to the Basic I/O shield docs - for max32 BTN 3 & 4 should be pins 80 & 81 respectively. 
This is based off the schematics and not seeing the physical hardware.

Overall impression with using these  two shields together:

> the slide switches are compromised:
SW1 (pin 2) impacts USB, and SW2 (pin 7) impacts Ethernet (NRST means reset?)

> I2C #1 is used by both shields in the form of daisy chain headers, and I/O shield has a temperature sensor on I2C#1

For just the network shield, I2C #1 and USB conflict but that is jumperable and mentioned in docs



chipKIT Max32   https://www.digilentinc.com/Products/Detail.cfm?NavPath=2,892,894&Prod=CHIPKIT-MAX32

Basic I/O shield  https://www.digilentinc.com/Products/Detail.cfm?NavPath=2,892,936&Prod=CHIPKIT-BASIC-IO-SHIELD

Network shield   https://www.digilentinc.com/Products/Detail.cfm?NavPath=2,892,942&Prod=CHIPKIT-NETWORK-SHIELD

board diagrams from Fritzing

http://fritzing.org/projectschipkit-max32
http://fritzing.org/projectschipkit-boards
