# Summary
The goal of this project is to design a path planner that is able to create smooth, safe paths for the car to follow along a 3 lane highway with traffic in the  [Udacity simulator](https://github.com/udacity/self-driving-car-sim/releases). The path planner generates trajectories that meets the following criteria:
* The car is able to drive without incident.
* The car doesn't drive faster than the speed limit. Also the car isn't driving much slower than speed limit unless obstructed by traffic
* The car does not exceed a total acceleration of 10 m/s^2 and a jerk of 10 m/s^3.
* The car does not have collisions.   
* The car stays in its lane, except for the time between changing lanes.
* The car is able to smoothly change lanes when it makes sense to do so, such as when behind a slower moving car and an adjacent lane is clear of other traffic.
   
#### Valid Trajectories
