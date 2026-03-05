<h1 style="text-align: center;">ECEN 743: Reinforcement Learning</h1>
<h1 style="text-align: center;">Assignment 3</h1>


## Overview
1. You have to submit a report in `HTML`, your code and two videos to Canvas.
2. Put all your files (`HTML` report, code, videos) into a **single compressed folder** named `Lastname_Firstname_A3.zip`.
3. In Jupyter Notebook, you can export it in `HTML` by going through the top toolbar: File -> Save and Export Notebook As... -> HTML.
4. This homework is self-containted in one Jupyter notebook. In your `zip`, we expect only your `HTML` report, **one** Jupyter notebook and **two** videos.


## Installation Instructions
This course uses the Texas A&M High Performance Research Computing (HPRC) system for all programming assignments.  
Follow the instructions from [Assignment 1](https://github.com/ECEN743-TAMU/ECEN743-SP26-A1-DP) to create your account, set up the required conda environment, and launch JupyterLab.  

**NOTE**: If you get an error while importing torch, please rerun step-3 from Assignment 1.


## Assignment
In this homework, you will train a deep Q-Learning algorithm to land a lunar lander on the surface of the moon. We will use the Lunar Lander environment (LunarLander-v3) from  Gymnasium. The environment consists of a lander with $4$ discrete actions and a continuous state space. A detailed description of the environment can be found [here](https://gymnasium.farama.org/environments/box2d/lunar_lander/). The problem is solved if the total reward per episode is 200 or above. Do not stop training on the first instance your agent gets a reward
above 200, your agent must achieve a reward of 200 or above consistently.

1. **Deep Q-Learning:** Implement deep Q-learning **with** experience replay and target network. You should include the training curve in the HTML report (x-axis is the number of episode and the y-axis should be episodic cumulative reward). Use a sliding window average to get smooth plots. Include a description of the hyperparameters used. Also, you should submit a video of the smooth landing achieved by your RL algorithm. Try to find the optimal hyperparameters that will enable fast convergence to the optimal policy.  

2. **Ablation Study:** Perform ablation study to understand the importance of experience replay and target network. You should include the training curves, and  describe your observations and inferences.   

3. **Algorithmic Improvements:** As we discussed in the class, there has been a number of improvements in the deep Q-learning algorithm and architecture, such as double DQN, dueling DQN, prioritized experience replay, and many other (see the slides and related papers).  Implement double DQN. Explain your implementation and demonstrate the benefit.  

4. **Deep Q-Learning on Another Environment:** Congratulations on implementing deep Q-Learning on the Lunar-Lander-v3 environment! Now,  learn the optimal  policy for another control problem (environment) using deep Q-Learning. You can select one environment from the *Classical Control* set, *Box2D* set or *Atari Games* set in Gymnasium.  In the HTML report, you need to clearly specify the environment and provide a link to the corresponding page in Gymnasium. You need to include the training curve and describe the hyperparameters used. You should also include the video of the performance. 
