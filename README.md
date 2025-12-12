# Reinforcement Learning Final Project  
**Hopper-v4 Continuous Control with PPO, SAC, and TD3**

This repository contains our final project for the Reinforcement Learning course, completed by Yurou Dai and me.  
The project explores training and evaluating multiple RL algorithms on the Hopper-v4 environment using Stable-Baselines3.  
All experiments, training code, evaluation plots, and comparisons are included in the Jupyter notebook **`project.ipynb`**.

---

## 📂 Project Contents

The main notebook includes the following parts:

#### 1. PPO Agent
- Environment setup and hyperparameters  
- Custom `RewardLogger` callback  
- PPO training on Hopper-v4  
- Plot of episode rewards and moving average  

#### 2. SAC Agent
- Training a SAC agent on the same environment  
- Rewards recorded using the same `RewardLogger` callback  
- Reward plot for SAC performance  

#### 3. TD3 Agent
- TD3 setup with action noise  
- Rewards recorded using the same callback`  
- Reward plot for TD3 performance    

#### 4. Algorithm Comparison
- Collects episode rewards from PPO, SAC, and TD3  
- Saves episode reward data to a JSON file (e.g. `models_rewards_YYYY-MM-DD_....json`)  
- Loads this JSON file and generates a combined comparison plot  
- Final comparison figure saved as `output_whole.png`

---

## 📦 Requirements

To run the notebook, you need:

```bash
pip install stable-baselines3[extra] gymnasium[mujoco] numpy matplotlib

