##To run code it:
setup:
install node through nvm
sudo apt-get libgif-dev
install pip
upgrade pymongo to 3.3
install sound play (something like sudo apt-get install ros-indigo-sound-play )
copy hcrlab_map.yaml from turtlebot_code_it_launchers/ to home/turtlebot/


###On the turtlebot: (bringump minimal and navigation stack)
roslaunch roslaunch turtlebot_code_it_launchers turtlebot_navigation.launch 

### on your desktop: (Rviz viewer - makesure to setrobot)
roslaunch turtlebot_rviz_launchers view_navigation.launch 

### also on desktop: (teleop - make sure to setrobot)
roslaunch kobuki_keyop keyop.launch 

tbc
