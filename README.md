# Zeplins Analog WASD add Thrusmaster TARGET to your game.
  
  TARGET scripting software to PWM HOTAS inputs into Duty Cycle timed keypresses.

This is the first public release of a PWM keypress system for a joystick axis of rotation. 

The idea was that I wanted a block of time (currently at 100ms can be change in script) to represent the range of motion from center to the max value of an axis. With a minimum buffer of a keypress to make sure that all input is properly executed (current set a 25ms can be change in script). 
This was not a simple task as I have been though no less than 5 code designs. This is a very close to finished script base. The basic functions all work and polling  for values and PWM cycles work on 100ms as default you can increase or decrese it but it can cause issues. As most games and/or windows discard any keypress less than 10-25ms.

## **WIP**

* ~~I have built in the ability to use the T16000.m Dual sticks (NO TESTING OF T1600.M HAS BEEN DONE YET).~~
* Build a default keymap for flight controls. 
* Build referance PDF's for flight control functions.
* TM T.Flight Rudder Pedals (TFRP) - in Flight Mode
* Planned features:
	1. Switchable throttle maps
	2. Switchable Joystick maps
	3. ~~Internal comm switch and external coms switch or both toggle with visual.~~
	4. Posable TrackIR/FaceTrack controls
	6. Posable VoiceCommand intgrations
	5. More to come as Starbase comes out

This system was designed with flight in mind for Starbase. But this system can be addapted to almost any game. Some functions will take more 'magic' to intergrate but TARGET has a high degree of coustamizablity. As this script can attribute to.

---

## Hardware
### Required hardware:  
Thrustmaster (TM) Warthog HOTAS – Throttle and Joystick

or

ThrustMaster (TM) T.16000M FCS Space Sim Duo

### Could work but I don't have to do the testing on the hardware:

ThrustMaster (TM) T.16000M FCM Flight Pack

TWCS Throttle

TPR Rudder

TCA Officer Pack Airbus Edition and its throttles or single stick

---


## Thrustmaster links to TARGET Software

* Thrustmaster US website: http://www.thrustmaster.com/en_US
* Thrustmaster US support: http://www.thrustmaster.com/en_US/support
* Thrustmaster US Warthog HOTAS downloads: https://support.thrustmaster.com/en/product/hotaswarthog-en/\
* Thrustmaster US FTRP downloads: https://support.thrustmaster.com/en/product/tfrp-en/  
* Target software found in download link above under software as of this writing on July 18, 2021 the file name was T.A.R.G.E.T.-Software v3.0.18.328 . There is no direct link I can give. The version number will change in the future.

---
## Installation:

   1. Download and extract the latest ‘source’ files. [Releases](https://github.com/zeplintwo/AnalogWASD-2/releases)
   2. Unpack zip and keep all files in same directory. 
   3. Open ‘TARGET Script Editor’ Open and Compile ‘Analog_WSAD_Profile.tmc'.
   4. Edit 'Analog_WSAD_User_Settings.ttm' save changes if any.
   5. Close ‘TARGET Script Editor’ window.
   6. Launch ‘TARGET GUI’ and ‘Run Configuration’ on 'Analog_WSAD_Profile.tmc'. 
      - You can also run the configuration from the Script Editor.
   7. The following binds are built in but can be changed in the Analog_WSAD_Keymapings.ttm
        1. ThrottleUp       USB[0x57]   //numpad + throttle step up
        2. AltThrottleUp    USB[0x55]   //numpad * alternate throttle step up
        3. ThrottleDown     USB[0x56]   //numpad - throttle step down
        4. AltThrottleDown  USB[0x54]   //numpad / alternate throttle step down
        5. TrimInc          USB[0x59]   //numpad 1 trim increase step up
        6. TrimDecr         USB[0x5A]   //numpad 2 trim decrease step down
        7. PitchDown        USB[0x16]   //s pitch down, nose down
        8. PitchUp          USB[0x1A]   //w pitch up, nose up
        9. RollRight        USB[0x07]   //d roll right, roll clockwise
        10. RollLeft         USB[0x04]   //a roll left, roll anti-clockwise
        11. YawRight         USB[0x08]   //e yaw right, nose right
        12. YawLeft          USB[0x14]   //q yaw left, nose left
        13. ThrustUp         USB[0x52]   //up arrow translate, accend, stafe thrust 
        14. ThrustDown       USB[0x51]   //down arrow translate, decend, thrust down
        15. ThrustRight      USB[0x4F]   //right arrow translate, strafe,thrust right
        16. ThrustLeft       USB[0x50]   //left arrow translate, strafe,thrust left
   9. Launch save game and enjoy. 
