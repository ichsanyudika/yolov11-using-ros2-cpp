## Prerequisites

- ROS 2 (Foxy, Humble, or compatible)

- OpenCV ≥ 4.5 (with contrib)

- ONNX Runtime (C++ version)

- ROS 2 dependencies: rclcpp, geometry_msgs

- Tools: cmake, colcon, rosdep

### Model Setup

- Download the YOLOv11 ONNX model (e.g., yolov11.onnx)

- Place it in the models/ directory

- Also place coconames.txt (class labels) in the same folder

### Path Verification

- ONNX Runtime: Libraries must be installed and linked properly

- Model: yolov11.onnx inside models/

- Labels: coconames.txt inside models/

### Build & Run

    #1 Clone the repository
    git clone https://github.com/ichsanyudika/Yolov11-ROS2-CPP.git
    cd Yolov11-ROS2-CPP
    
    #2 Build the workspace
    colcon build --symlink-install
    
    #3 Source the environment
    source install/setup.bash

    # Run
    ros2 run yolo_ws main

### Result

![](output/output.png)  
