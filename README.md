# Deep Reinforcement Learning Project : Continuous Control 
My solution to Udacity Deep Reinforcement Learning Nanodegree 's Project 2 - Continuous Control 

## Environment Details
In this environment, a double-jointed arm agent is trained to move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its tip at the target location for as many time steps as possible.

### State and Action Space
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.


### Solving condition
The task is episodic, and in order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes.
As shown below, the tip of the trained agent can reach the target position (green pot) and then rotate with it.
![trained agent](assets/trained_agent.gif)

## Instructions
This project implement a reinforcement learning method called Deep Deterministic Policy Gradient(DDPG). DDPG is an Actor-Critic algorithm which concurrently learns a Q-function and a policy. It uses off-policy data and the Bellman equation to update the Q-function, and uses the Q-function to update the policy. Refer the paper [Continuous control with deep reinforcement learning](https://arxiv.org/abs/1509.02971) to see more DDPG algrithm details. 

And refer [the Report file](https://github.com/oliver1112/Udacity-DRL-ContinuousControl/blob/master/Report.md) to see my hyperparameters details, along with ideas for future work.

Follow the code in [the ipynb file](https://github.com/oliver1112/Udacity-DRL-ContinuousControl/blob/master/Continuous_Control.ipynb) in order to train the agent.

The algorithm is written in PyTorch and Python 3


## Getting Started
To set up your python environment to run the code in this repository, follow the instructions below.

1. please follow the instructions in the python file to set up your Python environment. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.
```bash
pip install .
```

2. You don't need to choose the complete Unity environment, just choose the environment that matches your operating system to install the  environment.

    I use the Windows (64-bit) operating system, [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip) to install.

    For other operating system, please download the environment from one of the links below.
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)




3. Follow the instructions in `Continuous_Contral.ipynb` to run my code!  
