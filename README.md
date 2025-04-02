# Reinforcement Learning FlappyBird

This repository contains the implementation of the Flappy Bird environment with reinforcement learning algorithms (QLearning and Sarsa) for two scenarios: small gap and big gap between pipes. Below is the structure of the project and descriptions of the files and directories.

<img src="videos/big_gap_videos/MyQLearning_ep=0.1_ga=0.95_lr=0.1/72000.gif" width="400px">

### 1. **`content/`**
This directory contains the trained models for both QLearning and Sarsa algorithms in the small gap and big gap scenarios:
- **`big_gap_QLearning.pkl`**: The trained QLearning model for the big gap scenario (gap = 80).
- **`big_gap_Sarsa.pkl`**: The trained Sarsa model for the big gap scenario (gap = 80).
- **`small_gap_QLearning.pkl`**: The trained QLearning model for the small gap scenario (gap = 65).
- **`small_gap_Sarsa.pkl`**: The trained Sarsa model for the small gap scenario (gap = 65).

These `.pkl` files store the policy tables for their respective models and are used for evaluation in the `eval_FlappyBird.ipynb` notebook.

---

### 2. **`videos/`**
This directory contains videos demonstrating the training process for both QLearning and Sarsa models in both scenarios. The videos are further organized by gap size and algorithm:
- **`big_gap_videos/`**: Contains videos for the big gap scenario (gap = 85).
  - **`QLearning/`**: Videos showing the training process of the QLearning model.
    - **`video1.mp4`**: Shows the early stages of training where the agent begins learning.
    - **`video2.mp4`**: Demonstrates later stages of training as the agent improves.
  - **`Sarsa/`**: Videos showing the training process of the Sarsa model.
    - **`video1.mp4`**: Captures the agent's initial attempts to learn the task.
    - **`video2.mp4`**: Highlights progress in later training stages.

- **`small_gap_videos/`**: Contains videos for the small gap scenario (gap = 65).
  - **`QLearning/`**: Videos showing the training process of the QLearning model.
    - **`video1.mp4`**: Demonstrates the agent's early learning behavior.
    - **`video2.mp4`**: Shows how the model improves over time.
  - **`Sarsa/`**: Videos showing the training process of the Sarsa model.
    - **`video1.mp4`**: Captures initial learning stages for the agent.
    - **`video2.mp4`**: Shows more advanced progress during training.

---


### 3. **`ex1_FlappyBirdMidTerm.ipynb`**
- This notebook is used for training the models. It includes the implementation of QLearning and Sarsa algorithms and their training process for both small gap and big gap scenarios. It outputs the trained models as `.pkl` files in the `content/` directory.

### 4. **`eval_FlappyBird.ipynb`**
- This notebook is used for evaluating the trained models. To run this notebook, you need to load the corresponding `.pkl` files from the `content/` directory:
  - `content/big_gap_QLearning.pkl`
  - `content/big_gap_Sarsa.pkl`
  - `content/small_gap_QLearning.pkl`
  - `content/small_gap_Sarsa.pkl`

The evaluation notebook demonstrates how well the models perform based on the learned policies.

---

### 5. **`report.pdf`**
- This file contains the detailed report of the project, including methodology, results, and discussion.

---

### Instructions
1. **Training**: Use the `ex1_FlappyBirdMidTerm.ipynb` notebook to train the models for both the small gap and big gap scenarios.
2. **Evaluation**: Use the `eval_FlappyBird.ipynb` notebook to evaluate the models. Ensure that the `.pkl` files from the `content/` directory are available.
3. **Videos**: Explore the `videos/` directory to observe the training process for both algorithms in both scenarios.
