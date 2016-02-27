# SBMLT_Robotics
SBMLT working on robotics

## Purpose
This is git repository for Stony Brook Machine Learning Team's spcial group project. I will make this private repository if things are really get going and needs confidentiality. (As far as I know, they are participating [IGVC](http://www.igvc.org) which is actual competition with other schools.

##IGVC
The objective of the competition is to minimize the distance it uses to navigate through the map, hitting every waypoints, without crossing lines, avoiding obstacles, and come back to the start point.

###About robot
The robot has a lot of sensors, gyro, GPS, accelerometer, IMU sensors. But most importantly two cameras facing forward, 12cm apart from each other. They are using two of them to use computer vision related algorithm to create a bird view of the plane. 

###[Rules](http://www.igvc.org/2016IGVCRules.pdf)
The rule of the competition limits the amount of power the robot can use. However, he said we can assume unlimited power for now and later integrate it and come up with come solution.

### Reading
We will share reading related to the machine learning techniques that can help the robotics team.

### Goals
The things we should start doing:
* Edge Detection in color images to find white line "lanes"
* Sliding Windows to specify all pixels belonging to obstacles, and pixels belonging to background
* Maybe find some way to make the images robust against rotation

####Convolutionary Neural Network
#####[Alex Net](http://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)

### Lectures
[Convolutional Neural Network](https://youtu.be/n6hpQwq7Inw?list=PLNlv3xIQ7DATd3ARF_NtKUs2nzuH_mhWd)

### Papers
Okay, some of these papers are behind a paywall, as long as you are on a WolfieNet internet connection you should be able to access them without a problem. They will not all be relevant, in particular the SLAM has kind of already been implemented and the Image Patch Matching is part of SLAM, so it is not priority to study. Start with Contour and Texture segmentation if you want to try to do line detection, Efficient Sliding windows to try to do object recognition, or find better methods than the papers posted. Post more papers as you deem relevant.

* [ImageNet Classification with Deep Convolutional Neural Networks](http://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)
* [Simultaneous Localization and Mapping (SLAM) Introduction](http://ocw.mit.edu/courses/aeronautics-and-astronautics/16-412j-cognitive-robotics-spring-2005/projects/1aslam_blas_repo.pdf)
* [Robot Navigation by Machine Learning](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6419894&tag=1)
* [Contour and Texture Segmentation Introduction](http://www.cs.berkeley.edu/~malik/papers/MalikBLS.pdf)
* [Efficient Sliding Windows Object Localization](http://www.kyb.mpg.de/fileadmin/user_upload/files/publications/pdfs/pdf5070.pdf)
* [Image Patch Matching](https://www.cs.ubc.ca/~lowe/papers/ijcv04.pdf)

### Others

## Data to expect

>As far as the data collection, I have yet to plan exactly when it will happen, but I have an outline of what we plan to do. Since the software team is currently waiting for the mechanical build to complete, we will assemble a mock-up of the robot (scooter with devices attached) and take it up to the soccer field with a few obstacles. We will then perform a few runs through pre-planned routes and collect the sensor data (gps, gyro, camera) necessary to continue with software development and testing. We will also be sure to record ground-truth readings along with our sensor readings to give us an idea of the variance in our measurement noise. I will keep you posted as soon as I figure out when we can make it happen.

This is the reply from Anthony Musco (team learder of robotics software team).

He says he is mostly tied up with administrative works, so we have a great chance to specialize in analyzing data and giving feed back.

### Sample Dataset
There are some datasets of similar things we can begin to play with, especially to see how line detection/sliding windows work, since those should be pretty robust between datasets.

* [Park Video for Edge Detection](http://ilab.usc.edu/siagian/Research/data/PAMI07/PAMI07data.html)
* [Objects for Sliding Window](http://www.vision.caltech.edu/html-files/archive.html)
* [Maybe Data for Good Foreground/Background Learning](http://research.microsoft.com/en-us/projects/i2i/data.aspx)
* [Lots of textures to test Edge Detection](http://mosaic.utia.cas.cz/index.php?act=view_texs)

### GPS Data

### Gyro Data

### Camera Data (images & videos)

## Some possible keywords to start with
* Noise reduction
* Image processing
* Edge Detection
* Object Localization
