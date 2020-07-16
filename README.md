### Overview 

This repo contains my submission for Udacity Deep Reinforcement Learning course - Project 2.

The project is about training 20 double-jointed arms to move to their respective target locations and stay there as long as possible.

A reward of +0.1 is provided for each step that the agent's hand is in the goal location. 

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. 

Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The task is episodic and is considered successful when all the agents can obtain an average score of at least 30 points
over a window of 100 consecutive episodes.

### Setup

The agent is implemented in `ddpg_agent.py`.

There is a `Continuous_Control.ipynb` file with all dependency requirements placed on the top cell, including the agent file.

These dependencies are readily available on Udacity workspace. On local, any missing dependency can be installed via `pip install <dependency name>`.

Models are defined in-line within the notebook.

The environment can be obtained from the [official Udacity repo](https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control#getting-started). Here I am using the second version where there are 20 agents operating in parallel.

Once downloaded, unzip and place it in the same folder with the notebook, and change the file path accordingly to point to the environment file.

Now setup is finished. Running all the cells within `Continuous_Control.ipynb` will walk you through the training.

Successful model weights are saved in the `checkpoint_actor.pth` and `checkpoint_critic.pth` files.

Note that to be able to see the agents while training, the notebook needs to be run on local.


### Training

This can be found in the `REPORT.md` file
