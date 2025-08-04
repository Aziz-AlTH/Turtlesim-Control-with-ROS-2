# Turtlesim-Control-with-ROS-2
This project demonstrates how to manipulate the [turtlesim](https://github.com/ros/ros_tutorials/tree/ros2/turtlesim) package in **ROS 2** using a custom Python node that sends velocity commands to the turtle.


---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

- ROS 2 (Foxy, Humble, etc.)
- `turtlesim` package
- Python 3 environment

### 1. Source ROS 2 Workspace

```
source /opt/ros/humble/setup.bash
```

#### 2. Run turtlesim node 
```
ros2 run turtlesim turtlesim_node

```
![ros2 run turtlesim turtlesim_node](https://github.com/Aziz-AlTH/Turtlesim-Control-with-ROS-2/blob/main/Screenshot-1%20from%202025-08-04%2007-15-51.png)

#### 3. Run the controller node 
```
python3 move_turtle.py

```
![Run the controller node](https://github.com/Aziz-AlTH/Turtlesim-Control-with-ROS-2/blob/main/Screencast%20from-2%2008-04-2025%2007_18_54%20AM.webm)

![Run the controller node](https://github.com/Aziz-AlTH/Turtlesim-Control-with-ROS-2/blob/main/Screencast-3%20from%2008-04-2025%2007_26_24%20AM.webm)

#  🛠️ Advanced ROS 2 Features
#### Spawn a new turtle:
```
ros2 service call /spawn turtlesim/srv/Spawn "{x: 5.0, y: 5.0, theta: 0.0, name: 'turtle2'}"

```
![Spawn a new turtle](https://github.com/Aziz-AlTH/Turtlesim-Control-with-ROS-2/blob/main/photo-4_2025-08-04_07-50-46.jpg)

#### Kill a turtle:
```
ros2 service call /kill turtlesim/srv/Kill "{name: 'turtle1'}"
```
![ Kill a turtle](https://github.com/Aziz-AlTH/Turtlesim-Control-with-ROS-2/blob/main/photo-5_2025-08-04_07-51-39.jpg)

#### Clear the background:
```
ros2 service call /clear std_srvs/srv/Empty
```
![Clear the background](https://github.com/Aziz-AlTH/Turtlesim-Control-with-ROS-2/blob/main/photo-6%20_2025-08-04_07-51-52.jpg)

# 🎯 Educational Goals
Understand ROS 2 topics and publishers

Work with geometry messages (Twist)

Use ROS 2 services and parameters

Learn to create basic control nodes

# 👨‍💻 Author
#### Abdulaziz Awad Althubaiti
Student at Taif University – College of Computers and Information Technology

Project for learning and demonstrating basic ROS 2 control using turtlesim.
















