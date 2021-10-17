# House_Service
## Aim : To build a bot that can deliver an object from one point to another in an environment. The bot can simulataneously localise itself and find its goal (drop-off location).
### Before starting:-
 1. Unzip the File in your desktop
 
 2. unzip map.pgm file in the same folder (worlds)

### Project Workflow :-

```├──                                # Official ROS packages
    |
    ├── slam_gmapping                  # gmapping_demo.launch file                   
    │   ├── gmapping
    │   ├── ...
    ├── turtlebot                      # keyboard_teleop.launch file
    │   ├── turtlebot_teleop
    │   ├── ...
    ├── turtlebot_interactions         # view_navigation.launch file      
    │   ├── turtlebot_rviz_launchers
    │   ├── ...
    ├── turtlebot_simulator            # turtlebot_world.launch file 
    │   ├── turtlebot_gazebo
    │   ├── ...
    ├──                                # Your packages and direcotries
    |
    ├── map                          # map files
    │   ├── ...
    ├── scripts                   # shell scripts files
    │   ├── ...
    ├──rvizConfig                      # rviz configuration files
    │   ├── ...
    ├──pick_objects                    # pick_objects C++ node
    │   ├── src/pick_objects.cpp
    │   ├── ...
    ├──add_markers                     # add_marker C++ node
    │   ├── src/add_markers.cpp
    │   ├── ...
    └──
 
```
### Pakages Used:
 1. Gmapping: With the gmapping_demo.launch file,one can easily perform SLAM and build a map of the environment with a robot equipped with laser range finder           sensors or RGB-D cameras.
 2. Turtlebot_teleop: With the keyboard_teleop.launch file, one manually control a robot using keyboard commands.
 3. Turtlebot_rviz_launchers: With the view_navigation.launch file, you can load a preconfigured rviz workspace. By launching this file, it will automatically load     the robot model, trajectories, and map for you.
 4. Turtlebot_gazebo: With the turtlebot_world.launch you can deploy a turtlebot in a gazebo environment by linking the world file to it.


## To run this project:
### 1. clone the repository
```
git clone https://github.com/Iaryan-21/House_Service.git
```
### 2. Unzip the file and unzip the map.pgm file in the worlds folder
### 3. install xterm
``` sudo apt-get install xterm```
### 4. run the commands
``` ./h_s.sh ```
The above command will run all the nodes together required for the project.
