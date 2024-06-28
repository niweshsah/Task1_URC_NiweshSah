## Prerequisites

Before you can run the node, make sure you have the following installed:
- [ROS (Robot Operating System)](http://wiki.ros.org/ROS/Installation)
- [TurtleBot3](https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/)

## Installation

1.  **Make workspace (e.g. catkin_ws) **

     ```bash
    cd ~
    mkdir catkin_ws
    cd catkin_ws/
    
    ```

2.  **Clone the Repository**

    ```bash
    git clone <repository-url>
    ```

3. **Build the Package**

    Ensure you are in the workspace root directory (e.g., `catkin_ws`).

    ```bash
    catkin init
    catkin build
    source devel/setup.bash
    ```
4. **Save/copy map.yaml at home directory**
    

## Running the Node

To run the node, use the following command:

```bash
rosrun main_launch python_start_launches.py 
```
This will start 4 terminals:
1. Rosmaster
2. Gazebo world simulation with turtlebot3
3. RVIZ
4. Teleoperating command node


### Example

If your package name is `global_planner` and your node name is `global_planner_node`, you would run:

```bash
rosrun global_planner global_planner_node
```

## Usage

Describe how to use the node here. Include any necessary arguments or parameters.

```bash
rosrun global_planner global_planner_node _param1:=value1 _param2:=value2
```

## Launch Files

If you have launch files set up, you can use them to simplify running your node. For example:

```bash
roslaunch <package_name> <launch_file>
```

### Example

```bash
roslaunch global_planner global_planner.launch
```

## Troubleshooting

If you encounter any issues, check the following:
- Ensure all dependencies are installed.
- Verify the node is being run in the correct environment.
- Check ROS logs for error messages.

```bash
roslaunch global_planner global_planner.launch
```

## Contributing

If you would like to contribute, please fork the repository and create a pull request with your changes.

## License

Include information about the licensing of your project.

---

Feel free to modify the template according to your specific requirements.
