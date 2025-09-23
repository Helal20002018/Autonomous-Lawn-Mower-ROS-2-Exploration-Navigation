
# Autonomous Lawn Mower – ROS 2 Exploration & Navigation

## 📌 Project Overview

This project implements an **autonomous lawn mower robot** capable of navigating and covering all grassy areas in a given environment.
Using **ROS 2 Jazzy**, **Gazebo Harmonic**, and an **exploration algorithm**, the robot autonomously scans the environment, builds a map, and ensures complete area coverage while mowing.

<img width="2048" height="1152" alt="enhanced_WhatsApp Image 2025-01-16 at 1-41-00 PM" src="https://github.com/user-attachments/assets/741cbf4d-c28b-4651-b51d-5fd658421c20" />


![Generated File April 19, 2025 - 11_14PM](https://github.com/user-attachments/assets/52dad1af-4ba5-4f41-aef0-0b3de3c1ffa9)

## 🔧 Hardware Components

* **RPLiDAR A1** – for 2D LiDAR-based mapping and obstacle detection
* **Raspberry Pi 4 Model B (8 GB RAM)** – onboard processing unit
* **Chassis & Mower Platform** – differential drive base with cutting mechanism

## 🛠️ Software Stack

* **Operating System**: Ubuntu 22.04
* **Middleware**: ROS 2 Jazzy
* **Simulation**: Gazebo Harmonic
* **Mapping & Navigation**: ROS 2 Navigation Stack (Nav2)
* **Exploration**: Frontier-based exploration algorithm for full area coverage

## 🚀 Features

* Autonomous **area exploration and mapping**
* **Navigation with obstacle avoidance** using Nav2
* Full **grass coverage** of the mapped environment
* Real-time simulation in Gazebo Harmonic
* Modular launch files for easy execution

## ▶️ How to Run the Project

Open **four terminals** and run the following commands:

```bash
# Terminal 2: Spawn the robot model
ros2 launch robot_description spawn_robot.launch.py

# Terminal 3: Start the navigation stack
ros2 launch robot_description navigation.launch.py

# Terminal 4: Run the exploration algorithm
ros2 launch robot_exploration exploration.launch.py
```

Once running, the robot will **autonomously explore and cover all grassy areas** within the map.

## ✅ Outcome

* Achieved **fully autonomous lawn coverage** in a simulated environment.
* Successfully integrated **RPLiDAR A1** for mapping and obstacle avoidance.
* Demonstrated **ROS 2 Jazzy + Gazebo Harmonic** workflow with modular launch files.
* Provided a scalable framework for future **real-world deployment** on physical hardware.

---
