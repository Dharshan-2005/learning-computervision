# 90-Day Computer Vision → Drone & Defence AI Engineer Roadmap

## Goal

Build a job-ready profile for:

-   Computer Vision Engineer
-   Perception Engineer
-   Robotics AI Engineer
-   Drone/UAV Perception Engineer
-   Autonomous Systems Engineer
-   Defence AI/ML Engineer
-   Vision & Deep Learning Engineer
-   Robotics Research Engineer

### Target profile

``` text
Computer Vision
      +
Deep Learning
      +
3D Perception
      +
C++ / Linux
      +
ROS2
      +
PX4 / Gazebo
      +
Sensor Fusion / SLAM
      +
ONNX / TensorRT / Edge AI
      =
Drone / Autonomous Systems Perception Engineer
```

## Important strategy

Do not learn computer vision as only an OpenCV/YOLO skill.

The differentiator is:

> **Perception + 3D vision + robotics + real-time deployment**

You do not need to buy a drone during this roadmap. Use simulation with
PX4, Gazebo and ROS2.

------------------------------------------------------------------------

# Daily Study Structure

### Weekdays --- \~3 hours

  Time     Activity
  -------- ---------------------------------
  45 min   Theory
  60 min   Coding
  60 min   Project implementation
  30 min   Homework / independent research
  15 min   GitHub documentation

### Saturday --- 5--6 hours

Deep implementation + project work.

### Sunday --- 4--5 hours

Revision + challenging experiment + documentation.

### Core rule

``` text
30% learning
70% implementation
```

For every important concept:

``` text
Learn
  ↓
Implement from scratch
  ↓
Use a library
  ↓
Break/test it
  ↓
Benchmark
  ↓
Optimize
  ↓
Document
```

------------------------------------------------------------------------

# Skill Priority

  Skill                  Priority
  -------------------- ----------
  Python                    ★★★★★
  OpenCV                    ★★★★★
  PyTorch                   ★★★★★
  Object Detection          ★★★★★
  Object Tracking           ★★★★★
  3D Computer Vision        ★★★★★
  C++                       ★★★★★
  ROS2                      ★★★★★
  PX4                       ★★★★★
  Gazebo                    ★★★★★
  Linux                      ★★★★
  ONNX                       ★★★★
  TensorRT                   ★★★★
  CUDA                       ★★★★
  SLAM                       ★★★★
  Sensor Fusion              ★★★★
  Kalman / EKF               ★★★★
  Docker                      ★★★
  Git                       ★★★★★
  Kubernetes                   ★★

For the next 90 days, prioritize ROS2 + PX4 + 3D vision over Kubernetes.

------------------------------------------------------------------------

# PHASE 1 --- DAYS 1--14

# Computer Vision Foundations

## Day 1 --- Image Fundamentals

### Learn

-   Pixels
-   RGB/BGR
-   Grayscale
-   Resolution
-   Channels
-   Bit depth
-   Image tensors
-   Normalization

### Practice

-   Read image
-   Resize
-   Crop
-   Rotate
-   Flip
-   Brightness
-   Contrast
-   RGB → HSV

### Homework

Build an **Image Processing CLI**:

``` text
cv_tool.py

--resize
--crop
--rotate
--grayscale
--brightness
--contrast
--blur
```

------------------------------------------------------------------------

## Day 2 --- OpenCV

### Learn

-   OpenCV architecture
-   `VideoCapture`
-   Image writing
-   Drawing
-   Bounding boxes
-   Text
-   FPS calculation

### Homework

Build a real-time webcam analysis dashboard displaying:

-   Resolution
-   FPS
-   Average brightness
-   Dominant color
-   Motion detected

------------------------------------------------------------------------

## Day 3 --- Filtering

### Learn

-   Gaussian filter
-   Median filter
-   Bilateral filter
-   Sobel
-   Laplacian
-   Canny

### Homework

Compare:

``` text
Original
Gaussian
Median
Bilateral
Sobel
Laplacian
Canny
```

Explain when each filter fails.

------------------------------------------------------------------------

## Day 4 --- Morphology

### Learn

-   Erosion
-   Dilation
-   Opening
-   Closing
-   Morphological gradient

### Homework

Build a noise-removal pipeline:

``` text
Noisy binary image
        ↓
Morphological processing
        ↓
Clean object mask
```

------------------------------------------------------------------------

## Day 5 --- Contours

### Learn

-   Contour detection
-   Bounding rectangles
-   Rotated rectangles
-   Area
-   Perimeter
-   Convex hull
-   Shape approximation

### Homework

Build an **Object Shape Analyzer**:

``` text
Triangle
Rectangle
Circle
Unknown
```

------------------------------------------------------------------------

## Day 6 --- Motion Detection

### Learn

-   Frame differencing
-   Background subtraction
-   MOG2
-   Motion contours

### Start Project 1

# Project 1 --- Aerial Surveillance Motion Detection

Pipeline:

``` text
Video
 ↓
Preprocessing
 ↓
Background subtraction
 ↓
Motion detection
 ↓
Contour filtering
 ↓
Bounding boxes
 ↓
Track moving regions
 ↓
FPS + event log
```

Use public aerial footage.

------------------------------------------------------------------------

## Day 7 --- Weekly Challenge

Without YOLO, build a moving-object detection system.

Requirements:

-   Detect moving objects
-   Remove noise
-   Draw boxes
-   Calculate object area
-   Calculate FPS
-   Save detected frames

------------------------------------------------------------------------

## Day 8 --- Image Geometry

### Learn

-   Coordinate systems
-   Image coordinates
-   Translation
-   Rotation
-   Scaling
-   Affine transformation
-   Perspective transformation

### Homework

Implement basic transformations using NumPy/OpenCV.

------------------------------------------------------------------------

## Day 9 --- Homography

### Learn

-   Homography
-   Perspective transform
-   Planar mapping

### Homework

Build a **Drone Ground Mapping Simulator**:

``` text
Aerial image
     ↓
Perspective transform
     ↓
Bird's-eye / top-down view
```

------------------------------------------------------------------------

## Day 10 --- Feature Detection

### Learn

-   Harris
-   Shi-Tomasi
-   FAST
-   ORB
-   SIFT concepts

### Homework

Compare ORB vs SIFT under:

-   Rotation
-   Scaling
-   Blur
-   Illumination changes

------------------------------------------------------------------------

## Day 11 --- Feature Matching

### Learn

-   Descriptors
-   BFMatcher
-   FLANN
-   Ratio test
-   RANSAC

### Homework

Build an **Aerial Image Matching System**.

Input:

``` text
Image A
Image B
```

Output matching regions.

------------------------------------------------------------------------

## Day 12 --- Optical Flow

### Learn

-   Lucas-Kanade
-   Farneback
-   Sparse optical flow
-   Dense optical flow

### Homework

Track feature movement through a video.

------------------------------------------------------------------------

## Day 13 --- Camera Calibration

### Learn

-   Intrinsic parameters
-   Extrinsic parameters
-   Distortion
-   Focal length
-   Principal point
-   Camera matrix

### Homework

Implement:

``` text
camera_calibration.py
```

------------------------------------------------------------------------

## Day 14 --- Project 1 Completion

### Aerial Vision Surveillance System

Recommended structure:

``` text
aerial-surveillance/
├── src/
│   ├── preprocessing/
│   ├── motion/
│   ├── tracking/
│   └── visualization/
├── configs/
├── tests/
├── demo/
├── requirements.txt
└── README.md
```

------------------------------------------------------------------------

# PHASE 2 --- DAYS 15--30

# Deep Learning + Object Detection

## Day 15 --- Neural Network Fundamentals

Learn:

-   Neural networks
-   Tensors
-   Forward propagation
-   Loss
-   Backpropagation

### Homework

Implement a small neural network in PyTorch.

------------------------------------------------------------------------

## Day 16 --- CNN

Learn:

-   Convolution
-   Stride
-   Padding
-   Pooling
-   Receptive field

### Homework

Build a CNN image classifier.

------------------------------------------------------------------------

## Day 17 --- Training

Learn:

-   Batch normalization
-   Dropout
-   Augmentation
-   Learning rate
-   Optimizers

Experiment with:

-   Adam
-   SGD
-   AdamW

------------------------------------------------------------------------

## Day 18 --- Transfer Learning

Learn:

-   Transfer learning
-   ResNet
-   EfficientNet
-   Feature extraction

Train your own classifier.

------------------------------------------------------------------------

## Day 19 --- Detection Fundamentals

Understand:

``` text
Classification
Localization
Object detection
Segmentation
```

------------------------------------------------------------------------

## Day 20 --- YOLO Deep Dive

Do not just learn:

``` python
model.predict()
```

Understand:

-   Backbone
-   Neck
-   Detection head
-   Bounding boxes
-   Confidence
-   NMS
-   IoU

------------------------------------------------------------------------

## Day 21 --- Custom YOLO Dataset

Train YOLO on a custom aerial dataset.

Possible classes:

``` text
person
vehicle
building
tree
road
```

------------------------------------------------------------------------

## Day 22 --- Evaluation

Learn:

-   Precision
-   Recall
-   F1
-   IoU
-   mAP50
-   mAP50-95
-   Confusion matrix

### Homework

Create a complete evaluation report.

------------------------------------------------------------------------

## Day 23 --- Dataset Engineering

Learn:

-   Dataset imbalance
-   Hard negatives
-   Augmentation
-   Label noise
-   False positives
-   False negatives

### Homework

Create an intentionally bad dataset and diagnose model failure.

------------------------------------------------------------------------

## Day 24 --- Object Tracking

Learn:

-   Detection vs tracking
-   Kalman filter
-   Hungarian algorithm
-   DeepSORT
-   ByteTrack

------------------------------------------------------------------------

## Day 25 --- Multi-Object Tracker

Build:

``` text
YOLO
 ↓
Kalman Filter
 ↓
Data Association
 ↓
Track IDs
```

------------------------------------------------------------------------

## Day 26 --- Tracking Failure Modes

Test:

-   Occlusion
-   ID switches
-   Track loss
-   Re-identification

Make the tracker survive:

-   Object disappears
-   Object reappears
-   Multiple objects cross

------------------------------------------------------------------------

## Day 27 --- Segmentation

Learn:

-   Semantic segmentation
-   Instance segmentation
-   U-Net
-   Mask R-CNN
-   YOLO segmentation

------------------------------------------------------------------------

## Day 28 --- Aerial Scene Segmentation

Segment:

``` text
road
vegetation
building
vehicle
person
```

------------------------------------------------------------------------

## Day 29 --- Vision Transformers

Understand:

-   Image patches
-   Positional encoding
-   Attention
-   ViT
-   DETR

Focus on architectural tradeoffs rather than memorizing every model.

------------------------------------------------------------------------

## Day 30 --- Project 2

# Project 2 --- Autonomous Aerial Perception System

Architecture:

``` text
Drone Video
     ↓
YOLO Detector
     ↓
ByteTrack / DeepSORT
     ↓
Object IDs
     ↓
Trajectory estimation
     ↓
Event detection
     ↓
Dashboard
```

Track:

-   Object ID
-   Class
-   Confidence
-   Position
-   Velocity estimate
-   Trajectory

------------------------------------------------------------------------

# PHASE 3 --- DAYS 31--45

# 3D Computer Vision

## Day 31 --- 3D Coordinate Systems

Learn:

-   3D coordinate systems
-   Camera coordinates
-   World coordinates
-   Body coordinates

------------------------------------------------------------------------

## Day 32 --- Transformations

Learn:

-   Rotation matrices
-   Translation
-   Homogeneous coordinates
-   SE(3)

------------------------------------------------------------------------

## Day 33 --- Perspective Projection

Understand:

``` text
3D world
   ↓
Camera
   ↓
2D image
```

------------------------------------------------------------------------

## Day 34 --- Camera Model

Learn:

-   Intrinsic matrix
-   Extrinsic matrix
-   Projection matrix

### Homework

Implement camera projection with NumPy.

------------------------------------------------------------------------

## Day 35 --- PnP

Understand:

``` text
3D points
+
2D image points
      ↓
Camera pose
```

Implement OpenCV PnP.

------------------------------------------------------------------------

## Day 36 --- Stereo Vision

Understand:

``` text
Left camera + Right camera
          ↓
      Disparity
          ↓
         Depth
```

------------------------------------------------------------------------

## Day 37 --- Stereo Depth

Build a stereo depth estimation system using a public stereo dataset.

------------------------------------------------------------------------

## Day 38 --- Epipolar Geometry

Learn:

-   Triangulation
-   Epipolar geometry
-   Fundamental matrix
-   Essential matrix

------------------------------------------------------------------------

## Day 39 --- Visual Odometry

Build:

``` text
Frame t
 ↓
Features
 ↓
Frame t+1
 ↓
Feature matching
 ↓
Essential matrix
 ↓
Pose estimation
```

------------------------------------------------------------------------

## Day 40 --- Optical Flow Visual Odometry

Compare:

``` text
Feature matching
vs
Optical flow
```

------------------------------------------------------------------------

## Day 41 --- Kalman Filter

Understand:

``` text
Prediction
    ↓
Measurement
    ↓
Correction
```

Implement the equations.

------------------------------------------------------------------------

## Day 42 --- Kalman Filter From Scratch

Track:

``` text
x
y
vx
vy
```

with noisy measurements.

------------------------------------------------------------------------

## Day 43 --- Extended Kalman Filter

Learn why nonlinear systems require EKF.

------------------------------------------------------------------------

## Day 44 --- Sensor Fusion

Understand:

``` text
Camera + IMU
     ↓
State estimation
```

Study:

-   State
-   Measurement model
-   Process noise
-   Measurement noise

------------------------------------------------------------------------

## Day 45 --- Project 3

# Project 3 --- Vision-Based Drone Localization

Build:

``` text
Camera frames
      +
IMU data
      ↓
Feature tracking
      ↓
Visual odometry
      ↓
EKF
      ↓
Estimated drone trajectory
```

Compare:

``` text
Ground-truth trajectory
vs
Estimated trajectory
```

Measure trajectory error.

------------------------------------------------------------------------

# PHASE 4 --- DAYS 46--60

# ROS2 + PX4 + Gazebo

## Day 46 --- Linux for Robotics

Learn:

-   Filesystem
-   Processes
-   Permissions
-   Bash
-   SSH
-   Environment variables

------------------------------------------------------------------------

## Day 47 --- Robotics Environment

Configure:

-   Ubuntu / WSL2 if using Windows
-   ROS2
-   Gazebo

------------------------------------------------------------------------

## Day 48 --- ROS2 Basics

Learn:

-   Nodes
-   Topics
-   Publishers
-   Subscribers

------------------------------------------------------------------------

## Day 49 --- ROS2 Camera Pipeline

Build:

``` text
camera_publisher
camera_subscriber
```

------------------------------------------------------------------------

## Day 50 --- ROS2 Services and Actions

Learn:

-   Services
-   Actions
-   Parameters
-   Launch files

------------------------------------------------------------------------

## Day 51 --- TF2

Understand:

``` text
map
 ↓
odom
 ↓
base_link
 ↓
camera
```

------------------------------------------------------------------------

## Day 52 --- ROS2 + OpenCV

Build:

``` text
Camera
 ↓
ROS2
 ↓
OpenCV
 ↓
YOLO
 ↓
Detection topic
```

------------------------------------------------------------------------

## Day 53 --- Gazebo

Learn:

-   Worlds
-   Models
-   Sensors
-   Cameras
-   Depth cameras
-   IMU

------------------------------------------------------------------------

## Day 54 --- PX4 Fundamentals

Understand:

``` text
PX4
 ↓
Flight controller
 ↓
Sensors
 ↓
Actuators
```

------------------------------------------------------------------------

## Day 55 --- PX4 SITL

Run a simulated quadrotor.

Learn:

-   SITL
-   Simulation environment
-   Vehicle state
-   Basic telemetry

------------------------------------------------------------------------

## Day 56 --- PX4 + ROS2

Understand:

``` text
Gazebo
 ↓
PX4 SITL
 ↓
ROS2
 ↓
Computer Vision
```

------------------------------------------------------------------------

## Day 57 --- Drone Camera + YOLO

Build:

``` text
Drone camera
 ↓
ROS2
 ↓
YOLO
 ↓
Detection
```

------------------------------------------------------------------------

## Day 58 --- Obstacle Detection

Build:

``` text
Camera / depth
      ↓
Obstacle estimation
      ↓
Distance
      ↓
Warning
```

------------------------------------------------------------------------

## Day 59 --- Safe Autonomous Avoidance

Implement a simulation-only avoidance pipeline:

``` text
Obstacle
   ↓
Perception
   ↓
Free-space estimation
   ↓
Planner
   ↓
Safe waypoint
```

------------------------------------------------------------------------

## Day 60 --- Project 4

# Project 4 --- Autonomous Drone Perception & Avoidance Simulator

Architecture:

``` text
                  GAZEBO
                    │
             Simulated Drone
                    │
          ┌─────────┴─────────┐
          │                   │
       Camera                IMU
          │                   │
          └─────────┬─────────┘
                    ↓
                  ROS2
                    ↓
              Vision Node
                    ↓
              YOLO / CV
                    ↓
          Object + Obstacle Map
                    ↓
                Planner
                    ↓
                PX4 SITL
```

------------------------------------------------------------------------

# PHASE 5 --- DAYS 61--75

# Production CV + Edge AI

## Day 61 --- C++ Fundamentals

Focus on:

-   Classes
-   Pointers
-   References
-   STL
-   Vectors
-   Maps
-   Smart pointers
-   OOP

------------------------------------------------------------------------

## Day 62 --- CMake

Learn:

-   Headers
-   Source files
-   CMake
-   Linking
-   Libraries

------------------------------------------------------------------------

## Day 63 --- OpenCV C++

Recreate one Python computer vision pipeline in C++.

------------------------------------------------------------------------

## Day 64 --- CUDA Fundamentals

Understand:

-   CPU vs GPU
-   Threads
-   Blocks
-   Memory
-   Parallelism

------------------------------------------------------------------------

## Day 65 --- ONNX

Build:

``` text
PyTorch
 ↓
ONNX
 ↓
ONNX Runtime
```

------------------------------------------------------------------------

## Day 66 --- Inference Benchmark

Compare:

``` text
PyTorch
vs
ONNX Runtime
```

Measure:

-   FPS
-   Latency
-   Memory

------------------------------------------------------------------------

## Day 67 --- TensorRT

Learn:

-   TensorRT concepts
-   FP32
-   FP16
-   INT8
-   Optimization
-   Inference engines

------------------------------------------------------------------------

## Day 68 --- Optimized Detector

Convert your detector into an optimized inference pipeline.

------------------------------------------------------------------------

## Day 69 --- Quantization

Compare:

``` text
FP32
FP16
INT8
```

Measure accuracy vs performance.

------------------------------------------------------------------------

## Day 70 --- Real-Time Systems

Measure:

-   Capture latency
-   Preprocessing latency
-   Inference latency
-   Postprocessing latency
-   Total latency
-   FPS

------------------------------------------------------------------------

## Day 71 --- Docker for AI

Containerize:

-   CV pipeline
-   YOLO
-   ROS2 component
-   API

------------------------------------------------------------------------

## Day 72 --- Logging + Monitoring

Log:

-   FPS
-   Latency
-   Detection count
-   Confidence
-   Errors
-   CPU
-   GPU

------------------------------------------------------------------------

## Day 73 --- CV Testing

Test:

-   Empty frame
-   Bad image
-   Low light
-   Motion blur
-   Occlusion
-   Camera failure

------------------------------------------------------------------------

## Day 74 --- Stress Testing

Stress-test the full perception pipeline.

------------------------------------------------------------------------

## Day 75 --- Project 5

# Project 5 --- Real-Time Edge Vision Pipeline

Architecture:

``` text
Camera
 ↓
OpenCV
 ↓
ONNX / TensorRT
 ↓
Object Detection
 ↓
Tracking
 ↓
Event Engine
 ↓
ROS2
 ↓
Dashboard
```

Measure:

-   FPS
-   Latency
-   CPU
-   GPU
-   RAM
-   Model size

------------------------------------------------------------------------

# PHASE 6 --- DAYS 76--90

# Advanced Autonomous Perception + Jobs

## Day 76 --- SLAM Fundamentals

Understand:

``` text
Localization
+
Mapping
=
SLAM
```

------------------------------------------------------------------------

## Day 77 --- Visual SLAM

Study:

-   ORB-SLAM concepts
-   Feature tracking
-   Loop closure
-   Map points

------------------------------------------------------------------------

## Day 78 --- Run a Visual SLAM System

Run an existing system and draw its complete architecture yourself.

------------------------------------------------------------------------

## Day 79 --- Multi-Sensor Fusion

Understand:

``` text
Camera
IMU
GPS/GNSS
Depth
LiDAR
```

------------------------------------------------------------------------

## Day 80 --- Perception Failure Modes

Test:

-   Low light
-   Motion blur
-   Occlusion
-   Camera vibration
-   Rapid movement
-   GPS loss
-   Poor texture
-   Weather-like degradation

------------------------------------------------------------------------

## Day 81 --- Robustness Test Suite

Create datasets for:

``` text
normal
blur
dark
bright
noise
occlusion
compression
```

Measure model degradation.

------------------------------------------------------------------------

## Day 82 --- Domain Adaptation

Understand:

``` text
Training environment
        ↓
Deployment environment
```

Study how distribution shifts affect detection and perception.

------------------------------------------------------------------------

## Day 83 --- Synthetic Data

Generate simulated data with:

-   Different lighting
-   Camera angles
-   Obstacles
-   Backgrounds
-   Object positions

------------------------------------------------------------------------

## Day 84 --- Active Learning

Understand:

``` text
Model
 ↓
Uncertain samples
 ↓
Human labeling
 ↓
Retraining
```

------------------------------------------------------------------------

## Day 85 --- Hard Example Mining

Automatically save images where:

``` text
confidence < threshold
```

Use them to build a retraining dataset.

------------------------------------------------------------------------

## Day 86 --- System Design

Design:

> Real-time autonomous aerial perception platform

Architecture:

``` text
Camera
 ↓
Preprocessing
 ↓
Detection
 ↓
Tracking
 ↓
Depth
 ↓
Localization
 ↓
Sensor fusion
 ↓
Planner
 ↓
Control
```

Be able to explain every component and its failure modes.

------------------------------------------------------------------------

## Day 87 --- Interview Day 1

Answer without notes:

1.  What is IoU?
2.  Why NMS?
3.  Explain YOLO architecture.
4.  Why tracking?
5.  What is a Kalman filter?
6.  What is optical flow?
7.  What is homography?
8.  Fundamental vs essential matrix?
9.  What is PnP?
10. How does camera calibration work?

------------------------------------------------------------------------

## Day 88 --- Interview Day 2

Explain:

-   VIO
-   SLAM
-   EKF
-   Sensor fusion
-   Stereo depth
-   Visual odometry
-   ROS2
-   PX4
-   Gazebo
-   Edge inference

------------------------------------------------------------------------

## Day 89 --- Resume + GitHub

Create:

``` text
01-aerial-surveillance
02-aerial-perception
03-visual-odometry
04-drone-autonomy
05-edge-vision
06-autonomous-aerial-perception
```

Every repository should contain:

-   README
-   Architecture diagram
-   Dataset information
-   Training procedure
-   Results
-   Metrics
-   Failure cases
-   Demo video
-   Installation instructions
-   Future work

------------------------------------------------------------------------

# DAY 90 --- FINAL CAPSTONE

# Project 6 --- Autonomous Aerial Perception & Navigation Research Platform

Combine everything.

``` text
                         SIMULATION
                             │
                         PX4/Gazebo
                             │
                    ┌────────┴────────┐
                    │                 │
                 Camera              IMU
                    │                 │
                    └────────┬────────┘
                             ↓
                           ROS2
                             ↓
                    ┌────────┴────────┐
                    │                 │
              Object Detection    Visual Odometry
                    │                 │
                 Tracking          EKF/VIO
                    │                 │
                    └────────┬────────┘
                             ↓
                     Scene Perception
                             ↓
                    Obstacle / Free Space
                             ↓
                       Path Planner
                             ↓
                          PX4 SITL
                             ↓
                     Autonomous Mission
```

### Benchmark

Measure:

-   Detection FPS
-   Tracking accuracy
-   Localization error
-   Trajectory error
-   Inference latency
-   CPU utilization
-   GPU utilization
-   Failure rate

------------------------------------------------------------------------

# Research Experiments

Do not stop at tutorials.

Create research questions.

## Experiment 1 --- Aerial Resolution

Question:

> How does aerial image resolution affect small-object detection?

Compare:

``` text
640 × 640
512 × 512
416 × 416
320 × 320
```

Measure:

-   mAP
-   Recall
-   FPS
-   Latency

------------------------------------------------------------------------

## Experiment 2 --- Camera Motion vs Tracking

Compare:

``` text
Stable camera
Slow movement
Fast movement
Motion blur
```

Measure tracking performance.

------------------------------------------------------------------------

## Experiment 3 --- Optical Flow + Detection

Question:

> Can optical flow improve tracking during temporary detection failure?

------------------------------------------------------------------------

## Experiment 4 --- Quantization

Compare:

``` text
FP32
FP16
INT8
```

Measure:

-   Accuracy
-   FPS
-   Latency
-   Memory

------------------------------------------------------------------------

## Experiment 5 --- Visual Odometry Drift

Measure how trajectory error increases over time.

------------------------------------------------------------------------

# Job Search Strategy

Do not search only for "Drone Engineer".

Search for:

## Computer Vision

-   Computer Vision Engineer
-   Computer Vision Intern
-   Vision AI Engineer
-   Deep Learning Engineer
-   Perception Engineer

## Robotics

-   Robotics Perception Engineer
-   Robotics Software Engineer
-   Autonomous Systems Engineer
-   Robotics AI Engineer

## Drone

-   Drone Perception Engineer
-   UAV Perception Engineer
-   Autonomous Drone Engineer
-   UAV Computer Vision Engineer
-   Aerial Intelligence Engineer

## Defence

-   AI/ML Engineer
-   Defence AI Engineer
-   Vision & Deep Learning Engineer
-   Autonomous Systems Engineer
-   Robotics Research Engineer
-   Perception Research Engineer

------------------------------------------------------------------------

# Defence Career Strategy

Use three paths simultaneously:

``` text
                  DEFENCE TARGET
                       │
        ┌──────────────┼──────────────┐
        │              │              │
       DRDO       Defence Startups   Robotics
        │              │              │
     JRF / RA      CV / AI Engineer  Perception
        │              │              │
        └──────────────┼──────────────┘
                       │
                   Experience
                       ↓
               Defence R&D roles
```

Monitor:

-   DRDO research/JRF/RA opportunities
-   Defence startups
-   UAV companies
-   Robotics companies
-   Aerospace companies
-   Autonomous systems companies
-   Computer vision startups

------------------------------------------------------------------------

# Portfolio Strategy

## Project 1

### Aerial Motion Detection & Surveillance Vision

Focus:

-   Classical CV
-   Motion detection
-   Background subtraction
-   Contours

------------------------------------------------------------------------

## Project 2

### Multi-Object Aerial Perception & Tracking

Focus:

-   YOLO
-   Detection
-   ByteTrack / DeepSORT
-   Tracking
-   Trajectory estimation

------------------------------------------------------------------------

## Project 3

### Vision-Based Drone Localization

Focus:

-   3D vision
-   Optical flow
-   Visual odometry
-   EKF
-   Camera geometry

------------------------------------------------------------------------

## Project 4

### ROS2-PX4 Autonomous Drone Perception Simulator

Focus:

-   ROS2
-   PX4
-   Gazebo
-   YOLO
-   Depth
-   Obstacle avoidance

------------------------------------------------------------------------

## Project 5

### Real-Time Edge Vision Pipeline

Focus:

-   ONNX
-   TensorRT
-   CUDA
-   FP16/INT8
-   Latency
-   FPS
-   Profiling

------------------------------------------------------------------------

## Project 6

### Autonomous Aerial Perception & Navigation Research Platform

Focus:

-   ROS2
-   PX4
-   Gazebo
-   Detection
-   Tracking
-   Visual odometry
-   EKF/VIO
-   Scene perception
-   Obstacle avoidance
-   Path planning
-   Edge inference

------------------------------------------------------------------------

# Final Skill Stack

``` text
PROGRAMMING
├── Python
├── C++
└── Linux

COMPUTER VISION
├── OpenCV
├── Image Processing
├── Geometry
├── Detection
├── Segmentation
├── Tracking
├── Optical Flow
└── 3D Vision

DEEP LEARNING
├── PyTorch
├── CNN
├── YOLO
├── Transformers
└── Vision Transformers

ROBOTICS
├── ROS2
├── TF2
├── Gazebo
├── PX4
└── SITL

PERCEPTION
├── Visual Odometry
├── Stereo
├── VIO
├── SLAM
├── EKF
└── Sensor Fusion

DEPLOYMENT
├── ONNX
├── TensorRT
├── CUDA
├── Docker
└── Edge Inference

ENGINEERING
├── Git
├── Testing
├── Benchmarking
├── Profiling
└── System Design
```

------------------------------------------------------------------------

# The Aggressive Learning Method

For every important concept:

``` text
LEARN
  ↓
IMPLEMENT FROM SCRATCH
  ↓
USE LIBRARY
  ↓
BREAK IT
  ↓
BENCHMARK IT
  ↓
OPTIMIZE IT
  ↓
DOCUMENT IT
```

Example --- Kalman Filter:

``` text
Day 1:
Understand equations

Day 2:
Implement NumPy version

Day 3:
Use library implementation

Day 4:
Add noisy measurements

Day 5:
Compare prediction errors

Day 6:
Integrate with tracker

Day 7:
Document failure cases
```

This is the difference between:

> "I completed a computer vision course."

and:

> "I can engineer and debug a real-time perception system."

------------------------------------------------------------------------

# 90-Day Outcome

At the end of the roadmap, your target profile is:

``` text
Junior AI Engineer
       +
Computer Vision
       +
Deep Learning
       +
3D Perception
       +
C++
       +
ROS2
       +
PX4
       +
Gazebo
       +
SLAM / VIO / EKF
       +
ONNX / TensorRT
       +
Edge AI
       +
6 serious portfolio projects
       ↓
Drone / Robotics / Autonomous Systems /
Computer Vision / Defence AI roles
```

## Core principle

> **Do not become another YOLO developer. Become an engineer who
> understands the complete perception stack from pixels → detection →
> tracking → depth → localization → sensor fusion → robotics → real-time
> deployment.**
