# MoveIt1 - Noetic Installation steps on Ubuntu 20.04

1. Follow instructions in [moveit_tutorials](https://ros-planning.github.io/moveit_tutorials/doc/getting_started/getting_started.html#install-ros-and-catkin).

2. In case of timeout in first step: `rosdep init/update`, refer to [this website](https://www.dtmao.cc/news_show_828073.shtml) or [this file](./rosdep_init_and_rosdep_update_problem.html).

3. In case of command `wstool merge -t . https://raw.githubusercontent.com/ros-planning/moveit/master/moveit.rosinstall`: for whom cannot access github fast especially in China, replace `https://raw.githubusercontent.com/ros-planning/moveit/master/moveit.rosinstall` with [this file](./moveit.rosinstall).

4. Note that when using command `catkin`, please add `sudo` prefix.

5. Boost_INCLUDE_DIR may be not found when `catkin build`, just add `find_package(Boost QUIET)` in `ws_moveit/src/geometric_shapes/CMakeLists.txt`.





