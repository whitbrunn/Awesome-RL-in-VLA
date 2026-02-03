# Awesome Works of RL in VLA
Hi, here is a curated list of research papers, datasets, benchmarks and resources related to Reinforcement Learning (RL) in Visual Language Agents (VLA)!

Note that,

- The focus will especially be on the domain of embodied AI and Robotics.
- Notes on our main focus will be linked, and any discussions or contributions are highly welcome [here](#contact)!

## Table of Contents
- [Paper](#paper)
    - [Paper Stage - Main Focus (w.r.t. the Industry)](#paper-stage)
    - [Paper Scope - A Broader Horizon (w.r.t. the Community)](#paper-scope)
- [Datasets & Benchmarks](#datasets--benchmarks)
- [Pool of Works - To be Shared](#pool-of-works)
- [Reference Materials](#reference-materials)

## Paper

### Paper Stage

| # | Paper Title | Date | Key Take-aways | Company/Institute | Notes |
| -- | --------------- | --------- | ----------------- | --------- | ---- |
| 01 | <details><summary>SOP</summary>: A Scalable Online Post-Training System for Vision-Language-Action Models</details> | Jan 2026 | SOP | 智元机器人 | [Notes](notes/sop_260127/sop_260127.md) |
| 02 | <details><summary>${\pi}^{*}_{0.6}$</summary>: a VLA That Learns From Experience<details> | Nov 2025 | <details><summary>RECAP</summary>- consists of 3 steps: (1)data collection, (2)value function training and (3)advantage conditioned training.</details> | Physical Intelligence (PI) | [Notes](notes/pi0.6star_260127/Pi%2006_260127.pdf) |
| 03 | <details><summary>SARM</summary>: Stage-Aware Reward Modeling for Long Horizon Robot Manipulation</details> | Oct 2025 | <details><summary>SARM</summary>- dual reward model architecture: stage model and subtask model</details> / RA-BC | Stanford University / xdof.ai | [Notes](notes/sarm_260203/SARM_260203_155212.pdf) |


### Paper Scope
| Paper Title | Date | Key Take-aways | Conference | Institute |
| ----------- | --------- | ----------------- | --------- | --------- |
| <details><summary>A Distributional Perspective </summary>on Reinforcement Learning</details> | Jul 2017 | <details><summary>distributional Bellman equation</summary>- instead of using Q function to model the expectation of the return in the regular RL, it models the full distribution of returns.</details> | ICML | DeepMind |

## Datasets & Benchmarks
| # | Paper Title | Date | Platform | Models | Company/Institute | Key Take-aways |
| -- | ----------- | ------- | -------- | -------- | ------ | ----------------- |
| 01 | <details><summary>RoboReward</summary>: General-purpose Vision-Language Reward Models for Robotics</details> | Jan 2026 | (N) | RoboReward 4B / 8B | <details><summary>UC Berkeley / Stanford University</summary>- Sergey Levine / Chelsea Finn</details> | [Notes](notes/roboreward_260202/notes.md) |
| 02 | <details><summary>RoboArena</summary>: Distributed Real-World Evaluation of Generalist Robot Policies</details> | Nov 2025 | <details><summary>DROID Robot Platform</summary>- consists of a Franka Panda 7DoF robot arm, two adjustable Zed 2 stereo cameras, a wristmounted Zed Mini stereo camera, and an Oculus Quest 2 headset with controllers for teleoperation (refer to [here](https://droid-dataset.github.io/))</details> | (N) | <details><summary>UC Berkeley / Stanford University</summary>- Chelsea Finn / Sergey Levine</details> | <details><summary>distributed real-world policy evaluation</summary>- aggregates a large number of such pairwise, double-blind comparisons into a global policy ranking.</details> |
| 03 | <details><summary>Open X-Embodiment (OXE)</summary>: Robotic Learning Datasets and RT-X Models</details> | Since Oct 2023 | <details><summary>Multi</summary>- 22 different robotic embodiments from 21 different institutions</details> | RT-1-X / RT-2-X | DeepMind | <details><summary>1M+ real robot trajectories</summary>- constructed by pooling 60 existing robot datasets from 34 robotic research labs and converting them all into RLDS data format.</details> |

## Pool of Works

Please check [here](assets/to_be_read.md) for more information.

## Reference Materials
- [Reinforcement Learning Course by David Silver, UCL](https://davidstarsilver.wordpress.com/teaching/) 
- ME5418: Machine Learning in Robotics by Prof Guillaume, NUS, Fall 2025 (unfortunately not publicly available yet 😢)

## Contact
For any suggestions or contributions, please feel free to open an issue or submit a pull request. You are also welcome to reach out me for further questions via email at [maij@u.nus.edu](mailto:maij@u.nus.edu)!