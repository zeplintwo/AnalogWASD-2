# Analog_WASD
**---------- WIP ----------**
  
  TARGET scripting software to PWM HOTAS inputs into Duty Cycle timed keypresses.
  
**---------- WIP ----------**

This is the first public release of a PWM keypress system for a joystick axis of rotation. 

The idea was that I wanted a block of time (currently at 100ms can be change in script) to represent the range of motion from center to the max value of an axis. With a minimum buffer of a keypress to make sure that all input is properly executed (current set a 25ms can be change in script). 
This was not a simple task as I have been though no less than 5 code designs. And this current design while works I am not totally satisfied with it is build. 
I only have the conversion working for a single stick on the Thrustmaster Warthog HOTAS. 

**WIP**

*But have built in the ability to use the T16000.m Dual sticks (NO TESTING OF T1600.M HAS BEEN DONE). *

I am posting for the simple reason I am looking to show the code to get help with some questions that I have not been able to answer from my limited programing knowledge. But, with the limited C++ Code base that TARGET has not sure if these ideas will work. 

** Limitations Found **
The devices must have constant input from devices to trigger PWM. Working on finding some way to integrate a timed latch where every ~150ms it will pole for states. 
