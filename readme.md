# Deep Reinforcement Learning Project : Navigation

This project is part of Udacity's [AIRBUS Artificial Intelligence Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)

## Introduction

This project is based on Unity ml-agents which is:
>an open-source project that enables games and simulations to serve as environments for training intelligent agents.

*source: https://github.com/Unity-Technologies/ml-agents*

The goal is to collect as many yellow bananas as possible, while avoiding blue ones, in a closed square world:

![Image](https://video.udacity-data.com/topher/2018/June/5b1ab4b0_banana/banana.gif)

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. 

Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

*source: https://github.com/udacity/deep-reinforcement-learning/blob/master/p1_navigation/README.md*

## Files description

- `Navigation.ipynb`: Notebook used to explore game environment and train agents with DQL.
- `dqn_agent.py`: Python script defining agent class
- `model.py`: Python script defning the neural network architecture on which the agent is based
- `checkpoint.pth`: Checkpoint containing pre-trained model

## Getting started

### Requirements

- Configure a Python 3.6 (or higher) environment with Pytorch 0.4.0 (or higher). Needed requirements can be found in https://github.com/udacity/deep-reinforcement-learning#dependencies

- Download the environment from one of the links below.  You need only select the environment that matches your operating system:
  - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
  - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
  - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
  - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

### Train the agent

An agent has already been trained to play the game. This agent used Deep Q learning (brief description can be found in the report.md file).

To train a new agent, just execute the cells in the `Navigation.ipynb` notebook. You can change the architecture of the `model.py` file. 

To train the agent I uses Udacity's workspace which allows to use GPU. Playing manually or watch agent plays has not been implemented as it is not available with Udacity worspace.
