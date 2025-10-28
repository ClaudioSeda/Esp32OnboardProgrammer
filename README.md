# Esp32OnboardProgrammer
🔌 You dont need to place serial to usb converters onboard! 
An easy way to upload you binaries to wroom modules.
Simply plug the programmer in your board and upload your binaries.
Cool way to produce you esp32 boards!

✳how to proceed in programming:

Put in your core pcb the same connections to GPIOS indicated in PROG CONNECTOR.
Conect directly. Its preferable to have only esp32 in the 3.3V bus in the moment of program upload. So plan to have a
solder junper in the VCC bus to transfer only the necessary vcc enerrgy to supply the esp32. After that close the solder jumper and be happy.



✅ This project is for very beginners from integrating ESP32 Wroom Modules in their PCBs.
There´s no need to embedded serial to Usb chips like CH340 in your core bords. You can 
simply plug the right connections and progra many PCBs fast and safelly.

🛡 I also encourage users to start to assemble in SMT,and loose their concerns and know it´s easy and FASTER than use
PTH!

🎞 here follows the schematics picture and BOM bellow:

<img width="904" height="630" alt="image" src="https://github.com/user-attachments/assets/36d6b947-79f1-43b9-b3c0-da293d45aa82" />

✅ 	C1	1uF

✅ 	C2	100n

✅ 	C3	220uF

✅ R3	470

✅ R4	470

✅ 	R5	470

✅ 	R6	470

✅ 	R7	470

✅ 	R1	10k

✅ 	R2	10k

✅ 	D1	LED

✅ 	D2	LED

✅ 	D3	LED

✅ 	U1	CH340C

✅ 	U2	AMS1117-3.3

✅ 	Q1	UMH3N

✅ 	Q2	UMH3N

✅ 	USB_Micro_SMD

✅ 	PROGOUT Connector 2.54mm pitch

<h1> Sponsorship</h1>
Special thanks for our Partner PCBWAY
<img width="1897" height="631" alt="image" src="https://github.com/user-attachments/assets/87560be4-191f-4f47-86c4-b96cbfc414fd" />

<img width="450" height="449" alt="image" src="https://github.com/user-attachments/assets/1ff3d151-3384-4f52-b880-b49dd4329af0" />
<h2> If you wish to implement this project, I highly recommend their service, as they are fast, reliable and produce high quality boards for a fair price.
<h2>https://www.pcbway.com/</h2>
  
🎞 PCBWay works with: 🎞


😍 3D prototyping,

😍 PCB design, 

😍 manufacturing and assembly,

😍and also with CNC metal fabrication.

💚  Thank you for sponsoring this project!</h2>



<h1> 🏆 TIPS:🏆 </h1>

✅ 1.  If you could,preheat your pcb (not burnit,only pre heat to almost 70 oC

✅ 2.  You will need to use solder flux (no clean or rosin) but dont leave,in case of rosin,to stay to much time in heat. Appy when you solder.

✅ 3. I strongly recomend you to try to use a STENCIL,but this board is very easy,it´s not a must. For mor complex and fine pitch components,it´s almost mandatory (QFN for example)

✅ 4. If you do a mistake,only remove and try it again,remove all solder from pads an do it again. 

✅ 5. I recommend do not use more than 400oC heat from your soldering iron/station.

✅ 6. Use a very fine tip.

✅ 7. Don´t try to solder components like resistors,capacitors all lose. Try fine tip tweezers.
<img width="888" height="1225" alt="image" src="https://github.com/user-attachments/assets/62a5ddfb-ed05-4d56-a689-4ef044f4151a" />










