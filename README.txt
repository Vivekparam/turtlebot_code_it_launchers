## To run code it:
setup:
install node through nvm
sudo apt-get libgif-dev
install pip
upgrade pymongo to 3.3
install sound play (something like sudo apt-get install ros-indigo-sound-play )
copy hcrlab_map.yaml from turtlebot_code_it_launchers/ to home/turtlebot/

### On Turtlebot: 
roscore

### On the turtlebot: (bringump minimal and navigation stack)
roslaunch roslaunch turtlebot_code_it_launchers turtlebot_navigation.launch 

### On your desktop: (Rviz viewer - makesure to setrobot)
roslaunch turtlebot_rviz_launchers view_navigation.launch 

### Also on desktop: (teleop - make sure to setrobot)
roslaunch kobuki_keyop keyop.launch 

### on Turtlebot: (code_it backend)
roslaunch turtlebot_code_it_launchers code_it_backend.launch

### On Turtlebot: (sound play)
rosrun sound_play soundplay_node.py 

### On Turtlebot:(blinky)
roscd blinky/frontend; gulp serve; // will serve on :5001

### On Turtlebot: (code_it site)
roscd code_it/frontend; gulp; cd ../www; python -m SimpleHTTPServer 5000; // will serve on port 5000
