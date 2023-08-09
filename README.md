# Robotic-System-Science-Project


# Objective

Heriot Watt University robotic assessment.
A turtlebot made to SLAM in a maze while mapping specific symbols in space.
The turtlebot navigation is based on frontier exploration, setting the furthest free explored spot (with potential free unexplored space) as objective.
When the RGB camera pick a familiar object its position is calculated and reported in the rviz-map as a pin symbolising the recognised image.
The objects are recognised using the [find_object_2d](http://wiki.ros.org/find_object_2d) Ros package. 

## List of Task

- [x] Frontier exploration
- [x] Object Recognition 

## List of images to recognise

<div style="text-align:center">
<p align="center">
<img src="https://github.com/my-name-is-D/HW-Robotic-System-Science-Project/blob/master/images/symbol_clean.png " width="300" >
</p>
</div>

## How to use the package

Package for the project: "rss_project"
To use it:
  1. Copy the rss_project folder in your catkin workspace
  2. In a terminal: roscd; cd ..;
  3. catkin_make --only-pkg-with-deps rss_project
  4. add permission to all the py files, using "chmod +x [file.py]" command
 
 
 image processing :
 
 roslaunch marker_map launch.launch
    load the rightful data set on find 2d object
    click on "update object"
    add the Visual MArker in Rviz


## Dependencies

This list is expected to be uncomplete, but you must have at minima:
* a functioning turtlebot 
* a lidar 
* a RGB camera
* ROS melodic (expected to work on ROS noetic as well)
* python3
