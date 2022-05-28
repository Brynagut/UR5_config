# UR5_config
Configuration of UR5 robot arm


you need 

git clone -b <distro>-devel https://github.com/ros-industrial/universal_robot.git
  

git clone https://github.com/filesmuggler/robotiq.git

and 
  
~/catkin_ws/src/universal_robot/ur_description/urdf$ wget https://raw.githubusercontent.com/utecrobotics/ur5/master/ur5_description/urdf/ur5_robotiq85_gripper.urdf.xacro

in your workspace
  
change line 9 and 14 in
  
robotiq_description/urdf/robotiq_85_gripper.transmission.xacro
  
to
  
<hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
