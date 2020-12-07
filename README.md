# THE GEM

 State of the art GROW LED light w. current injection 25-30amp
 
  ![TOP](https://github.com/Juanduino/THE-GEM/blob/main/Images/GEM_perspective.PNG)
 
 This is a PAR light project based on the high-current controller M4SUBDRV (https://github.com/Juanduino/THE-DIMMER_M4SDRV_V1)
 
 The CREE XLAMP LED´s is one of the most advanced horticultural light emitters on the market. They have a huge µmol/watt output. (Source: https://www.cree.com/led-components/media/documents/CreeXLampHorticultureFeatureSheet.pdf)
 
 One controller can inject current into 4 seperate channels of up to 6 amp per channel. Furthermore there is a 5th WHITE LED channel, with a MOSFET on the lamp, which is controlled by the MCU. Each WHITE LED is driven @2000mA (MAX) x 6 LED´s per board @12v = 4 amp. (note: The white LED´s heats up faster compared to red´s and blues. 700mA per string (3 LED´s) is more realistic.
 
 Each red string is driven @MAX 1500mA, so 3 red amp per GEM. The Blues is driven @MAX 2000mA, which equals a total of (3red + 4blue + 1.4white = 8.4 AMP) x 3 boards per controller = 25,2 AMP @MAX. (approx. 300watt) 
 
 The boards is designed, so that they can be put in a line. That is, the 3 boards will be parrallel connected and is internally routed to withstand the needed current flow.
 
 Two controllers (6 lamps) will run of a 12v 500-600watt PSU (Powersupply). Many have old PSU´s sitting in computers, which typically have a 500watt capasity.
 
 The goal of the project is to make a smart plant grow light, which controls the light intensity based on temperature sensor input.
 
 By making the lamp output pwm and temperature controlled, the final capacity of the lamp depends on the amount of cooling applied or the amount of heat allowed.
 
 Because the controller can be connected to a CAN (Controller Area Network) and USB, you can monitor and control each string/color (Red, Blue, White)

 
 ![TOP](https://github.com/Juanduino/THE-GEM/blob/main/Images/TOP.PNG)
 
 HEAT CIRCULATION
 
Although LED´s have become more efficient than the old gas-type bulbs, when driving the LED´s with high currents, there will be generated heat. How to re-cirkel and use that energy is a major task.

Case: Imagine a part of your living space, where you can grow greens all year round, and at the same time use the heat-output to warm up your space. This could especially benefit families in developing countries, where this type of technology, not only can provide food all year, but also expand the outdoor season by starting sprouts indoor, in a controlled environment, before they are ready to be planted out. 

Another mayer benefit by utilising the radiated heat, is the possibility to fully heat your living space with green energy. This means less foresting for wood to burn. Less Co2 emissions from NOT BURNING WOOD or other carbon-based energy sources. Naturally all this requires a solid environmentally friendly energy infrastructure.

By introducing CAN (Controller Area Network) to the "intelligent" GEM/lamps, and possibly wireless connections, there are many possibilities to make smart solutions for re-circulation of the heat-output.

![x4](https://github.com/Juanduino/THE-GEM/blob/main/Images/GemX4_top.PNG)

A larger version, without the possibility or need to connect smaller Gem´s. approx 400w (MAX) 

 ![TOP](https://github.com/Juanduino/THE-GEM/blob/main/Images/GemX4_back.PNG)
 
 Changelog:
 
 My Focus is now the 400watt lamp and to cut down on complexity.
 
 Have decided against the 5th LED channel. The white LED´s will be mounted on a fully white and bright GEM. The GemX4 is still 98 very intens LED´s, so the reeason is also based on a considoration for the final BOM count and the fans current consomption.

White LED´s use energy to lite up the full visible spectrum. The Red and Blue only one wavelentht(area) and  is terefore cooler in use. The difference  between the red and blue wavelength  is another matter. 

Added 4 4pin PWM FAN plug headers. One is for the outtside end-fan, which sits just before the controller and therefore cools the conttroller alswell.

For office invironment the fully white GEM would be more pleasant for the  humaan eye.  In a school schenario the lamps would  be part of  photon to plant  growth process. 

Inside the lamp another 3 eg. 60mm fans can be mounted. This all  depennds on the enclosure design. The fans will be controlled by a common PWM puls.


 ![perspectve](https://github.com/Juanduino/THE-GEM/blob/main/Images/perspectve.PNG)
 
 To connect a 120mm fan as the front cooller,  you need the adabtor 3D print  file.
 
 As seen in above image, the power cables can be solderen in  by using the  split&twist tech.
 
 To add wireless com. you need a Bluetooth / Wify or NB add-onn module on the I2C or SPI bus.
 
 (Controller: https://github.com/Juanduino/THE-DIMMER_M4SDRV_V1)
 
  ![Adaptor](https://github.com/Juanduino/THE-GEM/blob/main/Images/adaptor.jpg)
  
   ![Enclosure](https://github.com/Juanduino/THE-GEM/blob/main/Images/GEM_enclosure_OpenLight.jpg)
   
 
Added 4 x MAX31725MTA+T temperature sensor on I2C bus. (up to 150C). (https://datasheets.maximintegrated.com/en/ds/MAX31725.pdf)

  ![TipTop](https://github.com/Juanduino/THE-GEM/blob/main/Images/TOP2.PNG)
  
  
 
