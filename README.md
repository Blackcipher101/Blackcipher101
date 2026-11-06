<h1 align="center">Nehal Nevle</h1>
<p align="center"><b>Robotics engineer · state estimation · SLAM · planning</b><br>
I build the software that lets robots know where they are and decide where to go next.</p>

---

### 🤖 Every embodiment, then the ocean

I work across the full robotics stack, from sensor drivers and state estimation to planning, control and
simulation. I've shipped it on almost every kind of robot:

| | Embodiment | What I built |
|---|---|---|
| 🚗 | **Autonomous cars & pods** | City-scale planning and prediction stack (50k+ lines of production C++), localization, trajectory optimization |
| 🛵 | **Two-wheelers** | Navigation and motion planning; stereo + LiDAR + IMU + GPS state estimation |
| 🐕 | **Quadrupeds** | Autonomy and localization for legged robots |
| 🌲 | **Outdoor autonomy** | Off-road and outdoor navigation, robust to GPS and vision dropouts |
| 🛡️ | **Defence** | Autonomy and secure embedded systems |
| 🔍 | **Inspection & scanners** | Inspection robots, scanning and mapping |
| 🦾 | **Manipulators & AMRs** | Perception-to-control loops for mobile manipulation |
| 🌊 | **Underwater**: *now* | VIO + DVL fusion, GPU front ends, AI inspection reports, sim-trained ROV control |

Underwater is the one embodiment I hadn't done yet, so that's where I'm working now.

### 🧠 What I specialise in

- **State estimation & SLAM**: visual-inertial, lidar-inertial, DVL/pressure fusion, factor graphs (GTSAM),
  fixed-lag smoothing, relocalization, sensor dropout handling
- **Planning & control**: path planners, trajectory optimization, MPPI, prediction, low-latency C++
- **Simulation**: built an *agentic pipeline on Unreal Engine that generates photorealistic driving simulators*
  (Minus Zero); Stonefish, Gazebo, MuJoCo
- **GPU & real-time**: CUDA perception and planning, Jetson Orin, multithreaded low-latency systems
- **Embodied AI**: RL locomotion and control policies (MJX + PPO), vision-language models for robot
  decision-making and inspection

### 🌊 Building now

| Project | What it does | Result so far |
|---|---|---|
| [uw-vio-dvl](https://github.com/Blackcipher101/uw-vio-dvl) | Stereo-inertial-pressure VIO with a tightly coupled DVL factor that survives dropouts | 20 s camera blackout: ATE **3.88 m → 0.66 m** with DVL |
| [uw-gpu-klt](https://github.com/Blackcipher101/uw-gpu-klt) | CUDA KLT stereo front end | **2.0–4.9×** faster, no accuracy loss |
| [uw-inspect-report](https://github.com/Blackcipher101/uw-inspect-report) | Detector + VLM that writes the draft inspection report | **8/8** true findings confirmed, precision 0.89 |
| [uw-calib-health](https://github.com/Blackcipher101/uw-calib-health) | In-water stereo calibration health monitor | every ≥ 0.2° drift caught, 0 false alarms |
| [uw-vslam-bench](https://github.com/Blackcipher101/uw-vslam-bench) | Benchmark harness, plus the experiments that didn't work, published honestly | — |

Next up: 🦿 **humanoids in MuJoCo** (walk, get up, backflip; DeepMimic-style imitation) and 🚤 an **RL ROV
controller** trained under currents in MuJoCo's fluid model.

### 🛤️ Path

- **Founding member, Bytes**: navigation, planning and state estimation for two-wheelers
- **Head of Planning & Prediction, Minus Zero**: led the planning stack for the ZPod autonomous vehicle
- **Founding Research Engineer, Minus Zero**: localization, planning, control, camera/LiDAR drivers
- **Perception & Localization Intern, Clutterbot**: stereo + odometry fusion, closed-loop manipulation
- **Hardware Security Engineer, Traboda**: secure embedded systems
- **B.Tech, Electrical & Computer Engineering (robotics), Amrita Vishwa Vidyapeetham**

### 🧰 Stack

`C++` `Python` `CUDA` `ROS 2` `GTSAM` `Eigen` `OpenCV` `PyTorch` `JAX` `MuJoCo` `Unreal Engine` `Gazebo` `Stonefish` `Nav2`

### 📬 Say hi

**nehalnevle@gmail.com**: always up for hard robotics problems, especially wet ones.
