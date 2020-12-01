# Continuous-Control
This is for completing the Udacity Deep Reinforcement Learning Project 2.

# Project Details
The agent is a double-jointed arm that can move to target locations in a Unity ML-Agents Reacher Environment. The goal of the agent is to maintain its position at the target location for as many time steps as possible.

1. The state space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. 
2. Each action is a vector with four numbers, corresponding to torque applicable to two joints and each number is between -1 and 1.
3. This project contains a single agent.
4. The task is episodic. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. The agent must get an average score of +30 over 100 consecutive episodes to solve the environment.

# Getting Started
The code is written in Python 3 and PyTorch. Instructions for installing dependencies or downloading needed files for Windows are provided on https://github.com/udacity/deep-reinforcement-learning#dependencies. The process is summarized as follows:
1. Download AnaConda3
2. Open the AnaConda Powershell Prompt to enter the following commands to create and activate a new env "drlnd" using an old Python version 3.6 required by this project:
    ```
    conda create --name drlnd python=3.6
    conda activate drlnd
    ```
3. In the new env "drlnd", run the following to install the old PyTorch version for installing Unity provided by Udacity:
    ```
    conda install pytorch=0.4.0 -c pytorch
    git clone https://github.com/udacity/deep-reinforcement-learning.git
    cd deep-reinforcement-learning/python
    pip install .
    ```
4. Create an IPython kernel for the drlnd environment:
    ```
    python -m ipykernel install --user --name drlnd --display-name "drlnd"
    ```
# Instructions
The instructions for running the code are provided below. 
1. Replace the notebook Continuous_Control.ipynb in deep-reinforcement-learning/p2_continuous-control with the code given here and also copy model.py and dqn_agent.py to the same folder.
2. For Windows 64-bit, download the file https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip, unzip the file and place the folder Reacher_Windows_x86_64 in the same p2_continuous-control folder.
3. Open Jupyter Notebook.
4. On Notebook, open Continuous_Control.ipynb and select drlnd in the Kernel.
5. Run the code in each cell. The results for the weights are stored in the checkpoint_actor.pth and checkpoint_critic.pth files. The rewards per episode are shown in a plot in the Notebook. The environment with the double-jointed arm is shown in another window. The training will take about an hour with GPU.
6. After the goal is reached, the environment is close and the project is completed.

# References
1. Udacity Deep Reinforcement Learning Nanodegree Program https://www.udacity.com/
2. https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum
3. Continuous control with deep reinforcement learning https://arxiv.org/abs/1509.02971
4. https://github.com/ShangtongZhang/DeepRL
