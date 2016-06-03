## The Inflatable Robotic Arm (IRA) System
 - **Creators**: Andres Ulloa, Travis Emery, Shehan Jayasekera,  Timothy Kremers, and Lucas Prilenski
 - **Supervisors**: Dr. Kathleen Lamkin-Kennard, and Art North
 - **Sponsors**: Rochester Institute of Technology, Boeing

![Demo CountPages alpha](https://github.com/aulloa/inflatable_robotic_arm/raw/master/photo_gallery/output.gif)

### Alyssa insert plain words description of the robot underneath
The IRA is a inflatable soft robotic arm which is mobile

### Repository Structure
The IRA system is broken down into 4 subsystems:
 - [Controls/Software](#Controls/Software)
 - [Arm/Hand](#Arm/Hand)
 - [Air Flow](#Air Flow)
 - [Car](#Car)

All subsystems contain README.md files which contain instructions for building the subsystem.

### Subsystem Summaries
<a name="Controls/Software"/>
##### Controls/Software
 -  The control system is centered around the [Arduino Mega](https://www.arduino.cc/en/Main/arduinoBoardMega) microcontroller board, with control code written in Arduino c++, and a UI in the form of a [wireless Xbox 360 controller](http://www.xbox.com/en-US/xbox-360/accessories/controllers). We link the Xbox controller to the arduino using the [Arduino USB Host Shield](https://www.arduino.cc/en/Main/ArduinoUSBHostShield) and [Microsoft Xbox 360 Wireless Receiver](http://www.amazon.com/Microsoft-Xbox-Wireless-Receiver-Windows/dp/B000HZFCT2).
 - User--->Xbox Controller--->Wireless Receiver---->Usb Host Shield--->Arduino--->Subsystems

<a name="Arm/Hand"/>
##### Arm/Hand
The Arm/Hand system is the primary focus of the project.
 - Arm
 	- The arm and hand is made of [4 channels molded into 13 layers using Smooth-on Dragon Skin](http://www.instructables.com/id/Soft-Robots-Make-An-Artificial-Muscle-Arm-And-Gri/?ALLSTEPS). These compartments are adhered together and expand when air pressure is applied. Using a 4 channel system allows for 3-dimensional control of the arm by the user.
<p>
<img src = "https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/arm_before_inflation.jpg" style="float:left;" alt="" /><img src = "https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/arm_after_inflation1.jpg" style="float:right;" alt="" /> 
</p>

 - Hand
 	- The hand is created by attaching 3 [PneuNets Bending Actuators](http://softroboticstoolkit.com/book/pneunets-bending-actuator) to the PlexiGlass hand base which is attached to the end of the arm. Pressure is then fed into the actuators causing them to close. Small rubber bands are attatched to the actuators to allow retraction.
<p>
<img src = "https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/finger_after_inflation.jpg" style="float:left;" alt="" /><img src = "https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/finger_before_inflation.jpg" style="float:right;" alt="" /> 
<break>
<img src = "https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/finger1.JPG" width="600" alt="" /> 
</p>

<a name="Air Flow"/>
##### Air Flow
 - The air flow system starts with a compressor which pressurizes a 500mL tank. The tank then sends downregulated air pressure to a manifold where solonoid valves control entry into each channel and the fingers. Pressure is also downregulated to the fingers.
 ![flow loop](https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/flowloop_img.jpg)

<a name="Car"/>
##### Car
 - A 2ft x 1.5ft frame holds 4 wheels and 2 motors 4in above the floor.
 - **The steering system for the car did not work very well, a redesign is recommended.**
 <img src = "https://raw.githubusercontent.com/aulloa/inflatable_robotic_arm/master/photo_gallery/mounted.JPG" width="600"/>
