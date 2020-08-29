# pid_tank_level_control_2
PID tank level control source code and other files


Installation and Configuration
1. Download the Arduino IDE and Install - https://www.arduino.cc/en/main/software

2. Download and Install Proteus software - https://crackdaily.com/proteus-download/

3. Extract the Zip folder PID

4. After Installing the Arduino IDE need to install the library for the PID
	1. Got the PID folder and then open the Arduino Library folder copy the Arduino-PID-Library-master
	2. Go to the Document folder of your computer, open the arduino folder and then open library folder.
	3. Past the copied folder (Arduino-PID-Library-master)

5. Need to config the library files for arduino and ultrasonic sensor in proteus software
	1. Open the source location of the proteus software installed in your computer
	   in my case (C:\Program Files (x86)\Labcenter Electronics\Proteus 8 Professional\Library)
	2. Then open the Library folder in proteus software installed location 
	3. Before that copy the two file inside the --> PID/Proteus_library/Arduino/
	4. Past that copied files in the location mentioned in 1st point
	5. Follow the same procedure for one more (ultrasonic) folders in location mentioned in 2nd Point.

6. Basic installation and Library configs all are completed

7. Open the arduino source code from PID/Arduino Program/pid_tank_level_1/pid_tannl_level.ino

8. Go to File->Perferences and checkIn compilation option, then click ok.

9. Then Click the Run button, Sketch->Verify/Complie or Ctrl+R or click the tick button on the top left corner below the file option.


10. Remaining procedures, please follow up the connection video - https://drive.google.com/file/d/1X6kjz4Gw5r7aeIpVbohMmJM0Z46KTpYr/view?usp=sharing
      Demo video - https://drive.google.com/file/d/1cJdIa9PXhykPHhrT60z29FlJD4V3QF_M/view?usp=sharing


Pin Connection:
	Components used:-
		1.  Arduino UNO - 1 
		2.  LM35 (Temperature Sensor) - 3
		3.  HC-SR04 (Ultrasonic Sensor) - 2
		4.  Push Button - 1
		5.  GSM (for Simulation purpose we are using virtual terminal) -1
		6. Resistor

	Connections:
		1.  LM35 sensor 1:
			LM35 Vcc        -   Arduino 5V
			LM35 Gnd       -   Arduino Gnd
			LM35 Out Pin  -  Arduino A1

		2.  LM35 sensor 2:
			LM35 Vcc        -   Arduino 5V
			LM35 Gnd       -   Arduino Gnd
			LM35 Out Pin  -  Arduino A2	

		3.  LM35 sensor 1:
			LM35 Vcc        -   Arduino 5V
			LM35 Gnd       -   Arduino Gnd
			LM35 Out Pin  -  Arduino A3

		5.  Ultrasonic Sensor 1 (Sub-tank):
			Sensor Vcc     	-  Arduino 5V
			Sensor Gnd     	-  Arduino Gnd
			Sensor Triger Pin    	-  Arduino 9th Pin
			Sensor Echo Pin      	-  Arduino 10th Pin

		6.  Ultrasonic Sensor 2 (Main-tank):
			Sensor Vcc     	-  Arduino 5V
			Sensor Gnd     	-  Arduino Gnd
			Sensor Triger Pin    	-  Arduino 11th Pin
			Sensor Echo Pin      	-  Arduino 12th Pin
		
		7.  GSM (Virtual Terminal):-
			GSM Vcc		-  5Watt Power Supply
			GSM Gnd		-  Power Supply Gnd (Arduino Gnd and Power Supply Gnd Should be short)
			GSM Tx		-  Arduino Rx Pin (0th Pin)
			GSM Rx		-  Arduino Tx Pin (1st Pin)
