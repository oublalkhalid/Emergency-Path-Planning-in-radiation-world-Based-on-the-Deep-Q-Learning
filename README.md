# Emergency-Path-Planning-in-radiation-world-Based-on-the-Deep-Q-Learning
This code accompagne "Emergency Path Planning in radiation world Based on the Deep Q-Learning (DQL)", which is apparu on draft preprint easychair.org conference of inf581-rl-2022.

## About
This project uses a deep reinforcement learning algorithm in association with a particle dynamics model to train agents to find the fastest path to evacuate a human from radioactive building with presence of the enemy.

Efficient emergency evacuation is crucial for survival. However, it is not clear if the application of the self-driven force of the social-force model results in optimal evacuation, especially in complex environments with obstacles of radiation. In this work, we developed a deep reinforcement learning algorithm in association with the social force model to train agents to find the fastest evacuation path. During training, we penalized every step of an agent in the room and gave zero reward at the exit. We adopted the Dyna-Q learning approach. We showed that our model can efficiently handle modeling of emergency evacuation in complex environments with multiple room exits and convex and concave obstacles where it is difficult to obtain an intuitive rule for fast evacuation using just the social force model.

# *How to use this code*
## Setup
*Note:* This code was designed to be used with Python 3.6.13, and is not compatible with later versions.

To install this project's package dependencies, please run the following command:

    pip install -r requirements.txt

## Test
This project provides framework to train an agent for emergency evacuation in two scenarios.

Our work on this project is summarized in a workbook that you can run in less than 10 minutes.
 
```
Emergency_Path_Planning_in_radiation_world_Based_on_the_Deep_Q_Learning.ipynb
```


## Cite

To reference this work, please use the following:
```
@article{pathdeepqlearning,
  title={Emergency Path Planning in radiation world Based on the Deep Q-Learning (DQL)},
  author={Khalid Oublal, Xinyi DAI, Yutong Meng},
  year={2022},
  publisher={Ecole Polytechnique}
}
```
