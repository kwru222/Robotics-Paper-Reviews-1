# Visual Odometry for Ground Based Vehicle Applications
* Authors: David Nister, Oleg Naroditsky, James Bergen
* Venue: Wiley
* Year: 2005
* Reviewed By: Keith Russell

### Broad area/overview
This paper details a vision based motion estimation system, using either a single or stereo camera.  Their system works in real time and is able to accurately track the motion of the camera relative to baseline GPS data.

### Notation
* $x$: ...

### Specific Problem
Computer vision has been a very popular research topic in the past few decades due to the enormous variety and usefulness of its real world implementations.  This paper seeks to develop a robust and streamlined method of motion tracking based solely on visual data, either from a single or stereo camrea pair.  Their model, unlike others before it, does not require any knowledge of the robot's prior motion, instead relying only on what data is available immediately from the cameras.

### Solution Ideas
* Their solution uses Harris corner detection in every image frame, which is a method of detecting corners using computer vision developed in 1988 [1].  
* Once features are detetced using the Harris corner detection, they are matched to features in the next frame within a certain disparity limit, which changes depending on smoothness of input.
* 

### Comments
* The paper focuses on ...

### Recent Papers
**Note**...

### Citations

[1] https://docs.opencv.org/master/dc/d0d/tutorial_py_features_harris.html


