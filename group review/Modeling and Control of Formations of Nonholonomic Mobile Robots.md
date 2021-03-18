@def review = true 
@def tags = ["reviews"] 
@def reviewers = ["Keith Russell, Samrat Patel"] 
@def hasmath = true 
@def class = "journal" 
@def authors = "Jaydev P. Desai; James P. Ostrowski; and Vijay Kumar;" 
@def title = "Modelling and Control of Formation of Nonholonomic Mobile Robots" 
@def venue = "IEEE" 
@def year = "2001"

\toc

\toc

### Broad Area Overview

This paper addresses the control of a team of nonholonomic mobile robots navigating in a terrain with obstacles while maintaining a desired formation and changing formations when required, using graph theory. 

### Specific Problem 
This paper describes a problem statement which is related to concurrent control and coordinations of multiple autonomous robots and develop a framework for transitioning from one formation to the other while following a certain trajectory and changing the shape of the formation in order to negotiate with the obstacle and reverting back to the original formation shape after passing by the obstacle.

### Solution

The team of swarm  is modeled as triple which can be identified by the group element ‘g’ , that describes the gross position of the lead robot , a shape variable ‘r’ and and control graph H that describes the behaviour of the robot in formation using a framework that enables the representation and enumeration of possible control graphs allowing coordination of transition between two different kinds of formation shapes or topologies. When viewed in this framework the problem can be broken down into three subproblems that is 
a)	Trajectory planning
b)	Robot Control and 
c)	Formation control
The concurrent planning of the actuator inputs increases the complexity exponentially with the number of the robots and obstacles and quickly become intractable which is solved here in this paper using robots having their own sensors and feedback controllers

Another related concept of the string stability has also been  addressed here and decentralized control law for shape variables and feedback controller  have been developed for the framework for each robot to maintain position and enable changes in the leader follower formation where states and position of the leader and follower which are represented relative to each other for example the position of the follower can be described by its relative position coordinates with respect to the leader and same rules apply to the leaders position wrt to the followers. There is a unique lead robot R1 designated that controls its followers in formation which is then followed by other leaders R2 R3 .. Rn which controls other follower robots using a control graph which is a digraph with each vertex having uniquely assigned integers which are based on certain constraints for lead robot where every lead robot on (vertex) has no incoming edge but has at least one outgoing edge. Every edge goes from lower vertex to higher vertex in the digraph and lastly the number of edges in the vertex is equal to the number of the output variable from the robots.



### Comments

Control graph algorithm was developed which was proved and tested for enumerating formation control and transition using Polya's Theorem. The non linear control theory strategies were implemented for 

Transition from one control graph to another control graph is modelled by a transition matrix which is the difference between the final and initial adjacency matrix . Appearance of -1 in the transition matrix denotes that the edges connecting the robots vertices needs to be broken and +1 means that edges need to be formed 

Simulation tested 3 robots and 6 robots  for transition of the formation from  triangle (Initial Control Graph)  a straight line (Final Control Graph) Rectangle shape . The formation change in sensory noise was measured. It was observed that even in the presence of sensory noise the formation converged to the desired shape and exhaustive list of desired shapes was proposed.

This paper does not take into consideration the routing and switching between the nodes which is another problem that needs to be studied as message passing between the nodes, especially the control data for formation, plays an important role for keeping the formation intact.


 ### Recent Articles 

●	Teruel, E., Aragues, R., & López-Nicolás, G. (2019). A distributed robot swarm control for dynamic region coverage. Robotics and Autonomous Systems, 119, 51-63

●	Xu, H., Li, S., Yu, D., Chen, C. P., & Li, T. (2021). Adaptive swarm control for high-order self-organized system with unknown heterogeneous nonlinear dynamics and unmeasured states. Neurocomputing, 440, 24-35.

●	Mohanty, P. K., & Dewang, H. S. (2021). A smart path planner for wheeled mobile robots using adaptive particle swarm optimization. Journal of the Brazilian Society of Mechanical Sciences and Engineering, 43(2), 1-18.

