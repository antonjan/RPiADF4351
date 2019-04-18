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
