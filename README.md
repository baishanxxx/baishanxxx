# Hi there, I'm WEN 👋 / 你好，我是 WEN 👋

🤖 **Research Focus | 研究方向:** Embodied AI (具身智能) | Multi-modal Robot Learning (多模态机器人学习) | Vision-Language-Action (VLA) 

### 🔬 Research Interests | 研究兴趣

**EN:** Focused on Embodied AI and Multi-modal Robot Learning. Developing Vision-Language-Action (VLA) architectures for long-horizon task planning. Researching closed-loop feedback and autonomous error correction to improve the robustness of end-to-end policies in complex, dynamic environments.

**ZH:** 专注于具身智能与多模态机器人学习。开发用于长视距任务规划的视觉-语言-动作 (VLA) 架构。研究闭环反馈与自主纠错，以提高端到端策略在复杂动态环境中的鲁棒性。

### 🛠 Tech Stack | 技能栈

**Programming & Frameworks (编程与框架):**
`Python` `C++` `PyTorch` `ROS/ROS2` `OpenCV` `MATLAB`

**Robotics & AI Algorithms (机器人与 AI 算法):**
`Diffusion Policy` `Flow Matching` `VLA (Vision-Language-Action)` `PPO` `IQL` `V-JEPA2`

**Simulation & Design (仿真与设计):**
`MuJoCo` `Isaac Gym` `PyBullet` `robosuite` `SolidWorks` `AutoCAD`

#### 1. Adversarial Diffusion Policy for Observation-Based Learning  | 基于观察学习的对抗扩散策略
[![View Repository](https://img.shields.io/badge/View_Project_Details-Click_Here-blue?style=for-the-badge&logo=github)](https://github.com/baishanxxx/Adversarial-Diffusion-Policy)

- **Summary:** Proposed a framework combining Conditional Diffusion Models with GANs to recover manipulation policies from vision-only expert sequences. / 提出了一种结合条件扩散模型与生成对抗网络的框架，用于从纯视觉专家序列中恢复操作策略。
  
#### 2. Whole-Body Control of a Mobile Legged Manipulator| 移动腿足机械臂的全身控制
[![View Repository](https://img.shields.io/badge/View_Project_Details-Click_Here-blue?style=for-the-badge&logo=github)](https://github.com/baishanxxx/Mobile-Legged-Manipulator)

- **Summary:** Integrating RL-based High-Dynamic Locomotion and Diffusion Policy-based Visuomotor Manipulation via an asynchronous architecture. / 融合基于强化学习的高动态运动控制与基于扩散策略的视觉精细操作，并通过异步架构实现极低延迟部署。

### 🔥 Featured Projects 

#### 1. Adversarial Diffusion Policy for Observation-Based Learning
![Status](https://img.shields.io/badge/Status-In_Preparation-blue) [![View Repository](https://img.shields.io/badge/Code-View_Repo-orange?logo=github)](https://github.com/baishanxxx/Adversarial-Diffusion-Policy)

> A novel Imitation Learning from Observation (IfO) framework recovering robust manipulation policies exclusively from vision-only expert sequences, eliminating the need for explicit action supervision.

<div align="center">
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/video1_1.gif" width="45%" alt="Adversarial Discriminator Agent"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/video2_1.gif" width="45%" alt="Feature MSE Agent"/>
</div>

* **Core Method:** Combined Conditional Diffusion Models with GANs (Visual-feature Discriminator as reward generator).
* **Key Results:** Achieved an **85% success rate** on `robomimic lift` (MuJoCo), retaining 91% of the performance of a fully action-supervised expert baseline.

#### 2. Whole-Body Control of a Mobile Legged Manipulator
![Status](https://img.shields.io/badge/Status-In_Preparation-blue) ![Hardware](https://img.shields.io/badge/Hardware-Unitree_Go2_+_Arm-lightgrey) [![View Repository](https://img.shields.io/badge/Code-View_Repo-orange?logo=github)](https://github.com/baishanxxx/Mobile-Legged-Manipulator)

> An embodied deployment framework integrating low-level high-dynamic motion control (RL) and high-level multi-modal perception interfaces (Diffusion Policy).

<div align="center">
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/target_2.gif" width="45%" alt="Target Tracking"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/jump_1.gif" width="45%" alt="High Dynamic Backflip"/>
</div>
<div align="center">
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/button_video_1.gif" width="45%" alt="Real-world Execution"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/button_inference.gif" width="45%" alt="Policy Inference"/>
</div>

* **High-Dynamic Locomotion (RL):** Implemented whole-body 6D target tracking and high-dynamic backflips via PPO in Isaac Gym.
* **Visuomotor Manipulation:** End-to-end mapping from raw visual input to motor commands using Diffusion Policy.
* **Architecture:** Designed an asynchronous decoupled system (1Hz inference, 50Hz+ execution), reducing inference latency to **< 0.01s**.

---
<div align="center">
<i>For comprehensive project details, mathematical formulations, and publications, please view my <a href="#">Curriculum Vitae</a>.</i>
</div>
