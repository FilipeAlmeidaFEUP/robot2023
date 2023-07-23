# Teleop tutorial ([link](https://github.com/FilipeAlmeidaFEUP/ros2_teleopkeys_tutorial))

## Theoretical concepts

This tutorial explains to the user how ROS is structured in Nodes and how each of them should have a singular task. It shows how Nodes communicate between them using either Topics (subscriber and publisher model) or Services (server and client model). It also reinforces the importance and value of the modular structure of ROS by showing how it can be used effectively.

## Practical concepts

This tutorial shows the user how to: 
1. Use ROS 2 launch files to run several nodes
2. Change the Flatland's launch parameters
3. Create an instance of the class Node in Python
4. Publishing and subscribing to Topics in a Python script using the Node class
5. Make a service request in a Python script using the Node class
6. Use ROS 2 commands to see information about active Nodes, Topics and Services
7. Add new models to the visualization file (ROS RViz file)
8. Modify relevant setup files, such as the Python setup and the Extensible Markup Language (XML) package file
9. Configure Flatland world and layer files
10. Manage Flatland layers
11. Configure Flatland models and their plugins
12. Use plugins such as the ones in the robot from this package
13. Create two separate Nodes that communicate with each other
14. Control a robot in ROS 2 using the keyboard.


The concept of layers makes Flatland essentially a 2.5D simulator since each layer can contain different components of the world that work independently in terms of physics. This means objects in different layers will not collide with each other and a Flatland world can only have up to 16 layers. Managing layers can quickly become a very complex task, even for relatively simple projects. To provide the user some extra help with this task, a Google Slides presentation was included in the tutorial to demonstrate a method based on Graph Theory to determine the minimum number of layers and which components need to interact with them.

## Self-Learning/Autonomous work

By the end of the tutorial, the user is encouraged to attempt to create a new controller for the robot. As the example package in this tutorial already has a lot of code, it is not very inviting to make changes. To combat this issue, a [template package](https://github.com/FilipeAlmeidaFEUP/ros2_flatland_robot_controller) is also provided. This package has a similar setup to the one presented, but the Python controller written for the robot only contains a few commented basic code examples to make the robot either move forward, in a circle, or forward and turn to the right when it finds an obstacle in front of it.

The package also offers other pre-prepared maps along with the maze that the user can choose from. Some of these maps were created to resemble real-life scenarios to try to captivate the user's interest in Robotics such as a racetrack and an example of house plans.
