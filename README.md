# RPiADF4351
Control an ADF4351 using spi on any GPIO pins from a Raspberry Pi

call using sudo ./adf4351 fff.f

fff.f is the frequency in MHz (>35 and <4400)

or sudo ./adf4351 off to turn the VCO off

GPIO pins for LE, CLK and DATA can be set in adf4351.c using wiringPi numbering.

# Adf4351 Evaluation Board Diagram.
Diagaram<br>
![Adf4351 Eval Board](images/Adf_4352_Diagram_1.png?raw=true "ADF4350 Eval Boards")<br>
Board picture<br>
![Adf4351 Eval Board](images/35M-4.4GHz_PLL_RF_Signal_ADF4351_1.png?raw=true "ADF4350 Eval Boards")<br>
# Checking your pin status and direction configuration.
The gpio should be installed by default on Raspberry pi<br>
Pins 17, 18, 19 and 20: (BCM_GPIO 28, 29, 30 and 31) These are additional GPIO pins on the Rev. 2 board.<br>
Remember: The Raspberry Pi is a 3.3 volt device! Attempting to directly connect to any 5V logic system will very likely result in tears…<br>
gpio -v<br>
gpio readall<br>
