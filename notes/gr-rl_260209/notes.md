# GR-RL: Going Dexterous and Precise for Long-Horizon Robotic Manipulation

## Key Take-aways

### 1. 效果惊艳的穿鞋带Demo

Video refer to [project page](https://seed.bytedance.com/en/gr_rl).

### 2. Distributional critic model

- base: a causal transformer with 5B parameters
- recipe 
    - data: successful + failed trajectories
    - method: only offline RL
- reward: sparse reward 0/1
- others
    - output: bounded between [0,1]


### 3. Policy model
- base (same architecture as GR-3)
    - backbone: Qwen2.5-VL-3B-Instruct
    - action head: DiT trained by flow matching objectives
- recipe
    - data 
        - filtered by trained critic model, 
        - value drop greater than a certain threshold

    - method: offline RL + **online RL (DSRL)**

---
Note,
1. online RL方法与RoboReward中的RL方法一致，均为DSRL (including S. Levine)
---

### 4. morphological symmetry augmentation

Policy training offline RL阶段的一种数据增强的方法，本文贡献之一

- method
    1. 所有图像翻转，左右腕部相机交换
    2. 所有state和action基于世界坐标系翻转
    3. 语言指令中涉及左右的词汇互换

---
Note，
1. 并未进行消融实验

    > Empirically, the symmetry data augmentation can effectively enhance the performance of the policy

---