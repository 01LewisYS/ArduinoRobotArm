# Arduino Robot Arm (Mark I & Mark II)
## Table of Contents
* [Gerenal Info](#general-info)
* [FAQ](#faq)
* [Important Notice](#important-notice)

## General Info
Robot Arm (Mark I): 
* Function: Picks up a 100N object at a location, and dropping it off the object at the _same_ location.
* Video: [Arduino 4DOF Robot Arm (Mark I): Picking Up & Dropping Off 100N Load](https://www.youtube.com/watch?v=N_4QJMrR-Z4)

Robot Arm (Mark II):
* Function: Picks up a 100N object at a location, but drops off the object at a _different_ location by rotating itself to a different direction for drop off.
* Video: [Arduino 4DOF Robot Arm (Mark II): Picking Up & Dropping Off 100N Load](https://www.youtube.com/watch?v=Gq96fXNVIpc)

Micro Servos & Functions:
1) Left servo (servoL) controls the height of clamp from the ground. 
2) Right servo (servoR) controls the horizontal retraction and extension of the robot arm.
3) Base servo (servoB) controls the rotation of the entire robot arm, so that the gripper/clamp can face any direction.
4) Clamp servo (servoC) of robot arm controls the opening and closing of clamp. 

## FAQ
1) Which one is the "Left servo"? Which one is the "Right servo"?

Answer: Firstly, look at your computer screen. Now, position the robot arm so that the robot arm's clamp/gripper also faces the computer screen. Now look at your robot arm, the leftmost servo is the Left servo, and the rightmost servo is the Right servo.

2) Which one is the "Base Servo"?

Answer: Base servo is the servo that's between the left & right servos (other than the clamp's servo).

## Important Notice
This program will only work properly if:
  1) The robot arm was built using this instruction manual guide: https://static.rapidonline.com/pdf/75-0040_v1.pdf
  2) All micro servos were calibrated as such before/during the construction of your Robot Arm:
  ```
  servoB.write(90);
  servoL.write(90);
  servoR.write(90);
  servoC.write(25);
  ```
