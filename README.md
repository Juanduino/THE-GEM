# THE GEM
 State of the art GROW LED light w. current injection 25-30amp
 
 This is a PAR light project based on the high-current controller M4SUBDRV (https://github.com/Juanduino/THE-DIMMER_M4SDRV_V1)
 
 The CREE XLAMP LED´s is one of the most advanced horticultural light emitters on the market. They have a huge µmol/w output. (Source: https://www.cree.com/led-components/media/documents/CreeXLampHorticultureFeatureSheet.pdf)
 
 One controller can inject current into 4 seperate channels of up to 6 amp per channel. Furthermore there is a 5th WHITE LED channel, with a MOSFET on the lamp, which is controlled by the MCU. Each WHITE LED is driven @350mA x 6 LED´s per board = 2.1 amp.
 
 Each red string is driven @MAX 1500mA, so 3 red amp per GEM. The Blues is driven @MAX 2000mA, which equals a total of (3red + 4blue + 2.1white = 9.1 AMP) x 3 boards per controller = 27.3 AMP @MAX.
 
 The boards is designed, so that they can be put in a line. That is, the 3 boards will be parrallel connected and is internally routed to withstand the needed current flow.
 
 Two controllers (6 lamps) will run of a 12v 500-600watt PSU (Powersupply). Many have old PSU´s sitting in computers, which typically have a 500watt capasity.
 
 The goal of the project is to make a smart plant grow light, which controls the light intensity based on temperature sensor input.
 
 By making the lamp output pwm and temperature controlled, the final capacity of the lamp depends on the amount of cooling applied or the amount of heat allowed.
 
 Because the controller can be connected to a CAN (Controller Area Network) and USB, you can monitor and control each string/color (Red, Blue, White)

 
 ![TOP](https://github.com/Juanduino/THE-GEM/blob/main/Images/TOP.PNG)
