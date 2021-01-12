## Landmark Detection & Robot Tracking (SLAM)
# Description
In this project, SLAM (Simultaneous Localization and Mapping) algorithm is implented for a 2 dimensional world. We combine robot sensor measurements and movement to create a map of an environment from only sensor and motion data gathered by a robot, over time.

SLAM gives a way to track the location of a robot in the world in real-time and identify the locations of landmarks such as buildings, trees, rocks, and other world features.

# Files
Robot Moving and Sensing.ipynb : Robot moving and sensing  
Omega and Xi, Constraints.ipynb : Omega and Xi, Constraints  
Landmark Detection and Tracking.ipynb : Landmark detection and tracking  
robot_class.py : Robot object with its world  
helpers.py : helper functions

# Graph SLAM
To implement Graph SLAM, a matrix and a vector (omega and xi, respectively) are introduced. The matrix is square and labelled with all the robot poses (xi) and all the landmarks (Li).

Every time an observation is made, for example as we move between two poses by some distance dx, it can relate those two positions, and can be represented as a numerical relationship in these matrices.

Here, I am referring to robot poses as Px, Py and landmark positions as Lx, Ly, and one way to approach this challenge is to add both x and y locations in the constraint matrices.
