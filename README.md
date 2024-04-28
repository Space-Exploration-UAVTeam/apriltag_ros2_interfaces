

# apriltag_ros2_interfaces for other packages which need it
mkdir -p ~/ros2_ws/src             
cd ~/ros2_ws/src                  
git clone https://github.com/Space-Exploration-UAVTeam/apriltag_ros2_interfaces.git  
cd ~/ros2_ws                       
rosdep install --from-paths src --ignore-src -r -y  
colcon build   
source /opt/ros/Galactic/setup.bash 
source /[your home directory]/apriltag_ws/install/setup.bash 
