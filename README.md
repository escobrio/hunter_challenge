# Robotic Systems Engineer Intern Coding Challenge 2025
This repo contains the code for a robotics internship application coding challenge.


The goals acheived by the applicant are:
- setup docker container with Ubuntu 22.04 and ROS2 Humble
- install and run the [Hunter](https://github.com/agilexrobotics/ugv_gazebo_sim/tree/humble/hunter_se) simulation
- Created the sevensense_pkg and ros node diff_to_ackermann.py to publish velocity commands (Differential Drive to Ackermann was not acheived)
- Video of the robot driving in a circle

# Thoughts regarding pure rotation
To perform pure rotation, the Instantaneous Center of Rotation (ICR) must lie in the middle of the rear axle and the front wheels have to be aligned perpendicular to the ICR.
As I'm didn't find out how exactly the Hunterbot is actuated, I assume the front wheels are for steering and the rear wheels are actuated, just like a car.
Therefore, a Differential Drive robot can acheive pure rotation by turning the front wheels accordingly and actuating one of the rear wheels to go forward and the other backward.
A Ackerman Drive robot can not  acheive pure rotation, as it always needs to drive forward to turn. 
