## Prerequisites

Before you can run the node, make sure you have the following installed:
- [ROS (Robot Operating System)](http://wiki.ros.org/ROS/Installation)
- [TurtleBot3](https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/)
- [aws-robomaker-bookstore-world](https://github.com/aws-robotics/aws-robomaker-bookstore-world)

## Installation

1. **Clone the Repository**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Build the Package**

    Ensure you are in the workspace root directory (e.g., `catkin_ws`).

    ```bash
    catkin_make
    source devel/setup.bash
    ```

## Running the Node

To run the node, use the following command:

```bash
rosrun <package_name> <node_name>
```

Replace `<package_name>` with the name of your package and `<node_name>` with the name of the node executable.

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
