# Introduction

Deep reinforcement learning, revolutionizing the field of AI, represents a step towards building an autonomous system with a deeper understanding of the visual world. In this project we demonstrate Deep Q-learning in the Arcade Learning Environment (ALE), a challenging framework composed of dozens of Atari 2600 games used to evaluate general competency in AI.

# Problem Statement 

The game that we have chosen for our project is: ASSAULT. This is a very famous game released in the year 1983 where we will control a spaceship fixated at the bottom of the screen. The gameplay involves the player shooting projectiles towards an enemy mothership that deploys smaller ships to attack the player. The model that we aim to build consists of a convolutional neural network, trained with a variant of Q-learning; whose input is raw pixels and output is a value function estimating future rewards. Our agent iteratively learns across a multitude of training iteration steps harnessing the power of deep reinforcement learning in order to achieve scores that match human intellect and eventually surpass it.

# Models

We have used DQN and DDQN Network models to train and test the provided ASSAULT game. DQN or Deep-Q Networks were first proposed to bring the advantages of deep learning to reinforcement learning (RL), Reinforcement learning focuses on training agents to take any action at a particular stage in an environment to maximize rewards. It uses a Loss function rather than an equation. It also uses the Predicted (Current) Q Value, Target Q Value, and observed reward to compute the Loss to train the network, and thus improve its predictions. DDQN or Dueling Deep Q Networks is a reinforcement learning algorithm that tries to create a Q value via two function estimators: one that estimates the advantage function, and another that estimates the value function. It utilizes Double Q-learning to reduce overestimation by decomposing the max operation in the target into action selection and action evaluation. We evaluate the greedy policy according to the online network, but we use the target network to estimate its value.

# Results 

Let's see the performance of the DDQN model before training: 


https://user-images.githubusercontent.com/29314283/176975183-1a2e3d57-e230-431c-9f22-9c0ed694059d.mp4

We can compare it with the results obtained after the training: 


https://user-images.githubusercontent.com/29314283/176975208-6c4de23a-8231-4064-9b02-f427fae6b21b.mp4

Overall we can see the improvement in the score. We learnt how they (DQN and DDQN) use their functions to predict Q-values, target Q-values and provide the rewards for the predicted Q-values. 



