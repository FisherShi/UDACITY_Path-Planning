# Summary
The goal of this project is to design a path planner that is able to create smooth, safe paths for the car to follow along a 3 lane highway with traffic in the  [Udacity simulator](https://github.com/udacity/self-driving-car-sim/releases). The path planner generates trajectories that meets the following criteria:
* The car is able to drive without incident.
* The car doesn't drive faster than the speed limit. Also the car isn't driving much slower than speed limit unless obstructed by traffic
* The car does not exceed a total acceleration of 10 m/s^2 and a jerk of 10 m/s^3.
* The car does not have collisions.   
* The car stays in its lane, except for the time between changing lanes.
* The car is able to smoothly change lanes when it makes sense to do so, such as when behind a slower moving car and an adjacent lane is clear of other traffic.
   
## Check if the car in front is too close
The car keeps driving at speed limit (50 mph) until the car in front is too close. For how does the path planner determines if the car in front is too close, see row 246 to row 269 of the code in main.cpp for details. 

## Check if it is safe to change lane
If the car in front is too close, the planner needs to check if it is safe to switch lane. For how does the path planner determines if it is safe to switch lane, see row 273 to row 316 of the code in main.cpp for details. 

## Generate trajectory
I used [splin tool](http://kluge.in-chemnitz.de/opensource/spline/) to generate trajectory. For how the trajectory is generated, see row 337 to row 444 of the code in main.cpp for details. 
 