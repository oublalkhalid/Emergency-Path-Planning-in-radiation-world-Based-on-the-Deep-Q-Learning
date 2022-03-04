# Emergency-Path-Planning-in-radiation-world-Based-on-the-Deep-Q-Learning
This code accompagne "Emergency Path Planning in radiation world Based on the Deep Q-Learning (DQL)", which is apparu on easychair.org conference of inf581-rl-2022.

## About
This project uses a deep reinforcement learning algorithm in association with a particle dynamics model to train agents to find the fastest path to evacuate a room with obstacles.

Efficient emergency evacuation is crucial for survival. However, it is not clear if the application of the self-driven force of the social-force model results in optimal evacuation, especially in complex environments with obstacles of radiation. In this work, we developed a deep reinforcement learning algorithm in association with the social force model to train agents to find the fastest evacuation path. During training, we penalized every step of an agent in the room and gave zero reward at the exit. We adopted the Dyna-Q learning approach. We showed that our model can efficiently handle modeling of emergency evacuation in complex environments with multiple room exits and convex and concave obstacles where it is difficult to obtain an intuitive rule for fast evacuation using just the social force model.

# *How to use this code*
## Setup
*Note:* This code was designed to be used with Python 3.6.13, and is not compatible with later versions.

To install this project's package dependencies, please run the following command:

    pip install -r requirements.txt

## Train
This project provides framework to train an agent for emergency evacuation in two scenarios:

1. An empty room with four exits. To train this model, run the following command:
```
    python .py
```

2. A room with three exits and two obstacles. To train this model, run the following command:
```
    python .py
```

## Test
A built-in testing script can be used to assess generalization capabilities, illustrating the optimal policy learned by an agent during training. A pre-trained policy has been included in the model folder, which can be tested for reference. To run the testing framework, you can use the following command:

    python .py



## Cite

To reference this work, please use the following:
```
[1]  In  Lecture  III  -Q-learning.INF581 Advanced Machine Learning andAutonomous Agents, 2022.

[2]  G.  A.  Rummery  and  M.  Niranjan  On-line  Q-learning  using  connection-ist systems. https://www.researchgate.net/publication/2500611On-LineQ-LearningUsingConnectionistSystems, 1994.

[3]  C.  J.  C.  H.  Watkins  and  P.  Dayan  ,  Technical  note  q-learning.  https://link.springer.com/article/10.1023/A:1022676722315, 1992.

[4]  V. Mnih, K. Kavukcuoglu, and D. S. et al Human-level control throughdeep reinforcement learning. https://daiwk.github.io/assets/dqn.pdf, 2015.

```
