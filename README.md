# 🤖 Human Preference Alignment Tutorial

This repository serves as a hands-on tutorial for aligning language models to human preferences using various techniques such as Reinforcement Learning from Human Feedback (RLHF), Direct Preference Optimization (DPO), and instruction fine-tuning.

Each notebook walks through a key component in the human preference alignment pipeline, from reward modeling to policy optimization.

---

## 📚 Tutorial Notebooks

| Notebook | Description |
|----------|-------------|
| [Instruction_fine_tuning.ipynb](./Instruction_fine_tuning.ipynb) | A step-by-step guide on fine-tuning a base language model using human-written instructions. This is the first step in making the model follow general human instructions better. |
| [RewardTrainer.ipynb](./RewardTrainer.ipynb) | Demonstrates how to train a reward model using preference-labeled data (e.g. comparisons between two completions) to score generations. This model is used to represent human preferences. |
| [PPOTrainer.ipynb](./PPOTrainer.ipynb) | Shows how to use Proximal Policy Optimization (PPO) to fine-tune a model using the reward model as feedback, forming the core of RLHF. |
| [DPO_Fine_Tuning.ipynb](./DPO_Fine_Tuning.ipynb) | Implements Direct Preference Optimization (DPO), a simpler and more stable alternative to PPO that directly optimizes the model towards preferred outputs. |

---

## 🔍 Goal

The goal of this tutorial series is to provide a clear, working implementation of key alignment methods so you can:

- Understand how to train a reward model
- Apply instruction tuning
- Fine-tune a model using PPO or DPO
- Experiment with and compare alignment strategies

---

## 📦 Requirements

Make sure to install the required dependencies, such as:

```bash
pip install transformers accelerate datasets trl peft
