
#Preliminary Mechanical Design of a Simple Robotic Dog

##1. Body Shape and Chassis Design
A rectangular body with smooth, rounded edges was selected to simplify the chassis manufacturing process and reduce sharp edges in the design. The chassis will be made from 3D Printed Plastic because it is lightweight, inexpensive, and easy to manufacture and modify.
The battery is placed in the lower center of the robot body to keep the center of gravity low. Plastic supports are added above the battery to hold the Controller, keeping the main components close to the center of the body, which helps improve weight distribution.

##2. Leg Design
The robot has four identical legs. Each leg consists of two main parts: Thigh, Lower Leg.
The legs are designed symmetrically to help distribute the weight evenly and keep the center of mass close to the middle of the robot, improving stability while standing and walking.
The bottom of each foot is covered with Rubber to increase friction with the ground and reduce the possibility of slipping during movement.

##3. Joints and Degrees of Freedom
Each leg has two joints: the Hip Joint and the Knee Joint. Therefore, each leg has 2 Degrees of Freedom (2 DOF).
This number of joints was selected because the purpose of the design is to understand the basic mechanical principles required for the robot to stand and walk rather than to build an advanced robotic system. This design allows the leg to move forward and backward, bend at the knee, and lift the foot during walking.

##4. Motor Selection
Servo Motors were selected to drive the joints because they are easy to control (using an Arduino, for example), small, lightweight compared to some other motor types, inexpensive, and suitable for a simple robot design.
Two servo motors are used for each leg, with one motor controlling each joint, resulting in a total of 8 Servo Motors.

##5. Preliminary Knee Joint Torque Calculation
The Knee Joint was selected for the preliminary torque calculation.
Lower leg length: 4 cm
Weight of the moving parts around the knee joint:
	Lower leg: approximately 10 g
	Foot: approximately 5 g
	Mounting parts: approximately 10 g
Total moving weight:
10 + 5 + 10 = 25 g = 0.025 kg
Where:
m = 0.025 kg
g = 9.81 m/s²
r = 0.04 m
Torque = Force × Distance
τ= m × g × r
τ = 0.025  × 9.81  × 0.04
τ ≈ 0.0098 N.m
0.01 N.m ≈ 0.1 kg.cm
##6. Stability and Center of Gravity
The center of gravity is located near the middle of the robot body because of the symmetrical leg design and the placement of the main components, such as the battery and controller, near the center of the chassis.
The battery is also placed in the lower part of the body to lower the center of gravity, which improves the robot's stability and reduces the possibility of tipping over while standing and walking.

##7. Proposed Walking Method
The Crawl Gait was selected, where one leg moves at a time while the other three legs remain in contact with the ground.
This walking method was chosen because it: Increases the robot's stability and helps maintain its balance while walking, Is suitable for a simple robot design.

8. Expected Mechanical Problems
1) Foot Slippage: The robot's feet may slip on smooth surfaces during walking. This problem is reduced by adding a rubber layer under the feet to increase friction and improve stability.
2) Weight Imbalance: Uneven distribution of the components may shift the center of gravity and reduce the robot's balance. To minimize this problem, the battery and controller are placed approximately at the center of the chassis to achieve better weight distribution.
3) Structural Vibration: The movement of the motors may cause vibrations in the chassis, which could affect the robot's stability.
4) Insufficient Motor Torque: The motors may not be able to move the legs properly if the available torque is insufficient.
