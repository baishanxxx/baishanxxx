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

### 🔥 Featured Projects | 精选项目

#### 1. Adversarial Diffusion Policy for Observation-Based Learning | 基于观测学习的对抗扩散策略
![Status](https://img.shields.io/badge/Status-In_Preparation-blue) [![View Repository](https://img.shields.io/badge/View_Project_Details-Click_Here-blue?style=for-the-badge&logo=github)](https://github.com/baishanxxx/Adversarial-Diffusion-Policy)

> **EN:** A novel Imitation Learning from Observation (IfO) framework recovering robust manipulation policies exclusively from vision-only expert sequences, eliminating the need for explicit action supervision.
> **ZH:** 一个仅利用纯视觉专家序列即可恢复稳健操作策略的新型模仿学习框架，完全无需显式的动作监督数据。

**Traditional IL vs. Our IfO Pipeline (传统模仿学习与我们的 IfO 管线对比):**

<div align="center">
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/method.png" width="60%" alt="Traditional IL vs. Our IfO Pipeline"/>
</div>

**Architecture vs. Performance (架构原理与效果演示):**

<div align="center">
  <p><i>Pathway 1: Adversarial Discriminator (对抗判别器机制)</i></p>
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/method1.png" width="40%" alt="Adversarial Architecture"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/video1_1.gif" width="20%" alt="Adversarial Demo"/>
</div>

<div align="center">
  <p><i>Pathway 2: Feature MSE Baseline (特征均方误差基线)</i></p>
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/method2.png" width="40%" alt="MSE Architecture"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Adversarial-Diffusion-Policy/main/assets/video2_1.gif" width="20%" alt="MSE Demo"/>
</div>

* **Core Method (核心方法):** Combined Conditional Diffusion Models with GANs, using a visual-feature discriminator to evaluate and align predicted observation sequences. (结合条件扩散模型与生成对抗网络，利用视觉特征判别器评估并对齐预测的观测序列。)
* **Key Results (关键结果):** Achieved an **85% success rate** on `robomimic lift`, retaining 91% of the performance of a fully action-supervised expert baseline. (在 `robomimic lift` 任务中达到 **85% 成功率**，保留了完全监督专家基线 91% 的性能。)

#### 2. Whole-Body Control of a Mobile Legged Manipulator | 移动腿足机械臂的全身控制
![Status](https://img.shields.io/badge/Status-In_Preparation-blue) ![Hardware](https://img.shields.io/badge/Hardware-Unitree_Go2_+_Arm-lightgrey) [![View Repository](https://img.shields.io/badge/View_Project_Details-Click_Here-blue?style=for-the-badge&logo=github)](https://github.com/baishanxxx/Mobile-Legged-Manipulator)

> **EN:** An embodied deployment framework integrating low-level high-dynamic motion control (RL) and high-level multi-modal perception interfaces (Diffusion Policy).
> **ZH:** 一个融合了底层高动态运动控制（强化学习）与顶层多模态感知接口（扩散策略）的具身部署框架。

**High-Dynamic Locomotion (高动态运动控制):**

<div align="center">
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/target_2.gif" width="40%" alt="Target Tracking"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/jump_1.gif" width="40%" alt="High Dynamic Backflip"/>
</div>

* **RL-based Control (强化学习控制):** Implemented whole-body 6D target tracking and high-dynamic backflips via PPO in Isaac Gym. (在 Isaac Gym 中通过 PPO 实现了全身 6D 目标追踪与高动态后空翻。)

**Visuomotor Manipulation & Architecture (视觉精细操作与系统架构):**

<div align="center">
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/button_video_1.gif" width="40%" alt="Real-world Execution"/>
  <img src="https://raw.githubusercontent.com/baishanxxx/Mobile-Legged-Manipulator/main/assets/button_inference.gif" width="40%" alt="Policy Inference"/>
</div>

* **Diffusion Policy (扩散策略操作):** End-to-end mapping from raw visual input to motor commands using Diffusion Policy. (利用扩散策略构建了从原始视觉输入到电机指令的端到端映射。)
* **Asynchronous System (异步解耦架构):** Designed an asynchronous decoupled system (1Hz inference, 50Hz+ execution), reducing inference latency to **< 0.01s**. (设计了异步解耦架构，将推理延迟降低至 0.01s 以下，确保实时响应。)

---
