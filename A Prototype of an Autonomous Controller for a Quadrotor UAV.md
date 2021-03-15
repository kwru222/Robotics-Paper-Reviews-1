# A Prototype of an Autonomous Controller for a Quadrotor UAV
* Authors: Ian D. Cowling, Oleg A. Yakimenko, James F. Whidborne, and Alastair K. Cooke
* Venue: IEEE
* Year: 2007
* Reviewed By: Keith Russell

### Broad area/overview
This paper is concerned with autonomy of quadrotor UAVs.  Specifically, the task of creating a controller which can incorporates both trajectory planning and path following.  

### Specific Problem
With the cost of lithium ion batteries being cheaper than ever before, as well as incresingly efficient, small unmanned aircraft such as quadrotor UAVs have become very popular consumer and industrial technology.  The main goal of this paper is to introduce a prototypical method of autonomous control for UAVs.

### Solution Ideas
* The property of differential flatness is used to simplify the problem of trajectory generation.
* The path following portion of the controller uses a standard linear multi-variable control technique.
* A quasi-optimal path planning is used so that the path can be generated in real time for robustness.  This takes into account possible changing of desired location or if discrepensies between desired and current location become too large.
* The controller is optimized by using the property of differential flatness to repose the problem in terms of the output space (ie, the spatial coordinates as opposed to the controls), which allows for optimization based on obstacle avoidance.
* The cost function of the controller is expressed in terms of total flight time and total distance travelled.
* The controller was simulated in several trajectory scenarios including moving in a straight line upwards, as well as reaching a desired coordinate while avoiding a pre-defined spherical obstacle.
* Wind and added error were factored into the controller to test for robustness and disturbance rejjection as well.

### Comments
* This paper demonstrated a very thorough design process for creating an autonomous controller.
* While the constraints and trajectories imlemented in the paper are quite simple, this paper manages to create a very good working model from which more complicated obstacle and vehicle avoidance can be added in.


