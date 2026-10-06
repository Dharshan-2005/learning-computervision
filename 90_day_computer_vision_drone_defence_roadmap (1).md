# 90-Day Aggressive Computer Vision → Drone AI → Defence Roadmap

**Target:** Become interview-ready for junior Computer Vision /
Perception / Robotics / UAV AI / Edge AI roles in \~90 days.

**Primary job targets** - Computer Vision Engineer - Perception
Engineer - Robotics/Autonomy Engineer - UAV/Drone AI Engineer - Edge AI
Engineer - Visual Navigation Engineer - AI/ML Engineer --- Defence /
Aerospace - Remote Sensing / Geospatial AI Engineer - Robotics Software
Engineer

**Important:** This roadmap is designed around non-weaponized
applications: surveillance, search-and-rescue, mapping, inspection,
navigation, obstacle avoidance, perimeter monitoring, disaster response,
and autonomous robotics. Do not build systems for weapon targeting or
autonomous engagement.

------------------------------------------------------------------------

# 1. What you should become after 90 days

Your profile should not look like:

> "I know Python, OpenCV and YOLO."

It should look like:

> **Computer Vision / AI Engineer who can build, evaluate, optimize and
> deploy real-time perception systems, integrate them with ROS 2/PX4
> simulation, perform tracking and visual localization, and deploy
> models on constrained NVIDIA edge hardware.**

Your technical stack:

``` text
Python
├── NumPy / SciPy
├── OpenCV
├── PyTorch
├── Albumentations
├── Ultralytics YOLO
├── ONNX
└── FastAPI

Computer Vision
├── Image processing
├── Camera geometry
├── Calibration
├── Feature detection/matching
├── Optical flow
├── Object detection
├── Segmentation
├── Multi-object tracking
├── Pose estimation
└── 3D vision

Robotics
├── Linux
├── C++
├── ROS 2
├── TF2
├── Gazebo
├── SLAM
├── VIO concepts
├── Kalman filtering
├── Sensor fusion
└── Coordinate frames

Drone
├── PX4
├── MAVLink concepts
├── PX4 SITL
├── Gazebo
├── Offboard control
├── Camera perception
└── Visual navigation concepts

Edge AI
├── CUDA basics
├── ONNX
├── TensorRT
├── Jetson
├── FP16 / INT8
├── Profiling
└── Real-time pipelines

Engineering
├── Git/GitHub
├── Docker
├── Linux
├── Testing
├── Logging
├── Benchmarking
└── CI basics
```

------------------------------------------------------------------------

# 2. Why this path is strong for defence/UAV jobs

Current defence/autonomy work publicly lists capabilities such as: - 3D
environment perception - obstacle avoidance - autonomous event
detection - autonomous navigation - precise localization - target/object
identification - vision-based autonomous navigation - edge AI -
motion/path planning - computer vision perception

DRDO's current technology-foresight material explicitly lists these
areas under autonomous systems and robotics.

Recent UAV/defence job descriptions also show the practical combination
employers want: - OpenCV - YOLO - Jetson/CUDA - camera/ISP knowledge -
Python/C++ - ROS/ROS 2 - visual localization / SLAM / VIO - EO/IR
imagery - sensor fusion - ONNX/TensorRT - PX4/ArduPilot/MAVLink -
embedded deployment

Therefore this roadmap deliberately goes beyond ordinary deep-learning
courses.

------------------------------------------------------------------------

# 3. Your 90-day learning architecture

  Phase         Days Main goal
  --------- -------- -----------------------------------------
  Phase 0       1--3 Environment + mathematics refresh
  Phase 1      4--14 Classical Computer Vision + OpenCV
  Phase 2     15--28 Deep Learning for Vision
  Phase 3     29--42 Detection + Segmentation + Tracking
  Phase 4     43--55 Geometry + 3D Vision + Localization
  Phase 5     56--65 Robotics + ROS 2 + SLAM + Sensor Fusion
  Phase 6     66--74 PX4 + Gazebo + Drone Autonomy
  Phase 7     75--82 Edge AI + CUDA + ONNX + TensorRT
  Phase 8     83--87 Defence-grade capstone
  Phase 9     88--90 Portfolio + interview + applications

------------------------------------------------------------------------

# 4. Daily schedule

## Monday--Friday: 2.5 to 3 hours

``` text
45 min  → theory/video
60 min  → implementation from scratch
30 min  → project work
20 min  → hard homework
15 min  → notes + Git commit
```

Do not spend 3 hours watching videos.

**Rule: 30--40% learning, 60--70% building.**

## Saturday: 5--7 hours

``` text
1 h     → theory
2 h     → implementation
3 h     → project
1 h     → debugging / documentation / GitHub
```

## Sunday: 4--6 hours

``` text
1 h     → revision
2–3 h   → project
1 h     → interview questions
1 h     → research paper / experiment / documentation
```

------------------------------------------------------------------------

# 5. Non-negotiable rules

1.  **Implement important algorithms yourself before using libraries.**
2.  Every week must produce something runnable.
3.  Every project must have quantitative metrics.
4.  Every project must have a README.
5.  Every project must contain failure cases.
6.  Every model must be benchmarked for FPS/latency where applicable.
7.  Keep a `research_notes/` folder.
8.  Read at least one paper or technical article every week.
9.  Push code to GitHub at least 5 days/week.
10. Record a short demo video for every major project.
11. Do not copy-paste tutorials without changing the experiment.
12. Learn enough C++ to read/write robotics and performance-critical
    code.
13. Learn Linux because drone/robotics environments are heavily
    Linux-oriented.
14. Learn deployment, not only model training.

------------------------------------------------------------------------

# 6. Hardware strategy --- no drone required

You do **not** need to buy a drone for this roadmap.

Use:

``` text
Laptop GPU
    ↓
OpenCV / PyTorch
    ↓
Datasets
    ↓
Gazebo simulation
    ↓
PX4 SITL
    ↓
ROS 2
    ↓
Virtual camera / IMU / GPS
    ↓
Perception + navigation
```

For edge deployment practice:

``` text
Laptop
 ↓
ONNX
 ↓
TensorRT
 ↓
benchmark
 ↓
Jetson concepts
```

If you later get access to Jetson hardware, the same pipeline transfers.

------------------------------------------------------------------------

# 7. Project portfolio

You will build **5 serious projects**.

## Project 1 --- Real-Time Aerial Perception Benchmark

**Days:** 4--14

Build: - image preprocessing - classical CV baselines - edge detection -
morphology - contour analysis - optical flow - feature detection -
camera calibration - performance benchmark

Deliverables: - Python package - CLI - benchmark CSV - visual outputs -
README - tests

------------------------------------------------------------------------

## Project 2 --- Aerial Object Detection + Tracking System

**Days:** 15--42

Build:

``` text
Video
 ↓
YOLO detector
 ↓
confidence filtering
 ↓
NMS
 ↓
ByteTrack/BoT-SORT-style tracking
 ↓
trajectory history
 ↓
FPS + latency monitor
 ↓
event logging
```

Use aerial/surveillance/search-and-rescue style datasets.

Add: - small-object evaluation - day/night experiment - motion blur
experiment - low-resolution experiment - false-positive analysis -
precision/recall/F1/mAP - ID switches - FPS

------------------------------------------------------------------------

## Project 3 --- Visual Localization / Mini-VIO Lab

**Days:** 43--65

Build a research-style system that demonstrates:

``` text
Camera frames
    ↓
Feature detection
    ↓
Feature matching
    ↓
Essential/Fundamental matrix
    ↓
Pose estimation
    ↓
Triangulation
    ↓
IMU simulation/data
    ↓
Kalman filtering
    ↓
Estimated trajectory
```

Do not claim it is production VIO unless it is validated properly.

Deliver: - estimated camera trajectory - ground truth comparison -
trajectory error - failure-case analysis

------------------------------------------------------------------------

## Project 4 --- Autonomous Drone Perception in Simulation

**Days:** 66--82

Build:

``` text
PX4 SITL
   ↕
ROS 2
   ↕
Gazebo
   ↓
Virtual camera
   ↓
CV perception
   ↓
Object/marker detection
   ↓
State machine
   ↓
Offboard navigation
```

Safe project scope: - visual landing-marker detection - obstacle
avoidance simulation - waypoint navigation - search-and-rescue
simulation - visual tracking - autonomous inspection route

------------------------------------------------------------------------

## Project 5 --- Defence-Oriented Edge Vision Platform

**Days:** 83--90

Build a complete simulated edge-perception platform:

``` text
Camera/video
    ↓
YOLO
    ↓
Tracking
    ↓
Threat/event classification
    ↓
Telemetry
    ↓
FastAPI
    ↓
Dashboard
```

Add: - ONNX - TensorRT where available - latency/FPS benchmarks -
logging - Docker - configurable thresholds - health endpoint - model
versioning - test suite

Safe use cases: - perimeter monitoring - unauthorized vehicle/person
detection - search-and-rescue object detection - infrastructure
inspection - disaster-area monitoring

------------------------------------------------------------------------

# 8. PHASE 0 --- DAYS 1--3

# Setup + Mathematics

## Day 1 --- Environment

### Learn

-   Linux basics
-   Python virtual environments
-   Git
-   GitHub
-   OpenCV installation
-   PyTorch installation
-   CUDA vs CPU concept
-   VS Code
-   Jupyter

### Build

Create:

``` text
cv-drone-roadmap/
├── phase01/
├── phase02/
├── phase03/
├── projects/
├── datasets/
├── research_notes/
├── benchmarks/
├── scripts/
└── README.md
```

### Homework

Create one script that: - reads an image - prints dimensions - converts
BGR → RGB - saves grayscale - calculates mean/std - displays histogram

------------------------------------------------------------------------

## Day 2 --- Linear Algebra

### Learn

-   vectors
-   matrices
-   matrix multiplication
-   transpose
-   inverse
-   eigenvalues/eigenvectors
-   dot product
-   cross product
-   norms

### Practice

Implement: - matrix multiplication - vector normalization - cosine
similarity - 2D rotation matrix

### Homework

Rotate a set of 2D points by arbitrary angles without OpenCV.

------------------------------------------------------------------------

## Day 3 --- Probability + Optimization

### Learn

-   mean
-   variance
-   Gaussian
-   conditional probability
-   likelihood
-   gradients
-   gradient descent
-   loss functions

### Homework

Implement linear regression from scratch using NumPy.

------------------------------------------------------------------------

# 9. PHASE 1 --- DAYS 4--14

# Classical Computer Vision

## Day 4 --- Pixels + Color

Learn: - RGB/BGR - HSV - grayscale - bit depth - normalization - image
tensors

Homework: - build RGB/HSV visualizer - compare object segmentation in
RGB vs HSV

------------------------------------------------------------------------

## Day 5 --- Image Filtering

Learn: - convolution - kernels - Gaussian blur - median filter -
bilateral filter - sharpening

Homework: Implement convolution from scratch.

------------------------------------------------------------------------

## Day 6 --- Edges

Learn: - Sobel - Scharr - Laplacian - Canny - gradient magnitude

Homework: Build an edge detector comparison tool.

------------------------------------------------------------------------

## Day 7 --- Morphology

Learn: - erosion - dilation - opening - closing - morphological
gradient - connected components

Homework: Remove noise from binary aerial imagery.

------------------------------------------------------------------------

## Day 8 --- Thresholding

Learn: - global threshold - adaptive threshold - Otsu - contour
detection

Homework: Detect objects in difficult lighting.

------------------------------------------------------------------------

## Day 9 --- Contours

Learn: - contour hierarchy - area - perimeter - bounding boxes - convex
hull - polygon approximation

Homework: Create an object-shape classifier.

------------------------------------------------------------------------

## Day 10 --- Feature Detection

Learn: - Harris - Shi-Tomasi - FAST - ORB

Homework: Compare feature counts under: - blur - rotation - scale -
illumination change

------------------------------------------------------------------------

## Day 11 --- Feature Matching

Learn: - descriptor - Hamming distance - brute-force matcher - ratio
test - homography - RANSAC

Homework: Build image matching between two aerial images.

------------------------------------------------------------------------

## Day 12 --- Optical Flow

Learn: - motion field - Lucas-Kanade - sparse optical flow - dense
optical flow - tracking points

Homework: Track motion in a drone-like video.

------------------------------------------------------------------------

## Day 13 --- Camera Calibration

Learn: - intrinsic matrix - extrinsic parameters - distortion -
radial/tangential distortion - checkerboard calibration

Homework: Calibrate a webcam.

Measure reprojection error.

------------------------------------------------------------------------

## Day 14 --- PROJECT 1

Finish the **Aerial Perception Benchmark**.

Minimum benchmark:

  Algorithm        Accuracy/Quality      FPS Failure cases
  -------------- ------------------ -------- ---------------
  Canny                      record   record record
  ORB                        record   record record
  Optical Flow               record   record record

### Interview test

Explain: - convolution - Canny - ORB - homography - RANSAC - camera
calibration - optical flow

without notes.

------------------------------------------------------------------------

# 10. PHASE 2 --- DAYS 15--28

# Deep Learning for Computer Vision

## Day 15 --- Neural Network Refresh

Learn: - neurons - activation - forward pass - backpropagation -
optimization

Homework: Implement a tiny neural network using NumPy.

------------------------------------------------------------------------

## Day 16 --- CNN

Learn: - convolution - stride - padding - pooling - receptive field -
feature maps

Homework: Draw the tensor dimensions through a CNN manually.

------------------------------------------------------------------------

## Day 17 --- PyTorch

Learn: - tensors - Dataset - DataLoader - transforms - training loop -
validation loop

Homework: Write a training loop without copying a tutorial.

------------------------------------------------------------------------

## Day 18 --- CNN Classification

Build: - training - validation - confusion matrix - precision - recall -
F1

Homework: Train an aerial image classifier.

------------------------------------------------------------------------

## Day 19 --- Data Augmentation

Learn: - crop - rotate - flip - color jitter - blur - noise - affine
transforms

Homework: Run an ablation:

``` text
No augmentation
vs
Basic augmentation
vs
Aggressive augmentation
```

------------------------------------------------------------------------

## Day 20 --- Transfer Learning

Learn: - pretrained weights - feature extraction - fine-tuning -
freezing layers

Homework: Compare: - training from scratch - transfer learning

------------------------------------------------------------------------

## Day 21 --- Overfitting

Learn: - train/validation leakage - dropout - weight decay - early
stopping - learning rate

Homework: Intentionally overfit a small dataset and then fix it.

------------------------------------------------------------------------

## Day 22 --- Metrics

Learn: - confusion matrix - precision - recall - F1 - ROC - PR curve -
calibration

Homework: Explain why accuracy is dangerous for imbalanced surveillance
datasets.

------------------------------------------------------------------------

## Day 23 --- Object Detection Theory

Learn: - classification vs localization - bounding boxes - IoU - NMS -
anchor-based vs anchor-free

Homework: Implement IoU and NMS yourself.

------------------------------------------------------------------------

## Day 24 --- YOLO

Learn: - YOLO architecture concept - detection head - confidence - class
score - NMS - inference pipeline

Homework: Run YOLO on an aerial dataset.

------------------------------------------------------------------------

## Day 25 --- Custom YOLO Dataset

Learn: - dataset structure - annotation formats - train/val/test split -
class imbalance

Homework: Create a small custom dataset.

------------------------------------------------------------------------

## Day 26 --- Train Detector

Train: - baseline YOLO - evaluate mAP - inspect false positives -
inspect false negatives

Homework: Write a model evaluation report.

------------------------------------------------------------------------

## Day 27 --- Small Object Detection

Learn: - image resolution - tiling - multi-scale training -
augmentation - feature pyramids

Homework: Compare native-resolution vs tiled inference.

------------------------------------------------------------------------

## Day 28 --- Research Day

Read one object-detection paper.

Produce: - 1-page summary - architecture diagram - strengths -
weaknesses - possible aerial application

------------------------------------------------------------------------

# 11. PHASE 3 --- DAYS 29--42

# Detection + Segmentation + Tracking

## Day 29 --- Advanced Detection

Learn: - confidence threshold - NMS threshold - class imbalance - hard
negatives

Homework: Perform threshold sweep and plot precision/recall.

------------------------------------------------------------------------

## Day 30 --- Segmentation

Learn: - semantic segmentation - instance segmentation - masks - Dice -
IoU

Homework: Build a segmentation baseline.

------------------------------------------------------------------------

## Day 31 --- U-Net

Learn: - encoder - decoder - skip connections

Homework: Implement a small U-Net in PyTorch.

------------------------------------------------------------------------

## Day 32 --- Instance Segmentation

Learn: - Mask R-CNN concept - YOLO segmentation concept

Homework: Compare boxes vs masks for aerial objects.

------------------------------------------------------------------------

## Day 33 --- Tracking Fundamentals

Learn: - tracking-by-detection - data association - track lifecycle -
track IDs

Homework: Build centroid tracking.

------------------------------------------------------------------------

## Day 34 --- Kalman Filter

Learn: - state - prediction - measurement - covariance - update

Homework: Track a moving object using your own Kalman filter.

------------------------------------------------------------------------

## Day 35 --- Hungarian Algorithm

Learn: - cost matrix - assignment problem - data association

Homework: Implement Hungarian assignment or use SciPy after
understanding the algorithm.

------------------------------------------------------------------------

## Day 36 --- SORT

Learn: - detector + Kalman filter + assignment

Homework: Build a SORT-style tracker.

------------------------------------------------------------------------

## Day 37 --- Modern MOT

Learn: - ByteTrack concept - BoT-SORT concept - appearance features -
occlusion

Homework: Compare simple tracker vs modern tracker.

------------------------------------------------------------------------

## Day 38 --- Tracking Metrics

Learn: - IDF1 - MOTA - ID switches - track fragmentation

Homework: Create tracking evaluation report.

------------------------------------------------------------------------

## Day 39 --- Aerial Tracking Challenges

Learn: - camera motion - scale changes - small objects - occlusion -
blur - compression

Homework: Stress-test tracker under 5 corruptions.

------------------------------------------------------------------------

## Day 40 --- Real-Time Optimization

Learn: - batching - frame skipping - asynchronous pipelines - queues -
CPU/GPU bottlenecks

Homework: Reach the highest FPS possible on your laptop.

------------------------------------------------------------------------

## Day 41 --- Project 2 Integration

Build:

``` text
Video
 ↓
YOLO
 ↓
Tracker
 ↓
Trajectory
 ↓
Metrics
 ↓
Event logger
```

------------------------------------------------------------------------

## Day 42 --- Project 2 Release

Release:

**Aerial Object Detection + Multi-Object Tracking Platform**

README must include: - architecture - dataset - metrics - FPS -
latency - failure cases - demo - installation - model card

------------------------------------------------------------------------

# 12. PHASE 4 --- DAYS 43--55

# Geometry + 3D Vision + Localization

## Day 43 --- Coordinate Systems

Learn: - world frame - camera frame - body frame - homogeneous
coordinates

Homework: Implement coordinate transformations.

------------------------------------------------------------------------

## Day 44 --- Projective Geometry

Learn: - pinhole camera - projection - homogeneous coordinates -
perspective transformation

Homework: Project 3D points into a synthetic camera.

------------------------------------------------------------------------

## Day 45 --- Epipolar Geometry

Learn: - fundamental matrix - essential matrix - epipolar constraint

Homework: Estimate F and E from two images.

------------------------------------------------------------------------

## Day 46 --- Pose Estimation

Learn: - PnP - RANSAC-PnP - rotation - translation

Homework: Estimate camera pose from known 3D/2D points.

------------------------------------------------------------------------

## Day 47 --- Triangulation

Learn: - stereo geometry - triangulation - depth

Homework: Reconstruct 3D points from two views.

------------------------------------------------------------------------

## Day 48 --- Stereo Vision

Learn: - stereo cameras - disparity - depth map - rectification

Homework: Generate a depth map.

------------------------------------------------------------------------

## Day 49 --- Feature Matching for Localization

Learn: - SIFT - ORB - learned feature concepts - robust matching

Homework: Build image-to-image localization.

------------------------------------------------------------------------

## Day 50 --- Visual Odometry

Learn: - frame-to-frame motion - feature tracks - essential matrix -
pose accumulation

Homework: Estimate trajectory from a video.

------------------------------------------------------------------------

## Day 51 --- SLAM Concepts

Learn: - localization - mapping - loop closure - pose graph - landmarks

Homework: Draw a full SLAM pipeline from memory.

------------------------------------------------------------------------

## Day 52 --- VIO

Learn: - camera + IMU - inertial measurements - scale - drift -
synchronization

Homework: Explain why camera-only systems drift.

------------------------------------------------------------------------

## Day 53 --- Kalman Filtering

Learn: - state-space models - process noise - measurement noise -
covariance

Homework: Implement a 1D and 2D Kalman filter.

------------------------------------------------------------------------

## Day 54 --- Sensor Fusion

Learn: - GPS + IMU - camera + IMU - complementary filtering - EKF
concept

Homework: Fuse simulated noisy GPS and IMU.

------------------------------------------------------------------------

## Day 55 --- Project 3

Build:

**Visual Localization / Mini-VIO Lab**

Output: - trajectory plot - error plot - estimated pose - feature
matches - failure analysis

------------------------------------------------------------------------

# 13. PHASE 5 --- DAYS 56--65

# Robotics + ROS 2

## Day 56 --- C++ for Robotics

Learn: - references - pointers - classes - structs - STL - smart
pointers - CMake

Homework: Rewrite a small OpenCV pipeline in C++.

------------------------------------------------------------------------

## Day 57 --- Linux Robotics

Learn: - processes - permissions - bash - SSH - environment variables -
package management

Homework: Create a bash script that launches your CV pipeline.

------------------------------------------------------------------------

## Day 58 --- ROS 2 Fundamentals

Learn: - nodes - topics - messages - publishers - subscribers

Homework: Build: - camera publisher - CV subscriber

------------------------------------------------------------------------

## Day 59 --- Services + Actions

Learn: - services - actions - parameters - launch files

Homework: Create a configurable perception node.

------------------------------------------------------------------------

## Day 60 --- TF2

Learn: - coordinate transforms - static transforms - dynamic transforms

Homework: Create:

``` text
map
 ↓
base_link
 ↓
camera_link
```

------------------------------------------------------------------------

## Day 61 --- ROS 2 + OpenCV

Build: - camera topic - OpenCV node - detection output topic

Homework: Publish bounding boxes as ROS messages.

------------------------------------------------------------------------

## Day 62 --- Gazebo

Learn: - simulation - sensors - camera - IMU - physics

Homework: Create a simulated robot with camera.

------------------------------------------------------------------------

## Day 63 --- SLAM in ROS 2

Learn: - mapping - localization - scan matching - navigation concepts

Homework: Run a basic simulated SLAM experiment.

------------------------------------------------------------------------

## Day 64 --- ROS 2 Architecture

Learn:

``` text
sensor
 ↓
perception
 ↓
state estimation
 ↓
planning
 ↓
control
```

Homework: Design the architecture for an autonomous inspection drone.

------------------------------------------------------------------------

## Day 65 --- Robotics Integration Test

Create one ROS 2 project with: - camera - perception - TF - logging -
launch file - Docker option

------------------------------------------------------------------------

# 14. PHASE 6 --- DAYS 66--74

# PX4 + Drone Simulation

## Day 66 --- Drone Fundamentals

Learn: - quadrotor - attitude - position - velocity - altitude - flight
controller - companion computer

Homework: Explain the drone control loop.

------------------------------------------------------------------------

## Day 67 --- PX4

Learn: - PX4 architecture - SITL - parameters - flight modes

Homework: Run PX4 SITL.

------------------------------------------------------------------------

## Day 68 --- Gazebo + PX4

Learn: - simulated sensors - simulated camera - world files - vehicle
models

Homework: Fly a simulated drone through waypoints.

------------------------------------------------------------------------

## Day 69 --- ROS 2 + PX4

Learn: - ROS 2/PX4 bridge - topics - QoS - offboard concepts

Homework: Send position setpoints from ROS 2.

------------------------------------------------------------------------

## Day 70 --- Coordinate Frames

Learn: - NED - ENU - FLU - frame conversions

Homework: Implement and test frame conversion.

------------------------------------------------------------------------

## Day 71 --- Vision Pipeline

Build:

``` text
Gazebo camera
 ↓
ROS 2
 ↓
OpenCV/YOLO
 ↓
Detection
 ↓
State machine
```

Homework: Detect a visual marker/object.

------------------------------------------------------------------------

## Day 72 --- Visual Landing Simulation

Build a safe precision-landing simulation using a visual marker.

Learn: - visual error - target center - state machine - safety timeout

------------------------------------------------------------------------

## Day 73 --- Obstacle Avoidance

Learn: - depth - obstacle regions - free-space concepts - reactive
avoidance

Homework: Create a simulated obstacle field and generate safe avoidance
commands.

------------------------------------------------------------------------

## Day 74 --- Project 4 Release

Release:

**Autonomous UAV Perception + Navigation Simulation**

Include: - PX4 - ROS 2 - Gazebo - camera - perception - state machine -
metrics - demo video

PX4's official material includes a current precision-landing tutorial
using PX4 + ROS 2 + OpenCV + Gazebo, making it an especially useful
reference for this phase.

------------------------------------------------------------------------

# 15. PHASE 7 --- DAYS 75--82

# Edge AI + CUDA + TensorRT

## Day 75 --- GPU Fundamentals

Learn: - CPU vs GPU - parallelism - CUDA concept - memory transfer

Homework: Benchmark CPU vs GPU tensor operations.

------------------------------------------------------------------------

## Day 76 --- CUDA

Learn: - kernels - threads - blocks - grids - memory hierarchy

Homework: Implement a simple CUDA vector operation if your environment
supports CUDA.

------------------------------------------------------------------------

## Day 77 --- ONNX

Learn: - model export - computational graph - operators - dynamic shapes

Homework: Export your detector to ONNX.

------------------------------------------------------------------------

## Day 78 --- TensorRT

Learn: - engine - optimization profiles - FP32 - FP16 - INT8 concept

Homework: Benchmark: - PyTorch - ONNX - TensorRT where available

------------------------------------------------------------------------

## Day 79 --- Jetson Concepts

Learn: - ARM - Jetson - CUDA cores - memory constraints - camera
pipelines

Homework: Design how your project would run on Jetson Orin Nano.

------------------------------------------------------------------------

## Day 80 --- Real-Time Pipeline

Learn: - GStreamer concept - asynchronous processing - queues -
batching - zero-copy concept

Homework: Design a low-latency video inference architecture.

------------------------------------------------------------------------

## Day 81 --- Profiling

Measure: - preprocessing - inference - postprocessing - tracking - total
latency

Homework: Create a latency breakdown table.

------------------------------------------------------------------------

## Day 82 --- Edge AI Benchmark

Final benchmark:

  Pipeline     FPS   Latency   Model size   Accuracy
  ---------- ----- --------- ------------ ----------
  PyTorch                                 
  ONNX                                    
  TensorRT                                

------------------------------------------------------------------------

# 16. PHASE 8 --- DAYS 83--87

# Defence-Oriented Capstone

## Day 83 --- System Design

Design:

``` text
Camera
 ↓
Preprocessing
 ↓
Detector
 ↓
Tracker
 ↓
Event classifier
 ↓
Telemetry
 ↓
FastAPI
 ↓
Dashboard
```

Requirements: - configuration - logging - health check - model version -
metrics

------------------------------------------------------------------------

## Day 84 --- Build API

Create FastAPI endpoints:

``` text
GET /health
GET /model
GET /metrics
POST /infer
POST /stream/start
POST /stream/stop
```

------------------------------------------------------------------------

## Day 85 --- Event Engine

Safe events: - person detected - vehicle detected - object enters
restricted region - abandoned object - crowd increase - infrastructure
anomaly

Homework: Implement configurable zones.

------------------------------------------------------------------------

## Day 86 --- Docker + Testing

Add: - Dockerfile - docker-compose - pytest - logging - configuration -
model checksum/version

------------------------------------------------------------------------

## Day 87 --- Benchmark + Failure Analysis

Test: - low light - blur - compression - small objects - camera motion -
occlusion - false positives

Produce a technical report.

------------------------------------------------------------------------

# 17. PHASE 9 --- DAYS 88--90

# Job Launch

## Day 88 --- Resume

Create a one-page CV focused on:

``` text
Computer Vision
Robotics
UAV autonomy
Edge AI
ROS 2
PX4
OpenCV
PyTorch
YOLO
Tracking
SLAM/VIO
ONNX/TensorRT
CUDA
C++
```

Do not list 50 technologies you cannot explain.

------------------------------------------------------------------------

## Day 89 --- Interview Day

Prepare:

### Computer Vision

-   convolution
-   Canny
-   ORB/SIFT
-   homography
-   RANSAC
-   calibration
-   optical flow
-   stereo
-   PnP
-   epipolar geometry

### Deep Learning

-   CNN
-   transfer learning
-   augmentation
-   IoU
-   NMS
-   mAP
-   precision/recall
-   overfitting

### Tracking

-   Kalman filter
-   Hungarian algorithm
-   SORT
-   ByteTrack
-   IDF1/MOTA

### Robotics

-   ROS 2
-   TF2
-   SLAM
-   VIO
-   EKF
-   coordinate frames

### Drone

-   PX4
-   SITL
-   Gazebo
-   MAVLink concepts
-   offboard control
-   companion computer

### Deployment

-   ONNX
-   TensorRT
-   CUDA
-   Jetson
-   FPS
-   latency
-   profiling

------------------------------------------------------------------------

## Day 90 --- Job Attack

Apply to:

``` text
Computer Vision Engineer
Perception Engineer
Robotics Engineer
UAV AI Engineer
Drone AI Engineer
Edge AI Engineer
AI Research Engineer
Autonomy Engineer
Computer Vision Intern
Robotics Intern
Defence AI Engineer
Aerospace AI Engineer
Remote Sensing AI Engineer
```

Target: - defence startups - UAV companies - aerospace companies -
robotics companies - satellite/remote-sensing companies - defence
electronics companies - DRDO labs/JRF/internship routes - government R&D
organizations - research labs

Do not wait until Day 90 to apply.

Start applications around **Day 35--45**.

------------------------------------------------------------------------

# 18. Weekly research habit

Every Sunday:

1.  Pick one recent paper.
2.  Read abstract.
3.  Understand the problem.
4.  Understand architecture.
5.  Identify dataset.
6.  Identify metric.
7.  Identify limitation.
8.  Reproduce one small experiment.
9.  Write one page.

Recommended paper areas: - object detection - multi-object tracking -
visual odometry - SLAM - VIO - visual localization - aerial object
detection - small-object detection - edge inference - sensor fusion -
remote sensing

------------------------------------------------------------------------

# 19. YouTube / video resource map

Use the videos as **learning accelerators**, not as substitutes for
implementation.

## A. Deep Computer Vision

### Stanford CS231n

Use for: - CNNs - image classification - optimization - deep learning
for vision - detection concepts

Video: https://www.youtube.com/watch?v=2fq9wYslV0A

The Spring 2025 Stanford lecture is a strong current reference and links
to the full CS231n playlist.

### Search playlist

https://www.youtube.com/results?search_query=Stanford+CS231n+Spring+2025+computer+vision

------------------------------------------------------------------------

## B. OpenCV

### Camera Calibration with OpenCV

https://www.youtube.com/watch?v=KGeRoScMs6Q

Use for: - camera calibration - distortion - checkerboards -
reprojection error

### Optical Flow

https://www.youtube.com/watch?v=hfXMw2dQO4E

Use for: - Lucas-Kanade - sparse optical flow - object tracking -
trajectories

### OpenCV learning search

https://www.youtube.com/results?search_query=OpenCV+computer+vision+full+course+Python

------------------------------------------------------------------------

## C. Object Detection

### YOLO / Ultralytics

https://www.youtube.com/results?search_query=Ultralytics+YOLO+object+detection+tracking+tutorial

Study: - training - custom datasets - validation - detection -
segmentation - tracking - export

Do not only learn how to run:

``` python
model.predict()
```

Learn what happens before and after inference.

------------------------------------------------------------------------

## D. Deep Learning / PyTorch

https://www.youtube.com/results?search_query=PyTorch+computer+vision+full+course

Study: - Dataset - DataLoader - transforms - training loop -
validation - transfer learning - CNNs

------------------------------------------------------------------------

## E. Robotics Mathematics

### NPTEL Kalman Filter

https://www.youtube.com/watch?v=E9QL8XWJIh8

Use for: - state estimation - prediction - update - covariance - noisy
measurements

### Robotics search

https://www.youtube.com/results?search_query=NPTEL+Introduction+to+Robotics+Kalman+filter+SLAM

------------------------------------------------------------------------

## F. ROS 2

### ROS 2 tutorials

https://www.youtube.com/results?search_query=ROS+2+full+course+Articulated+Robotics

Learn: - nodes - topics - services - actions - TF2 - launch -
parameters - packages - Nav2 concepts

------------------------------------------------------------------------

## G. PX4 + ROS 2 + Gazebo

### PX4 official precision landing tutorial

https://www.youtube.com/watch?v=ykVh8xER_1s

This is especially valuable because it demonstrates: - PX4 - ROS 2 -
OpenCV - ArUco - Gazebo - SITL - coordinate transforms -
offboard/control concepts - state-machine logic

### PX4 + ROS 2 masterclass

https://www.youtube.com/watch?v=cXdP29a-SEQ

Useful for: - PX4 architecture - ROS 2 integration - Micro XRCE-DDS -
SITL - Gazebo - offboard control - NED/ENU/FLU frames

### PX4 video search

https://www.youtube.com/results?search_query=PX4+ROS2+Gazebo+SITL+autonomous+drone

------------------------------------------------------------------------

## H. CUDA

### NVIDIA Modern CUDA C++ Programming Class

https://www.youtube.com/watch?v=Sdjn9FOkhnA

Learn: - CUDA programming - parallelism - memory - streams - kernels

### CUDA search

https://www.youtube.com/results?search_query=NVIDIA+CUDA+beginner+course+computer+vision

------------------------------------------------------------------------

## I. TensorRT / Jetson / Edge AI

TensorRT search:
https://www.youtube.com/results?search_query=NVIDIA+TensorRT+tutorial+YOLO+Jetson

Jetson search:
https://www.youtube.com/results?search_query=NVIDIA+Jetson+Orin+Nano+computer+vision+YOLO

DeepStream search:
https://www.youtube.com/results?search_query=NVIDIA+DeepStream+SDK+computer+vision+tutorial

Study: - ONNX - TensorRT - FP16 - INT8 - CUDA - profiling - GStreamer -
DeepStream

------------------------------------------------------------------------

## J. SLAM / Visual Odometry

https://www.youtube.com/results?search_query=visual+odometry+SLAM+computer+vision+course

https://www.youtube.com/results?search_query=ORB+SLAM3+tutorial+visual+SLAM

https://www.youtube.com/results?search_query=visual+inertial+odometry+VIO+tutorial+robotics

Focus on understanding the mathematics, not merely running an existing
SLAM package.

------------------------------------------------------------------------

# 20. Official/reference resources

## OpenCV

https://docs.opencv.org/

## PyTorch

https://pytorch.org/

## Ultralytics

https://docs.ultralytics.com/

## ROS 2

https://docs.ros.org/

## PX4

https://docs.px4.io/

## Gazebo

https://gazebosim.org/

## NVIDIA Jetson

https://developer.nvidia.com/embedded/jetson

## NVIDIA TensorRT

https://developer.nvidia.com/tensorrt

## NVIDIA DeepStream

https://developer.nvidia.com/deepstream-sdk

## ONNX

https://onnx.ai/

------------------------------------------------------------------------

# 21. Datasets

Start with:

### General vision

-   COCO
-   ImageNet subsets
-   CIFAR for quick experiments

### Aerial / UAV

-   VisDrone
-   UAVDT
-   DOTA
-   xView
-   Anti-UAV

### Remote sensing

-   SpaceNet
-   LoveDA

### Tracking

-   MOTChallenge datasets
-   VisDrone tracking

Dataset search:
https://www.google.com/search?q=aerial+drone+computer+vision+datasets+VisDrone+UAVDT+DOTA+xView

------------------------------------------------------------------------

# 22. GitHub repository structure

Your final portfolio should look like:

``` text
drone-computer-vision-roadmap/
│
├── classical_cv/
│   ├── filters/
│   ├── edges/
│   ├── features/
│   ├── optical_flow/
│   └── calibration/
│
├── deep_cv/
│   ├── classification/
│   ├── detection/
│   └── segmentation/
│
├── tracking/
│   ├── kalman/
│   ├── assignment/
│   └── mot/
│
├── geometry/
│   ├── calibration/
│   ├── epipolar/
│   ├── pnp/
│   ├── triangulation/
│   └── visual_odometry/
│
├── ros2/
│   ├── perception_node/
│   └── tf_demo/
│
├── px4/
│   └── autonomous_perception/
│
├── edge_ai/
│   ├── onnx/
│   ├── tensorrt/
│   └── benchmarks/
│
├── projects/
│   ├── aerial_perception/
│   ├── aerial_tracking/
│   ├── visual_localization/
│   ├── autonomous_uav/
│   └── defence_edge_vision/
│
├── research_notes/
├── benchmarks/
├── docs/
└── README.md
```

------------------------------------------------------------------------

# 23. What your final resume projects should say

Do not write:

> Made a YOLO project.

Write something closer to:

> **Real-Time Aerial Perception and Tracking System** --- Developed a
> PyTorch/YOLO-based aerial object detection and multi-object tracking
> pipeline; evaluated precision/recall/mAP and IDF1, analyzed
> small-object and camera-motion failure modes, and optimized the
> inference pipeline for real-time performance.

Second:

> **Visual Localization and Mini-VIO Research Prototype** ---
> Implemented camera calibration, feature matching, epipolar geometry,
> pose estimation, triangulation and Kalman filtering to estimate camera
> trajectory from image/IMU data and quantified trajectory error against
> reference motion.

Third:

> **Autonomous UAV Perception Simulation** --- Integrated ROS 2, PX4
> SITL and Gazebo with a computer-vision perception pipeline,
> implementing simulated visual detection, state-machine logic and
> autonomous navigation behaviors without physical drone hardware.

Fourth:

> **Edge AI Aerial Monitoring Platform** --- Exported a vision model to
> ONNX and optimized inference using TensorRT concepts, adding latency
> profiling, tracking, FastAPI telemetry, Dockerized deployment and
> failure-case benchmarking.

------------------------------------------------------------------------

# 24. Interview preparation ladder

## Level 1

You should explain: - image - pixel - convolution - CNN - YOLO - IoU -
NMS

## Level 2

You should implement: - convolution - IoU - NMS - Kalman filter -
optical flow basics - coordinate transforms

## Level 3

You should explain mathematically: - camera projection - homography -
essential matrix - fundamental matrix - PnP - triangulation

## Level 4

You should design: - object detection pipeline - tracking pipeline -
visual localization system - ROS 2 perception architecture - drone
autonomy architecture - edge inference pipeline

## Level 5

You should defend engineering decisions:

> Why YOLO?

> Why this input resolution?

> Why this tracker?

> Why not optical flow?

> Why TensorRT?

> Why FP16?

> What happens under low light?

> How do you handle false positives?

> What is your latency budget?

> How does camera motion affect tracking?

> How do you synchronize camera and IMU?

> What happens if GPS is unavailable?

> How would you deploy this on a Jetson?

> How would you test the system before flight?

------------------------------------------------------------------------

# 25. Job strategy --- start before finishing

From Day 35 onward:

``` text
Monday:
5 applications

Tuesday:
5 applications

Wednesday:
5 applications

Thursday:
5 applications

Friday:
5 applications

Saturday:
Networking + GitHub

Sunday:
Technical improvement
```

Target 20--30 quality applications/week rather than mass-applying
randomly.

Search terms:

``` text
Computer Vision Engineer UAV
Computer Vision Engineer Drone
Perception Engineer UAV
Robotics Perception Engineer
Autonomy Engineer
Visual Navigation Engineer
Drone AI Engineer
Edge AI Engineer
Computer Vision Defence
Aerospace AI Engineer
UAV ML Engineer
Robotics AI Engineer
Remote Sensing AI Engineer
EO IR Computer Vision
```

------------------------------------------------------------------------

# 26. Companies / organizations to monitor

India-focused:

-   DRDO
-   CAIR
-   DYSL-AI
-   DYSL-CT
-   NewSpace Research and Technologies
-   ideaForge
-   Garuda Aerospace
-   Zen Technologies
-   Big Bang Boom Solutions
-   GalaxEye
-   defence/aerospace startups
-   robotics startups
-   satellite/remote-sensing companies
-   counter-UAS companies

Also search: - Bengaluru - Hyderabad - Chennai - Pune - Noida - Delhi
NCR

Bengaluru is especially important for aerospace/defence/autonomy
opportunities.

------------------------------------------------------------------------

# 27. Reality check

Three months will **not** make you a senior autonomous-systems engineer.

But three months of aggressive execution can make you much stronger
for: - junior CV roles - AI internships - perception internships -
robotics internships - UAV AI internships - defence AI research
internships - entry-level edge AI roles

The differentiator is not the number of certificates.

It is:

``` text
Math
+
Computer Vision
+
Deep Learning
+
Geometry
+
Tracking
+
Robotics
+
Drone Simulation
+
Edge Deployment
+
Strong Projects
+
Interview Ability
```

That combination is much rarer than someone who only knows YOLO.

------------------------------------------------------------------------

# 28. The final target skill pyramid

``` text
                         DEFENCE / AUTONOMY AI
                                  ▲
                         System Architecture
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
               Autonomous Systems          Edge AI
                    │                           │
              ROS2 / PX4 / SLAM          CUDA / TensorRT
                    │                           │
              Sensor Fusion              Real-time CV
                    │                           │
             Visual Navigation          Detection / Tracking
                    │                           │
                    └─────────────┬─────────────┘
                                  │
                         Computer Vision
                                  │
                OpenCV + Geometry + Deep Learning
                                  │
                         Mathematics
                                  │
                    Linear Algebra + Probability
```

------------------------------------------------------------------------

# 29. The rule that will make this roadmap work

For every topic, follow:

``` text
LEARN
  ↓
IMPLEMENT FROM SCRATCH
  ↓
USE THE LIBRARY
  ↓
BREAK IT
  ↓
MEASURE IT
  ↓
OPTIMIZE IT
  ↓
DOCUMENT IT
  ↓
EXPLAIN IT IN AN INTERVIEW
```

If you follow that cycle for 90 days, your portfolio will demonstrate
**engineering ability**, not tutorial completion.
