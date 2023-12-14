# Roastuino-Fluidbed-Roaster

This roaster contains the same PID Roastuino v1.0 (hardware and software) like in the Popper Roaster project. Only difference is: we need the Fotek SSR 40 DA (for 2000W Heater) and a heat sink must be mounted on the SSR and IRF540 MOSFET (air pump driver).

The “rocket style” and the shaker idee is coming from [this project (Thanks Greencardigan!)](http://www.homeroasters.org/php/forum/viewthread.php?thread_id=2509&rowstart=20) 

Here you can see some Test videos:

- Test 1: Air Pump – Power test: https://youtu.be/C2j7yd1C9AM
- Test 2: 100g Columbia coffee bean: https://youtu.be/3-mqRSu4GRM
- Test 3: Failed at 9:40 : https://youtu.be/tRvCNzrr7H0
- Test 4: 250g Columbia coffee bean, roasted succesfully: https://youtu.be/k_GJ-7MUQUI
- Roastuino Bluetooth Demo: https://youtu.be/n37bFz3xK2w

**Here you can find details about this project: [BOM, Schematic, Source Codes, Android APK](https://github.com/cyberelectronics/Roastuino-Fluidbed-Roaster/tree/main/Docu)**

For functionalities and software description, please visit the Popper Roaster project.

!!! Warning !!!
 NEVER LEAVE ROASTER UNATTENDED WHILE IN OPERATION !!!
Always ensure there is a circular motion of the green beans in the roaster by adjusting the FAN speed, otherwise the beans can catch fire !!! First time make some tests without turning on the Heater!
Roastlogger will Start with 100% Heat and 0% FAN! Do not plug in (~230V) the Heater while you didn’t set the Heat Power (slider) to 0% ! 
Build and / or use at your own risk !!!
 

Default PID settings:  P = 100;  I = 0;  D = 0;

**My default Roast Profile for 300g green Columbia Coffee Beans:**

- Ramp 1 – 3:00 min – 160C – 100% FAN
- Ramp 2 – 4:00 min – 200C – 87% FAN
- Ramp 3 – 5:00 min – 234C – 63% FAN

then cool the beans with 87% FAN while bean temp drops below 50C (aprox. 2 min)

**My default Roast Profile for 300g green Ethiopia Coffee Beans:**

- Ramp 1 – 2:40 min – 160C – 99% FAN
- Ramp 2 – 4:30 min – 200C – 87% FAN
- Ramp 3 – 5:00 min – 234C – 63% FAN

then cool the beans with 87% FAN while bean temp drops below 50C (aprox. 2 min)

**Push Button functions:**

- S4 – ” START / STOP / SAVE″ – Start / Stop Manual and Auto Mode / Save Settings
- S3 – ” + ” – Increment Value
- S2 – ”  –  ″ – Decrement Value
- S1 – ” SELECT ” – Select variable which you want to change

Other functions available at startup (keep pressed then turn ON the controller):

- S4 – “PROFILE 1 ” – Load PROFILE 1 with 9 RAMP settings
- S3 – “PROFILE 2 ” – Load PROFILE 2 with 9 RAMP settings
- S2 – “PROFILE 3 ” – Load PROFILE 3 with 9 RAMP settings
- S1 – “PROFILE 4 ” – Load PROFILE 4 with 9 RAMP settings
- S3 AND S4 – “RESET RC” – Reset Roast Counter to 0
- S3 AND S2 – “BBCC PLOT” – Enable com. with BBCC Plotter – PID tuning (until Reset)
- S1 AND S2 – “SETTINGS” – Start Settings Mode (until Reset)

**Other Softwares and drivers needed for this project:**

- [Arduino](http://arduino.cc/en/Main/Software) (tested with 1.0.5 r2)
- [Adafruit MAX31855 Thermocouple Arduino library](https://learn.adafruit.com/thermocouple/using-a-thermocouple)
- [Processing](http://www.processing.org/download/) (for BBCC Plotter, optional)
- BBCC Plotter (for PID tuning, optional)
- [Roastlogger](http://homepage.ntlworld.com/green_bean/coffee/roastlogger/roastlogger.htm) (for PC Control and temp. curves display, optional)
- [Artisan](http://code.google.com/p/artisan/) (only for temperature curves display, optional)
- CP2102 USB driver (not needed for commercial Arduino Deumilanove / Uno boards)

