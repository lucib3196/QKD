---
{"dg-publish":true,"permalink":"/02-notes/servo-motion-tracking-ar-uco-marker-implementation-senior-design/","tags":["project","notes/atomic"]}
---

Link: [[02Notes/QKD Resources\|QKD Resources]] 

To achieve precise motion tracking, pose estimation using ArUco markers was implemented to calculate the angular error between the camera frame and the marker's reference frame.

The pan angle error (horizontal misalignment) is computed as x= arctan(x/z), where x is the marker's horizontal displacement and z is the depth (distance from the camera). Similarly, the tilt angle error (vertical misalignment) is given by y= arctan(y/z), where y represents the vertical displacement. 

For implementation, our reference point is the center of the camera frame and we are tracking the center of the ArUco marker.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfyZG-_k4ex2t6jXOvuRoFUhT60s7wbjH41eb9a_DzZQCNK1IHCvZ4GM4dz8wKhykHL9bwohzT67-FRNEEGnAcfDMnvGjNHyF9cLQWtFP7abj4MLf4fK-8JeOZflyeZkw2VUbG0sw?key=fRN2bvpFrwoE7mFmuP50Us9k)  
  
## PID Controller
 
These calculated angles serve as the error inputs for a PID controller, which adjusts the servo motors to minimize the deviation and align the system. The controller continuously receives feedback from the camera, updating the servo position to correct the alignment dynamically. By tuning the proportional (P), integral (I), and derivative (D) gains, the system ensures smooth, stable, and responsive motion correction. This approach allows precise laser alignment with the mirror, even when direct tracking is unnecessary, as transformations can be computed based on known reference points.





----
# Source