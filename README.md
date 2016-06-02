## The Inflatable Robotic Arm (IRA) System
**Creators**: Andres Ulloa, Travis Emery, Shehan Jayasekera,  Timothy Kremers, and Lucas Prilenski
**Supervisors**: Dr. Kathleen Lamkin-Kennard, and Art North
**Sponsers**: Rochester Institute of Technology, Boeing

**insert gif of robot here**


### Repository Stucture
The IRA system is broken down into 4 subsystems.
 - [Controls/Software](#Controls/Software)
 - [Arm/Hand](#Arm/Hand)
 - [Air Flow](#Air Flow)
 - [Car](#Car)

All subsystems contain README.md files which contain instructions for building the subsystem.

### Subsystem Summaries and Evaluations
<a name="Controls/Software"/>
##### Controls/Software
 - Summary
 	- The control system is centered around the [Arduino Mega](https://www.arduino.cc/en/Main/arduinoBoardMega) microcontroller board,with control code written in Arduino c++, and a UI in the form of an [wireless Xbox 360 controller](http://www.xbox.com/en-US/xbox-360/accessories/controllers). We link the xbox controller to the arduino using the [Arduino USB Host Shield](https://www.arduino.cc/en/Main/ArduinoUSBHostShield) and [Microsoft Xbox 360 Wireless Receiver](http://www.amazon.com/Microsoft-Xbox-Wireless-Receiver-Windows/dp/B000HZFCT2).
 	- User--->Xbox Controller--->Wireless Reciever---->Usb Host Shield--->Arduino--->Subsytems

<a name="Arm/Hand"/>
##### Arm/Hand
The Arm/Hand system is the primary focus of the project.
 - Arm
 	- The arm and hand is made from by [4 channels molded into Smooth-on dragon skin compartments](http://www.instructables.com/id/Soft-Robots-Make-An-Artificial-Muscle-Arm-And-Gri/?ALLSTEPS). These compartments are adhered together and expand when air pressure is applied. Using a 4 channel system allows 3 dimensional control of the arm by the user.
 	 - ![arm before inflation](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/arm_before_inflation.jpg)
 	 - ![arm after inflation](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/arm_after_inflation1.jpg)
 - Hand
 	- The hand is created by attatching 3 [PneuNets Bending Actuators](http://softroboticstoolkit.com/book/pneunets-bending-actuator) to the hand base made of PMMA. The hand base is attatched to the end of the arm. Pressure is then fed into the actuator causing them to close. Small rubber bands are attatched to the actuators to allow retraction.
 	- ![fingers on arm](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/finger1.JPG)
 	- ![finger before inflation](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/finger_before_inflation.jpg)
 	- ![finger after inflation](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/finger_after_inflation.jpg)
<a name="Air Flow"/>
##### Air Flow
 - The air flow system starts with a compressor which pressurizes a 500mL tank. The tank then sends down regulated air pressure to a manifold where solonoid valves control entry into each channel and the fingers. Pressure is also downregulated to the fingers.
 	- ![flow loop](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/flowloop_img.jpg)

<a name="Car"/>
##### Car
 - A 2ft by 1.5ft frame holds by 4 wheels and 2 motors (rear wheel drive) 4in above the floor.
 	- ![mounted](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/mounted.JPG)
