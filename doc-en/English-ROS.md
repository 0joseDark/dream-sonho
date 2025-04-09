- [back](https://github.com/0joseDark/dream-sonho/edit/main/doc-en/en-README.md)
- The **ROS (Robot Operating System)** is not an operating system in the traditional sense but rather a set of tools, libraries, and conventions to assist in the development of robotic applications. It provides a modular framework that allows different parts of a robot to communicate efficiently with each other.

## 🔹 **Key Concepts of ROS**
1. **Node** 🖥️  
   - A node is a process that performs a specific task within the ROS system.  
   - For example, one node may control the motors, another may capture images from a camera, and another may process sensor data.

2. **Topics** 🔄  
   - These are communication channels used by nodes to send and receive messages asynchronously.  
   - Example: A sensor node may publish readings on a topic called `/sensor_data`, and a control node may subscribe to this topic to process the data.

3. **Messages** 📦  
   - The data format used for communication between nodes.  
   - Example: A message may contain the position of a robot (x, y, θ) or the intensity of a sensor.

4. **Services** ⚡  
   - Unlike topics, which allow continuous communication, services enable request-response communication.  
   - Example: A node can send a request to another node to obtain the robot's current position.

5. **Actions** 🎯  
   - Similar to services but allow for long-running tasks and provide feedback during execution.  
   - Example: A robot may receive a command to move to a point and send updates during the journey.

6. **Packages** 📦  
   - ROS code is organized into packages, which can contain nodes, messages, services, and configurations.  
   - Example: A package may contain code to control a robotic arm.

7. **ROS Master** 🏆  
   - Coordinates communication between nodes.  
   - It keeps a record of which nodes exist and which topics are being published or subscribed to.

## 🔹 **Versions of ROS**
1. **ROS 1 (Classic)** 🏗️  
   - Used for many years but has limitations, such as a lack of native support for multiple robots in real-time.  

2. **ROS 2 (Current)** 🚀  
   - More modern, with better support for distributed robots and real-time communication.  
   - Uses **DDS (Data Distribution Service)** to improve communication.

## 🔹 **How is ROS Used?**
- **Mobile robots** 🤖 (e.g., autonomous cars, drones)  
- **Robotic arms** 🦾 (e.g., industrial production)  
- **Simulation** 🖥️ (e.g., Gazebo, RViz)  
- **Computer vision** 👀 (e.g., OpenCV + ROS)  

## 🔹 **Installing ROS on Ubuntu**
```bash
sudo apt update
sudo apt install ros-noetic-desktop-full
```
For ROS 2:
```bash
sudo apt update
sudo apt install ros-humble-desktop
```
