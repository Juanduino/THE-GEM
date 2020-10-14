# THE GEM
 State of the art GROW LED light w. current injection 25-30amp
 
 This is a PAR light project based on the high-current controller M4SUBDRV (https://github.com/Juanduino/THE-DIMMER_M4SDRV_V1)
 
 The CREE LED´s is one of the most advanced horticultural light emitters on the market. They have a huge umol/w output.
 
 One controller can inject current into 4 seperate channels of up to 6 amp per channel. Furthermore there is a 5th WHITE LED channel, with a MOSFET on the lamp, which is controlled by the MCU. Each WHITE LED is driven @350mA x 6 LED´s per board = 2.1 amp.
 
 The goal of the project is to make a smart plant grow light, which controls the light intensity based on temperature sensor input.
 
 By making the lamp output pwm and temperature controlled, the final capacity of the lamp depends on the amount of cooling applied.
 
 Because the controller can be connected to a CAN (Controller Area Network) and USB, you can monitor and control each string/color (Red, Blue, White)

 
 ![TOP](https://github.com/Juanduino/THE-GEM/blob/main/Images/TOP.PNG)
