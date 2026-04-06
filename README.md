# Awesome Works of RL in VLA
Hi, here is a curated list of tech report, research papers, datasets, benchmarks, insights, toolkits and resources related to World Models and Reinforcement Learning (RL) in Visual Language Agents (VLA)!

Note that,

- 🎯🤖 The focus will especially be on the domain of embodied AI and Robotics.
- ✍️🧑‍🤝‍🧑 Notes on our main focus will be linked, and any discussions or contributions are highly welcome [here](#contact)!
- 🔥🌟 We are updating! **Star** us to get notified of the latest updates!

## Table of Contents
- [Paper](#paper)
    - [Paper Stage - Main Focus (w.r.t. the Industry)](#paper-stage)
        - [1 World Models](#1-world-models)
        - [2 RL](#2-rl)
    - [Paper Scope - A Broader Horizon (w.r.t. the Community)](#paper-scope)
        - [World Models](#world-models)
        - [RL](#rl)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Toolkits & Projects](#toolkits--projects)
    - [Implementations of RL Algorithms](#implementations-of-rl-algorithms)
- [Pool of Works - To be Shared](#pool-of-works)
- [Insights of the field](#insights-of-the-field)
- [Reference Materials](#reference-materials)

## Paper

### Paper Stage

#### 1 World Models

| # | Paper Title | Date | Key Take-aways | Company/Institute | Notes |
| -- | --------------- | --------- | ----------------- | --------- | ---- |
| 01 | <details><summary>Causal World Modeling</summary>for Robot Control | Jan 2026 | LingBot-VA | 蚂蚁灵波 (Bobbyant) |  |
| 02 | <details><summary>Genie Envisioner (GE)</summary>: A Unified World Foundation Platform for Robotic Manipulation</details> | Aug 2025 | GE-Act | 智元机器人 (AgiBot) |  |

#### 2 RL

| # | Paper Title | Date | Key Take-aways | Company/Institute | Notes |
| -- | --------------- | --------- | ----------------- | --------- | ---- |
| 01 | <details><summary>SOP</summary>: A Scalable Online Post-Training System for Vision-Language-Action Models</details> | Jan 2026 | SOP | 智元机器人 (AgiBot) | [Notes](notes/sop_260127/sop_260127.md) |
| 02 | <details><summary>GR-RL</summary>: Going Dexterous and Precise for Long-Horizon Robotic Manipulation</details> | Dec 2025 | <details><summary>GR-RL</summary> - data filter &augmentation<br>- distributional critic<br>- offline &online RL for policy training</details> | 字节跳动 (ByteDance) Seed | [Notes](notes/gr-rl_260209/notes.md) |
| 03 | <details><summary>${\pi}^{*}_{0.6}$</summary>: a VLA That Learns From Experience</details> | Nov 2025 | <details><summary>RECAP</summary>- consists of 3 steps: (1)data collection, (2)value function training and (3)advantage conditioned training.</details> | Physical Intelligence (PI) | [Notes](notes/pi0.6star_260127/Pi%2006_260127.pdf) |



### Paper Scope

#### World Models

| Paper Title | Date | Key Take-aways | Conference | Institute |
| ----------- | --------- | ----------------- | --------- | --------- |
| <details><summary>Video Prediction Policy</summary>: A Generalist Robot Policy with Predictive Visual Representations</details> | May 2025 | VPP | <details><summary>ICML</summary>- Spotlight Paper</details> | <details><summary>IIIS, Tsinghua University / Shanghai AI Lab/ Qizhi Research Institute</summary>- Jianyu Chen</details> |
| <details><summary>Robotic World Model</summary>: A Neural Network Simulator for Robust Policy Optimization in Robotics</details> | Jan 2025 | <details><summary>RWM</summary>- unfortunately, the output of RWM, i.e., the observation, is only the robot proprioceptive state; that's to say, the robot is 'blind'. </details> | <details><summary>NeurIPS</summary>- Outstanding Paper Award, Embodied World Models for Decision Making Workshop</details> | ETH Zurich |
| <details><summary>Stable Video Diffusion</summary>: Scaling Latent Video Diffusion Models to Large Datasets</details> | Nov 2023 | SVD | CVPR | Stability AI |
| <details><summary>Align your Latents</summary>: High-Resolution Video Synthesis with Latent Diffusion Models</details> | Apr 2023 | <details><summary>Video LDM</summary>- a latent diffusion model for video generation<br>- additional temporal layers are interleaved with the existing spatial layers, and only the former will be updated during training.</details> | CVPR | LMU Munich / NVIDIA |

#### RL

| Paper Title | Date | Key Take-aways | Conference | Institute |
| ----------- | --------- | ----------------- | --------- | --------- |
| <details><summary>SARM</summary>: Stage-Aware Reward Modeling for Long Horizon Robot Manipulation</details> | Oct 2025 | <details><summary>SARM /</summary>- dual reward model architecture: stage model and subtask model [[Notes](notes/sarm_260203/SARM_260203_155212.pdf)]</details>RA-BC | ICLR | Stanford University / xdof.ai |
| <details><summary>Steering Your Diffusion Policy </summary>with Latent Space Reinforcement Learning</details> | Jun 2025 | <details><summary>DSRL</summary>- simply “steers” the diffusion policy to produce desired actions by **altering its input noise distribution**.</details> | CoRL | UC Berkeley |
| <details><summary>A Distributional Perspective </summary>on Reinforcement Learning</details> | Jul 2017 | <details><summary>distributional Bellman equation</summary>- instead of using Q function to model the expectation of the return in the regular RL, it models the full distribution of returns.</details> | ICML | DeepMind |


## Datasets & Benchmarks
| # | Paper Title | Date | Platform | Models | Company/Institute | Key Take-aways |
| -- | ----------- | ------- | -------- | -------- | ------ | ----------------- |
| 01 | <details><summary>RoboReward</summary>: General-purpose Vision-Language Reward Models for Robotics</details> | Jan 2026 | (N) | RoboReward 4B / 8B | <details><summary>UC Berkeley / Stanford University</summary>- Sergey Levine / Chelsea Finn</details> | [Notes](notes/roboreward_260202/notes.md) |
| 02 | <details><summary>RoboArena</summary>: Distributed Real-World Evaluation of Generalist Robot Policies</details> | Nov 2025 | <details><summary>DROID Robot Platform</summary>- consists of a Franka Panda 7DoF robot arm, two adjustable Zed 2 stereo cameras, a wristmounted Zed Mini stereo camera, and an Oculus Quest 2 headset with controllers for teleoperation (refer to [here](https://droid-dataset.github.io/))</details> | (N) | <details><summary>UC Berkeley / Stanford University</summary>- Chelsea Finn / Sergey Levine</details> | <details><summary>distributed real-world policy evaluation</summary>- aggregates a large number of such pairwise, double-blind comparisons into a global policy ranking.</details> |
| 03 | <details><summary>Open X-Embodiment (OXE)</summary>: Robotic Learning Datasets and RT-X Models</details> | Since Oct 2023 | <details><summary>Multi</summary>- 22 different robotic embodiments from 21 different institutions</details> | RT-1-X / RT-2-X | DeepMind | <details><summary>1M+ real robot trajectories</summary>- constructed by pooling 60 existing robot datasets from 34 robotic research labs and converting them all into RLDS data format.</details> |


## Toolkits & Projects

### Implementations of RL Algorithms

| RL Platform                                                        | Documentation                                                                                                                                                        | Code Coverage                                                                                                                                                | PyTorch support   | Tensorboard support  | Last Update                                                                                                       |
| ------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------ | ------------------ | ----------------------------------------------------------------------------------------------------------------- |
| [Stable-Baselines3](https://github.com/DLR-RM/stable-baselines3)   | [![Documentation Status](https://readthedocs.org/projects/stable-baselines/badge/?version=master)](https://stable-baselines3.readthedocs.io/en/master/?badge=master) | [![coverage report](https://gitlab.com/araffin/stable-baselines3/badges/master/coverage.svg)](https://gitlab.com/araffin/stable-baselines3/-/commits/master) | :heavy_check_mark: | :heavy_check_mark: | ![GitHub last commit](https://img.shields.io/github/last-commit/DLR-RM/stable-baselines3?label=last%20update)     |
| [Tianshou](https://github.com/thu-ml/tianshou)                     | [![Read the Docs](https://img.shields.io/readthedocs/tianshou)](https://tianshou.readthedocs.io/en/master)                                                           | [![codecov](https://img.shields.io/codecov/c/gh/thu-ml/tianshou)](https://codecov.io/gh/thu-ml/tianshou)                                                     | :heavy_check_mark: | :heavy_check_mark: | ![GitHub last commit](https://img.shields.io/github/last-commit/thu-ml/tianshou?label=last%20update)              |

<sup>*: Adapted from [source a](https://github.com/thu-ml/tianshou) and [b](https://github.com/DLR-RM/stable-baselines3), following MIT license.</sup> 

## Pool of Works

Please check [here](assets/to_be_read.md) for more information.

## Insights of the field

- H. Xu, Embodied AI: A 2025 Retrospective, Dec 2025. [[website](https://zhuanlan.zhihu.com/p/1983661736180589668)]
- Sergey Levine & Waymo, 
Robotics Startup Founder Sergey Levine is Building Robots for Your Home (and Work) | AI in Motion, Nov 2025. [[video](https://www.youtube.com/watch?v=0CfMCOzmJZI)]

## Reference Materials
- Reinforcement Learning Course by David Silver, UCL, 2015. [[slides](https://davidstarsilver.wordpress.com/teaching/)]
- ME5418: Machine Learning in Robotics by Prof Guillaume, NUS, Fall 2025 (unfortunately not publicly available yet 😢)
- Embodied-AI-Guide by TianxingChen. [[code](https://github.com/TianxingChen/Embodied-AI-Guide)]

## Contact
For any suggestions or contributions, please feel free to open an issue or submit a pull request. You are also welcome to reach out me for further questions via email at [maij@u.nus.edu](mailto:maij@u.nus.edu)!