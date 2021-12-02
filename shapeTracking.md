##### Time Encoded Imaging [PDF](../paper/DVS/shapeTracking.pdf)
_biomimetic event-based cameras_

* Over the past fewer years
1. temporal contrast vision sensors
2. gradient-based sensors
3. edge-orientation sensitive devices
4. optical flow sensor

*In this paper : asynchronous time image sensor (ATIS) --> a time-domain encodeing vision sensor -->304 x 240 pixel resolution*

The individual pixel --> sparse encoding

* Methods
1. Gaussian Blob Trackers
      1.  [x, y, t, pol]  plo is its polarity (-1 or 1)
      2. assumes that these event are normally distributed, the event cloud approximates a bivariate Gaussian distribution
      3. The probability of it belonging to the *i*  th Gaussian tracker $B^i$, and the event will be assigned to the tracker with the highest Gaussian probability
2. Spring-linked Feature Tracker
      1. A more complex object can be assumed that it is composed of simple shapes linked by geometric relation
      2. Euclidean Configuration: *Hooke's law*. the energy dissipation mechanism is represented by an ideal damper(阻尼器). Then applying *Newton's sencond law*
          1. assume this connection behave as a single linear spring: only take into account the Euclidean distance between the trackers
      3. Torsional Configuration: imaging the trackers as being linked by torsion springs.
          1. first-order approximation
      4. Cartesian Configuration: to keep both the **distance** and the **angle**.
3. Using the Energy as a Matching Criterion
      1. the elastic energy is a measure of the deformation of a connection--tracking the desired object, the energy of all of the connections remains stable
      2. Preventing a Single Tracker from Following the Wrong Cloud of Event
      3. Preventing a Group of Trackers From Following the Wrong Cloud of Event 
4. Remark
      1. different stiffnesses



![image](https://github.com/shaobo007/myNotes/shapeTracking_1.jpg = 600x400)
