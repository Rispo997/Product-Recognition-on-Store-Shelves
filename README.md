# Product-Recognition-on-Store-Shelves
![Alt text](https://i.imgur.com/h2mfnWM.png)

### What is this repository for? ###

* This repository implements two object detection algorithms based on SIFT 

### Package equirements ###

`Python version 3.9`    
`opencv-contrib version 4.4.0.44` 
`jupyter version 4.6`    
`numpy version 1.22.1`  


### Overview ###
 A project about object detection techniques based on computer vision.
 The algorithm can be deployed to identify query images contained inside a scene, the provided example shows an use case of product recognition on store shelves.
 In order to work properly, the algorithm needs two inputs:
 * A scene image, containing the query(ies) to be found.
 * A query image, the image to be recognised.

### Functioning ###
The project deploys two different algorithms in order to achieve object detection:

#### Mean-Shift clustering
![Alt text](https://i.imgur.com/6ubKSs1.gif)

This version uses mean-shift clustering to partition the detected keypoints into different clusters, then, for each cluster, matching is computed separately.
#### Generalized Hough Transform - Star Model
![Alt text](https://i.imgur.com/I34j2BE.gif)

This version uses GHT along with SIFT features, each matched keypoint casts a vote for where the barycenter is, then the resulting grid is thresholded to find objects.

### Who do I talk to? ###

* Luca Rispoli - luca.rispoli@studio.unibo.it
* Marco Ghaly - marcosafwat.ghaly@studio.unibo.it
