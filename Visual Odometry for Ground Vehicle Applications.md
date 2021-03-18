
@def review = true
@def tags = ["reviews","learning","control","analysis","optimization"]
@def reviewers = ["Hasan Poonawala","reviewer no. 2","reviewer no. 3"]
@def hasmath = true
@def class = "journal"
@def authors = "Poonawala, H.A.; Lauffer, N.;Topcu, U.;"
@def title = "Training Classifiers For Feedback Control With Safety In Mind"
@def venue = "Automatica"
@def year = "2021"

\toc


# Visual Odometry for Ground Based Vehicle Applications
* Authors: David Nister, Oleg Naroditsky, James Bergen
* Venue: Wiley
* Year: 2005
* Reviewed By: Keith Russell



### Broad area/overview
This paper details a vision-based motion estimation system, using either a single or stereo camera.  Their system works in real time and is able to accurately track the motion of the camera relative to baseline GPS data.

### Specific Problem
Computer vision has been a very popular research topic in the past few decades due to the enormous variety and usefulness of its real-world implementations.  This paper seeks to develop a robust and streamlined method of motion tracking based solely on visual data, either from a single or stereo camera pair.  Their model, unlike others before it, does not require any knowledge of the robot's prior motion, instead relying only on what data is available immediately from the cameras.

### Solution Ideas
* Their solution uses Harris corner detection in every image frame, which is a method of detecting corners using computer vision developed in 1988 [1].  
* Once features are detected using the Harris corner detection, they are matched to features in the next frame using normalized correlation.
* Once features are matched, they are tracked and triangulated into 3D points, from which the pose of the camera is computed using its relative position to those points.
* The stereo camera scheme is similar but requires matching of features between the stereo camera image pairs.

### Comments
* The model shown in this paper was able to accurately track the position of the camera for hundreds of meters using nothing but raw image data.  This is incredibly impressive, even for 2021.
* This paper not only demonstrates a very accurate system, but a robust one, that rejects noise and requires very little input to achieve its goal.
* While image data alone may not be the best way to localize/navigate a vehicle, the estimate given by image data is certainly a good supplement to highly utilized technology like GPS and can provide a very good alternative in cases where GPS may not be available.

### Citations

[1] https://docs.opencv.org/master/dc/d0d/tutorial_py_features_harris.html
