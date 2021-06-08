# Landmark-Detection-and-Robot-Tracking-SLAM-
Simulataneous Localization & Mapping(SLAM) is an active area of research in the field of autonomous systems & robotics. In this project, a map of an environment is created from sensor and motion data gathered by a robot over time and SLAM was implemented for a 2D world. This is my solution to Udacity's Landmark Detection & Tracking Project which is a requirement to complete the Computer Vision Nano degree.

# Overview
Combining knowledge of robot sensor measurements and movement to create a map of an environment from only sensor and motion data gathered by a robot, over time. SLAM (Simultaneous Localization and Mapping) provides a way to track the location of a robot in the world in real-time and identify the locations of landmarks such as buildings, trees, rocks, and other world features.
Below is an example of a 2D robot world with landmarks (purple X's) and the robot (a red 'O') located and found using only sensor and motion data collected by that robot.

![image](https://user-images.githubusercontent.com/59326134/121113734-30015d00-c81b-11eb-8b29-f02d158eaba5.png)

# Files

moving_and_sensing.ipynb : Define and visualize the world (environment)
Omega_and_Xi : Constraints and solving (linear algebra)
Landmark_Detection_and_Tracking : SLAM implementation
robot_class.py : Robot class definition

#**Key concepts to accommodate or use:**

# Uncertainty

Robot motion and sensors have some uncertainty associated with them. For example, imagine a car driving up hill and down hill; the speedometer reading will likely overestimate the speed of the car going up hill and underestimate the speed of the car going down hill because it cannot perfectly account for gravity and other factors. Similarly, we cannot perfectly predict the motion of a robot. A robot is likely to slightly overshoot or undershoot a target location.
To perform SLAM, we'll collect a series of robot sensor measurements and motions (with some noise; accounting for uncertainty and unaccounted behaviour), in that order, over a defined period of time. Then we'll use only this data to re-construct the map of the world with the robot and landmark locations.

# Omega, Xi and constraints

Matrix representation of Omega and Xi respectively:

![image](https://user-images.githubusercontent.com/59326134/121113942-94bcb780-c81b-11eb-959d-dffe58c915d7.png)

Poses as constraints filled in the matrix (example):

![image](https://user-images.githubusercontent.com/59326134/121113971-a2723d00-c81b-11eb-8287-454f187692bf.png)

# Instructions to run

1. Type git clone (https://github.com/MariaSimon-AI/Landmark-Detection-and-Robot-Tracking-SLAM-.git)[https://github.com/MariaSimon-AI/Landmark-Detection-and-Robot-Tracking-SLAM-.git] in your Git bash (Terminal)
2. Open terminal and type: jupyter notebook (make sure you've already installed jupyter notebook)
3. Navigate to the 'Landmark-Detection-and-Robot-Tracking' folder and browse through the notebooks/files.


