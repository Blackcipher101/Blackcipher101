# Hi there! I'm Nehal 👋

Robotics engineer working on **underwater robotics** and **embodied AI**: state estimation and SLAM that survive
murky water, perception and vision-language models that turn sensor data into decisions, and learned controllers
trained in simulation. 🌊🤖

## What I do 🛠️

- **State estimation & SLAM**: visual-inertial, lidar-inertial and DVL/pressure fusion; factor graphs (GTSAM),
  fixed-lag smoothing, localization and relocalization on real robots.
- **GPU acceleration**: CUDA front ends and planners, profiling and latency work on desktop GPUs and Jetson Orin.
- **Planning & control**: MPPI and sampling-based control, Nav2, route planning.
- **Perception & VLMs**: detection and segmentation (YOLO, OWLv2, SAM), vision-language models for inspection
  reports and task planning.
- **Embodied AI / RL**: training locomotion and vehicle-control policies in MuJoCo (MJX + PPO), sim-to-real minded.
- **Simulation**: Stonefish (underwater), Gazebo, MuJoCo.

## Current projects 🌊

Underwater stereo-inertial estimation and inspection. Each repo has measured baselines; all runs are offline on recorded data or in simulation.

| Project | What it does | Baseline result |
|---|---|---|
| [uw-vio-dvl](https://github.com/Blackcipher101/uw-vio-dvl) | Stereo-inertial-pressure VIO (GTSAM fixed-lag) with a tightly coupled DVL factor that survives DVL dropouts | 20 s camera blackout: ATE 3.88 m → 0.66 m with (simulated) DVL |
| [uw-gpu-klt](https://github.com/Blackcipher101/uw-gpu-klt) | CUDA KLT stereo front end, drop-in for the CPU tracker | 2.0x (RTX 5080 desktop) / 4.9x (laptop) faster front end, no ATE loss |
| [uw-inspect-report](https://github.com/Blackcipher101/uw-inspect-report) | Detector + vision-language model that drafts an inspection report from video and poses, with faithfulness checks | context verifier confirms 8/8 true findings, precision 0.89 |
| [uw-calib-health](https://github.com/Blackcipher101/uw-calib-health) | In-water stereo calibration health check | every ≥ 0.2° change detected, 0 false alarms |
| [uw-vslam-bench](https://github.com/Blackcipher101/uw-vslam-bench) | Shared benchmark harness + two honest negative results (learned failure warning, sonar-in-camera) | — |

In progress:
- 🦾 **Humanoid RL in MuJoCo**: walking, getting up, backflips; DeepMimic-style motion imitation.
- 🚤 **RL controller for an ROV**: MuJoCo fluid model, station keeping and trajectory tracking under currents, compared against PID.
- 🐟 **Stonefish underwater simulation benchmark** for the VIO + DVL estimator.

## Previously 🚗

- **Head of Planning and Prediction, Minus Zero**: autonomous mobility. I joined as one of the first engineers (Research Engineer, Autonomy)
  and worked on some of the hardest problem statements in the stack.
- **Computer Vision Intern, Clutterbot**: localised bins for a New Zealand client and cut build time.

I have a background in Schrödinger's states and cognitive computation, and still find the multiverse and multitasking suspiciously similar. 🤔

## Contact 📬

Email me at nehalnevle@gmail.com about opportunities or collaborations. 📩
