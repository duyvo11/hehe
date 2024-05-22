<!-- 

     .********
 Lau dia chi ros
 cd catkinv2_ws
 source ~/catkinv2_ws/devel/setup.bash
.          *******************************
 chay mo phong emtry world: roslaunch ros_mobile_robot drive_robot.launch
 chay mo phong house world: roslaunch ros_mobile_robot house_world.launch
 Chay slam gmaping: roslaunch ros_mobile_robot gmapping.launch
 chay slam hector: roslaunch hector_mapping mapping_default.launch 

 chay nav: roslaunch ros_mobile_robot amcl.launch
.          *******************************
 dieu khien robot bang gui: rosrun rqt_robot_steering rqt_robot_steering
 dieu khien robot bang nut nhan: rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=robot_diff_drive_controller/cmd_vel
 Luu map: rosrun map_server map_saver -f ~/map
 Create package: catkin_create_pkg gui_mobile std_msgs rospy 

  lenh pub vi tri den
 rostopic pub /move_base_simple/goal geometry_msgs/PoseStamped '{header: {stamp: now, frame_id: "map"}, pose: {position: {x: 3, y: 3.0, z: 0.0}, orientation: {w: 3.0}}}'
    
rospack plugins --attrib=plugin nav_core

-->

