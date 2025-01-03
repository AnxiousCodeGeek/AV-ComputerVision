# Autonomous Vehicle Computer Vision Project

## Overview
This repository showcases the technical aspects of a comprehensive computer vision system developed for autonomous vehicles. The project integrates multiple state-of-the-art computer vision techniques with sensor data fusion to ensure accurate perception, navigation, and decision-making capabilities for autonomous vehicles.

## Key Features
1. **Object Detection and Tracking**
    - Real-time detection and tracking of vehicles, pedestrians, traffic lights, and road signs using advanced deep learning models (e.g., YOLOv5, YOLOP).
    - A custom YOLOv5 model trained on traffic sign data and a traffic light classification model were loaded for detecting relevant objects and traffic signals and the signal colors (red, yellow, and green). We fine-tuned the parameters, confidence thresholds and IoU thresholds for optimal detection accuracy. A lightweight convolutional neural network (CNN) is used to classify traffic light colors. 
    - Optimization to reduce false positives and increase detection range for distant objects.
      
2. **Lane Detection**
     - Robust lane detection algorithms capable of identifying lanes under varying lighting and weather conditions.
     - Dynamic region of interest (ROI) optimization for efficient computation.

<div align="center">
  <img src="https://github.com/user-attachments/assets/2b18b600-50d6-4289-a2f5-bcf9552e52e7" alt="Example Image" width="700" />
</div>

       
3. **Depth Estimation for Distance Measurement**
     - The system calculates the distance to detected objects using depth information, providing warnings when objects come within a predefined safety range, thereby enhancing vehicle safety.
     - A side panel displays dynamic warnings and vehicle information, including lane curvature, vehicle position, and potential hazards.
     - We also subscribed to camera topic on ROS and published proximity warning. The topic published true upon detection of object within the set distance threshold and false if far.
  

<div align="center">
  <img src="https://github.com/user-attachments/assets/1ec616d1-feed-430f-bcf5-aa103da23c87" alt="Example Image" width="700" />
</div>


<div align="center">
  <img src="https://github.com/user-attachments/assets/815690bc-daf4-4a59-9803-7fd4943c5911" alt="Example Image" width="700" />
</div>

       
5. **Sensor Fusion**
     - Combining data from multiple sensors, including cameras, LiDAR, and GPS, to enhance perception and navigation accuracy.
     - Real-time data synchronization and processing.
       
6. **Path Planning and Control**
     - Basic motion planning experiments with ROS tools.
     - Incorporation of traffic light signals into autonomous vehicle decision-making.

<div align="center">
  <img src="https://github.com/user-attachments/assets/cd856c43-7faf-48d7-8902-ee62668b276a" alt="Example Image" width="400" />
</div>


## File Formats and Data Management

### Camera Data: 
Captured using ZED stereo cameras in .bag format.
### Processed Data: 
Object detection and distance data saved in .csv files for further analysis.
### Visualization: 
Heatmaps and 3D visualizations created using tools like RViz and Python libraries (e.g., Folium, Matplotlib).

## Contact
For further technical details, access to the codebase, or collaboration inquiries, please reach out to us at:

Email: [fatimaned3597@gmail.com](mailto:yatimaned3597@gmail.com)

LinkedIn: [Fatima Saud Linkedin](https://www.linkedin.com/in/fatima-saud-997606161/)
