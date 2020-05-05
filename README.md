# where-am-i

Use Adaptive Monte Carlo Localization (AMCL) to localize a mobile robot inside a map in the Gazebo Simulation environments

## How to 

- Clone to `~/catkin_ws/src`
- `cd ~/catkin_ws`
- `catkin_make`
- `source devel/setup.bash`
- `roslaunch my_robot world.launch`
- On a another terminal, `roslaunch my_robot amcl.launch`
- Optional, to use Teleop Package to control robot

```
cd ~/catkin_ws/src
git clone https://github.com/ros-teleop/teleop_twist_keyboard
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

Move the robot around to see how `amcl` quickly localize the robot position.

![Imgur](https://i.imgur.com/EWxN43R.png)

## Map setup

To generate the map from Gazebo simulation, I use Udacity's [pgm_map_creator](https://github.com/udacity/pgm_map_creator).
