# Hi, I'm You Youngil

Founder of **AeroRobot AI**.

I build drone, robotics, and AI systems with **Fast DDS**, **ROS 2**, **ArduPilot**, DDS Router, XRCE-DDS, video streaming, and mission-control platforms.

## Focus

- Drone autonomy and ground control systems
- GPS-denied drone navigation and inspection (LiDAR-inertial odometry, 3D reconstruction, AI crack analysis)
- DDS / RTPS communication platforms
- ROS 2, Fast DDS, DDS Router, XRCE-DDS
- ArduPilot integration and Mission Planner DDS bridge
- RTSP to DDS / WebRTC video pipelines
- Isaac Sim robotics simulation

## Featured: SmartCrackNoGps

GPS-denied drone inspection of bridge undersides — fly without GPS, rebuild the bridge in 3D, and show cracks found in the original high-resolution photos on that 3D model.

- **Localization without GPS**: FAST-LIO2 (LiDAR + IMU) ported to native Windows C++ without ROS; its live pose feeds the ArduPilot EKF as external navigation. R3LIVE and VINS-Fusion ported the same way as comparison baselines.
- **Transport**: Fast DDS end to end (XRCE-DDS Agent, DDS Router, Mission Planner over DDS) — no ROS / ROS 2 dependency.
- **3D reconstruction**: LiDAR map with photo colours and 3D Gaussian Splatting trained in our own C++/CUDA code.
- **Crack analysis**: segmentation (ONNX Runtime + DirectML) on the original photos, projected onto the LiDAR map with occlusion checks and multi-view voting; widths from image intensity profiles.
- **Inspection viewer** (C# WPF): 3D map / 3DGS / crack layers, click a point to trace back to the original photo, crack review (exclude / add missed cracks) and PDF report generation.
- **Simulation**: Isaac Sim 5.1 + ArduPilot SITL with DJI L2 (Livox pattern) and Ouster OS0 sensor models and a gimbal camera.
- **Measured in simulation**: full bridge-pier missions flown without GPS on live LiDAR-inertial pose, trajectory error (ATE) 0.02–0.11 m over ~770–790 m flights.

## Representative Projects

- **SmartCrackNoGps** — GPS-denied bridge inspection: LiDAR-inertial navigation, 3D reconstruction, crack analysis and reporting
- **ArduPilot DDS** — DDS-based communication and integration for ArduPilot systems
- **DDS WAN Platform** — DDS networking over WAN environments
- **Mission Planner DDS Bridge** — Mission Planner integration with DDS middleware
- **RTSP to DDS Video Platform** — real-time video transport through DDS and web clients
- **Isaac Sim Robotics** — robotics simulation and digital twin experiments
- **GenIDL DDS SDK** — IDL generation and DDS SDK tooling

## Technical Stack

**Languages:** C++, C#, Python, TypeScript, Bash, PowerShell  
**Middleware:** Fast DDS, DDS Router, XRCE-DDS, ROS 2, OpenDDS  
**Robotics:** ArduPilot, Mission Planner, MAVLink, Isaac Sim, FAST-LIO2, R3LIVE, VINS-Fusion  
**3D / AI:** CUDA, 3D Gaussian Splatting, ONNX Runtime, DirectML, YOLO segmentation  
**Video / Streaming:** RTSP, WebRTC, MPEG-TS  
**Platforms:** Linux, Windows, WPF, Unreal Engine, Docker

## What I Work On

I am focused on building reliable communication layers and autonomy for drones and robots:

- bridging embedded devices, ground stations, and cloud systems;
- moving telemetry, commands, sensor data, and video across DDS networks;
- flying and inspecting where GPS is not available;
- making robotics software easier to integrate, test, and deploy.

## Contact

- Email: youngil740414@gmail.com
- Website: [youngilyou.github.io](https://youngilyou.github.io)
