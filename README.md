[![PR](https://camo.githubusercontent.com/f96261621753dacf526590825b84f87ccb1db0e6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f5052732d77656c636f6d652d627269676874677265656e2e7376673f7374796c653d666c6174)](https://github.com/chinmaynehate/Venom/pulls)
[![Open Source Love png2](https://badges.frapsoft.com/os/v2/open-source.png?v=103)](https://github.com/chinmaynehate)
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

<a href="https://www.youtube.com/watch?v=NFO0sFC34yE&t=108s"><img src="https://i.imgur.com/M67nE8U.jpg" title="Venom" alt="Venom"></a>


# Venom : Sprawling-type Quadruped robot

> Venom is  a 12-DOF unmanned Quadruped(four legged robot) equipped with 12 Servo Actuators an ARM Processor for onboard computations.

> The Quadruped is based on Sprawling type motion with creep and trot gait successfully implemented on it.


[![Venom2](https://i.imgur.com/ZmYRAiz.jpg)]()

> This is a part of research project in Legged Mobility at Society of Robotics and Automation, VJTI.

- Most of the robots available in the industry make use of wheels for navigation. The goal is to build legged vehicle with multiple-terrain mobility  superior to existing wheeled and tracked vehicles.
- The system would be able to travel anywhere a person or animal  could  go using their legs while carrying its own fuel and payload. It would be smart enough to negotiate terrain with a minimum of human guidance and intervention



**Demo Video**

<a href ="https://www.youtube.com/watch?v=NFO0sFC34yE&t=108s"> VENOM- All terrain Quadruped</a>

---

## Table of Contents 

- [Installation](#Software-Installation)
- [Hardware Stack](#Hardware-Stack)
- [Team](#team)
- [FAQ](#faq)
- [License](#license)


---

## Creep GAIT Example

```python
venom = Quadruped(servoId) # Servo ID Array
venom.setParams(dirVector,FixedPoints)# Servo Direction and Set Points
venom.go2CreepStartPosition()
input("Press Enter") # Wait for user Input
# For CREEP GAIT
venom.walk(CREEP)
# For TROT GAIT
venom.walk(TROT)
```
---

## Software-Installation

- Requires Python 3.4+ installed on RaspberryPi (or Similar Development Board).

## Hardware-Stack

-  [Jetson Nano](https://www.nvidia.com/en-in/autonomous-machines/embedded-systems/jetson-nano/) (RasberryPi will work as well)
-  Servo Motors:  [ 12 Dynamixel AX-12A](https://www.trossenrobotics.com/dynamixel-ax-12-robot-actuator.aspx) or better / any Normal PWM Servo Motor (Torque > 20kgcm ). 
- Servo Motors(Alternate Servos): [Coreless Servo](https://robokits.co.in/motors/rc-servo-motors/ultra-torque-dual-shaft-metal-gear-35kgcm-coreless-servo-w-t-acc)
-  [PCA9685 16 Channel PWM Servo Driver](https://www.amazon.com/SunFounder-PCA9685-Channel-Arduino-Raspberry/dp/B014KTSMLA) for PWM Servo , [CM-530 Robotis Servo Controller
](https://www.trossenrobotics.com/p/cm-530-robotis-servo-controller.aspx) for Dyanmixel Servos.
- Acrylic Chasis (CAD Files Available)


### Clone

- Clone this repo to your local machine using `https://github.com/chinmaynehate/Venom.git`

### Setup

> Install dependencies

```shell
$ python3 -m pip install numpy adafruit_servokit busio sympy 
```



## License


- **[MIT license](http://opensource.org/licenses/mit-license.php)**
