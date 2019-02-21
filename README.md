# ROS-camera-callibration
To use camera in ROS enviroment, it require a calibration.yml file which basically tells the parameter of camera to ROS
This file look like something as -

/* camera calibration file for ros
image_width: 640
image_height: 480
camera_name: head_camera
camera_matrix:
  rows: 3
  cols: 3
  data: [634.1498901052836, 0, 357.4133903186774, 0, 634.1744827205051, 241.1570342122731, 0, 0, 1]
distortion_model: plumb_bob
distortion_coefficients:
  rows: 1
  cols: 5
  data: [0.06413781063425474, -0.1780036978914151, 0.001840731844165999, 0.003281693797725117, 0]
rectification_matrix:
  rows: 3
  cols: 3
  data: [1, 0, 0, 0, 1, 0, 0, 0, 1]
projection_matrix:
  rows: 3
  cols: 4
  data: [635.9409790039062, 0, 359.5976106785056, 0, 0, 638.7781982421875, 241.7553029854898, 0, 0, 0, 1, 0]
 */ 
    
So here is a step by step guide to calibrate USB camera, to remove Fish eye effect and to generate calibration.yml file for ROS.  
