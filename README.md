# Emergency-Path-Planning-in-radiation-world-Based-on-the-Deep-Q-Learning
This code accompagne "Emergency Path Planning in radiation world Based on the Deep Q-Learning (DQL)", which is apparu on draft preprint easychair.org conference of inf581-rl-2022 [(The paper is available here)](https://drive.google.com/file/d/1VZAT00KhMzYD-Yx5Ygv5xlNH43MpbvZ6/view?usp=sharing).

## Abstact
Robots are the best choice for rescue in many situations, such as in scenarios where there is nuclear radiation. For example, the leaks at the Chernobyl nuclear power plant and the Fukushima nuclear power plant in Japan.At the same time, remote control is often strongly interfered with in the presence of intense radiation, and the range of use of wired robots is very limited, so we want robots to be able to make their own choices in complex scenarios.This paper uses the reinforcement learning methods learned this semester: Q-learning and Deep Q learning to enable robots to make autonomous decisions about rescue solutions without human control. We make our robots learn in an abstract environment - similar to frozen lake.

## Overview
This project uses a deep reinforcement learning algorithm in association with a particle dynamics model to train agents to find the fastest path to evacuate a human from radioactive building with presence of the enemy.

Efficient emergency evacuation is crucial for survival. However, it is not clear if the application of the self-driven force of the social-force model results in optimal evacuation, especially in complex environments with obstacles of radiation. In this work, we developed a deep reinforcement learning algorithm in association with the social force model to train agents to find the fastest evacuation path. During training, we penalized every step of an agent in the room and gave zero reward at the exit. We adopted the Dyna-Q learning approach. We showed that our model can efficiently handle modeling of emergency evacuation in complex environments with multiple room exits and convex and concave obstacles where it is difficult to obtain an intuitive rule for fast evacuation using just the social force model.

![Game map](img/senario_2.png)

## Setup
*Note:* This code was designed to be used with Python 3.6.13, and is not compatible with later versions.

To install this project's package dependencies, please run the following command:

```
git clone https://github.com/oublalkhalid/Emergency-Path-Planning-in-radiation-world-Based-on-the-Deep-Q-Learning.git
cd Emergency-Path-Planning-in-radiation-world-Based-on-the-Deep-Q-Learning-main
```

```
pip install -r requirements.txt
```

```
cd main
python2 Controller.py
```

## Test
1. This project provides framework to train an agent for emergency evacuation in two scenarios.
- Please move to the main direction and run this command
```
python2 Controller.py
```

2. Our work on this project is summarized in a notebook that you can run in less than 10 minutes (in this case you don't need to install gym because here our environment has been built from scratch).
 
```
Emergency_Path_Planning_in_radiation_world_Based_on_the_Deep_Q_Learning.ipynb
```

- To display the environment made with gym AI open pose you have to run this command in the same main directory, please note that in this case you have to install the requirement before.

```
python?? path_project_env.py --env MiniGrid-ObstructedMaze-Full-v0
```
## Result

|   Simulation |   SARSA |   Qleraning |   DeepQlearning |
|-------------:|--------:|------------:|----------------:|
|            1 |   16318 |       17711 |           23304 |
|            2 |   16259 |       17881 |           23437 |
|            3 |   16590 |       17065 |           23469 |
|            4 |   16539 |       17217 |           23241 |
|            5 |   16421 |       17270 |           23234 |

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
