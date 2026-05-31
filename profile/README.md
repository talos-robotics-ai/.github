<h1 align="center">⁕ Talos Robotics AI</h1>

<p align="center"><b>Making humanoids work in the real world for specific tasks applications.</b></p>

<p align="center">
  A software layer that lets industrial customers <i>teach, deploy, adapt, and improve</i><br/>
  robot skills directly on their own hardware — no R&D team per site.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/ROS_2-Humble-22314E?logo=ros" />
  <img src="https://img.shields.io/badge/Sim-Isaac_Sim_5.1-76B900?logo=nvidia" />
  <img src="https://img.shields.io/badge/Sim-Gazebo_Fortress-orange" />
  <img src="https://img.shields.io/badge/Sim-MuJoCo-FF6F00" />
  <img src="https://img.shields.io/badge/GPI" />
  <img src="https://img.shields.io/badge/Based_in-Milan,_Italy-1f6feb" />
</p>

---

## 👋 What we build

Physical AI is advancing fast, but deployment still doesn't scale: **every new line is a
re-launch**, modern AI workflows are poorly integrated with robotics simulators, and
fleet data is hard to collect without breaking privacy. Talos closes that gap with a
**no-code platform** to design a skill, validate it in simulation, deploy it to existing
humanoid hardware, and keep improving it from real-world operational data.

Under the hood that platform is a full **sim-to-real robotics stack**:
with our implemented dashboard, the customer is capable of:
- Deploy inference in simulation.
- Evaluate the performances.
- Run real robot Physical AI models through an MCP style architecture.
- General Physical intelligence for enabling a robot agnostic platform.

---
<!--

## ⚙️ Core technology

---
-->


## 🏭 Applications

General Physical Intelligence · pick-and-place · warehouse and logistics tasks — taught
on the platform, validated in sim, deployed to real humanoid hardware, and improved from
fleet data.

---

## 🛠️ Tech stack

`ROS 2 Humble` · `NVIDIA Isaac Sim` · `Isaac Lab` · `Gazebo Fortress` · `Mujoco` ·
`CasADi` / `IPOPT` · `Bayesian Optimization (TPE + GP)` · `Reinforcement Learning` ·
`Qwen3-VL` · `Flow-matching Diffusion Transformer` · `Docker` · `WebSockets` ·
`Unitree Go2 & G1`

---

## 📄 Papers

**[Bayesian Optimization for Learning Nonlinear MPC in Autonomous Agent Navigation](https://github.com/talos-robotics-ai/Go2_navigation/blob/main/documentation/conference_101719.pdf)**
<br/>Lorenzo Ortolani, Gabriel Voss, Gabriele Beltrami, Francesco Dorati, Tommaso Felice Banfi — *Talos Robotics AI*

A map-free navigation stack pairing rolling-horizon **A\*** on a LiDAR **Gaussian occupancy
grid** with a **CasADi/IPOPT nonlinear MPC** (smooth sigmoid obstacle barrier). Controller
weights are tuned offline by **Tree-structured Parzen Estimator** Bayesian Optimization over
an 11-D parameter space, with a **GP surrogate** for sensitivity analysis. On the Unitree
Go2 (Gazebo Fortress → hardware) it reaches up to **90.0% success rate** and a **−38.7%**
average path length with negligible sim-to-real degradation.

[![Paper](https://img.shields.io/badge/Paper-PDF-b31b1b.svg)](https://github.com/talos-robotics-ai/Go2_navigation/blob/main/documentation/_3a__PathPlanning_MPC.pdf)
[![Code](https://img.shields.io/badge/Code-Go2__navigation-1f6feb?logo=github)](https://github.com/talos-robotics-ai/Go2_navigation)

---

## 👥 Team

| | |
|---|---|
| **Gabriel Voss** | CEO — Computer Engineering, PoliMi |
| **Lorenzo Ortolani** | CTO — Automation & Control Engineering (MSc), PoliMi |
| **Gabriele Beltrami** | HOE - Automation & Control Engineering (MSc), PoliMi |
| **Raul Rizzon** | CSO — Business & Entrepreneurship (MSc), UCSC |

**Manipulation:** Giacomo Galbiati · Massimiliano Menzolini · Filippo Rossetti
**Locomotion & RL:** Tommaso Banfi (visiting ETH, CERN) · Francesco Dorati
**Navigation & Mapping:** Gabriele Beltrami

📍 Milan, Italy

<p align="center"><sub>Talos Robotics AI — one software stack, from quadruped to humanoid, from simulation to the factory floor.</sub></p>
