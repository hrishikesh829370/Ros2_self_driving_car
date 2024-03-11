# Ros2_self_driving_car


Ros2_Self-Driving_Car

This project implements a Level 3 self-driving car using OSRF packages within the ROS2 framework. A Level 3 self-driving car can operate conditionally under specific environmental conditions and may require human intervention in some situations.

* **Designed a city environment in Blender and simulated it in Gazebo.**  
* **Developed a perception pipeline for lane detection and traffic signal recognition.** 
* **Implemented an advanced control algorithm for navigating T-junctions, intersections, and cruise control.** 
* **Utilized a custom CNN for object classification.** 
* **Implemented Dijkstra's and A star algorithms for path planning.**



The World:
![world](https://github.com/hrishikesh829370/Ros2_self_driving_car/assets/131910887/af6f7590-821c-4449-9545-6287c3107b12)


A realistic city environment created in Blender and simulated in Gazebo.

Traffic Signal Recognition:
![traffic_signal](https://github.com/hrishikesh829370/Ros2_self_driving_car/assets/131910887/fb6eeadc-ab3d-422c-94b8-7b6844594673)

The car identifies the traffic signal (red light) and comes to a stop.

## Project Structure:

* **The project code is organized into the following directories and files:**
```
├── computer_vision_node.py  # Core module for computer vision processing
├── config/                   # Configuration files
│   ├── config.py
│   └── __init__.py
├── data/                      # Data files (models, images, etc.)
│   ├── __init__.py
│   ├── Requirements.txt        # Dependencies for the data directory
│   ├── saved_model_Ros2_5_Sign.h5  # Trained CNN model for object classification
│   ├── TrafficLight_cascade.xml   # Pre-trained cascade classifier for traffic light detection
│   └── Vis_CNN.png               # Visualization of the CNN architecture (optional)
├── Detection/                 # Modules for object detection (lanes & signs)
│   ├── __init__.py
│   ├── Lanes/                   # Lane detection sub-modules
│       ├── a_Segmentation/        # Lane segmentation algorithms
│           ├── colour_segmentation_final.py
│           └── __init__.py
│       ├── b_Estimation/          # Lane estimation algorithms
│           ├── __init__.py
│           └── Our_EstimationAlgo.py
│       ├── c_Cleaning/             # Lane cleaning and refinement algorithms
│           ├── CheckifYellowLaneCorrect_RetInnerBoundary.py
│           ├── ExtendLanesAndRefineMidLaneEdge.py
│           └── __init__.py
│       ├── d_LaneInfo_Extraction/  # Lane information extraction algorithms
│           ├── GetStateInfoandDisplayLane.py
│           └── __init__.py
│       ├── __init__.py              # Lanes sub-module initialization
│       ├── Lane_Detection.py      # Main lane detection script
│       ├── Morph_op.py             # Image processing utilities
│       └── utilities.py            # General utility functions
│   ├── Signs/                    # Sign detection sub-modules
│       ├── Classification/        # Sign classification using CNN
│           ├── Classification_CNN.py
│           ├── CNN.py
│           ├── __init__.py
│           ├── test_images            # Folder containing test images for the CNN
│           └── Visualize_CNN.py        # Script to visualize the CNN architecture
│       ├── __init__.py              # Signs sub-module initialization
│       └── Sign

```
