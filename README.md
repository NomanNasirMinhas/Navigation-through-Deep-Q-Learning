# Project Overview
For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

# Completing Criteria
**The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.**

# Environment
We will use environment simulation of Unity application **Banana**.
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:
- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

# Installing Dependecies
We will use following lines to install dependencies
- !pip -q install ./python
- from unityagents import UnityEnvironment                    
- from dqn_agent import Agent
- from collections import deque

# Instructions
Run each cell sequentially to train and evaluate the agent.

# Training Sessions
We will run 8 training sessions. For each session, we will save weights into a file. For each session we train agent with different parameters.

# Training Parameters
We used following parameters to train our agent.
* _eps_start_ with random value from 0.988 to 0.955 with step 0.001, 
* _fc1_units_ with random value from 54 to 128 with step 32,
* _fc2_inits_ with random value from fc1_units - 8 to fc1_units - 8 with step 8.

# Training Results
We used 8 training sessions and got following results for each session.
1. fc1_units:  54 , fc2_units:  46
- train_numb:  0 eps_start:  0.99
- Episode: 639, elapsed: 0:14:11.673203, Avg.Score: 13.00,  score 14.0, How many scores >= 13: 53, eps.: 0.08
- terminating at episode : 639 ave reward reached +13 over 100 episodes

2. fc1_units:  118 , fc2_units:  118
- train_numb:  1 eps_start:  0.992
- Episode: 634, elapsed: 0:14:09.634947, Avg.Score: 13.01,  score 15.0, How many scores >= 13: 53, eps.: 0.08
- terminating at episode : 634 ave reward reached +13 over 100 episodes

3. fc1_units:  54 , fc2_units:  46
- train_numb:  2 eps_start:  0.993
- Episode: 613, elapsed: 0:13:40.427706, Avg.Score: 13.00,  score 13.0, How many scores >= 13: 59, eps.: 0.09
- terminating at episode : 613 ave reward reached +13 over 100 episodes

4. fc1_units:  54 , fc2_units:  46
- train_numb:  3 eps_start:  0.988
- Episode: 629, elapsed: 0:14:01.435002, Avg.Score: 13.00,  score 19.0, How many scores >= 13: 58, eps.: 0.08
- terminating at episode : 629 ave reward reached +13 over 100 episodes

5. fc1_units:  54 , fc2_units:  54
- train_numb:  4 eps_start:  0.991
- Episode: 588, elapsed: 0:13:10.050657, Avg.Score: 13.00,  score 17.0, How many scores >= 13: 57, eps.: 0.09
- terminating at episode : 588 ave reward reached +13 over 100 episodes

6. fc1_units:  54 , fc2_units:  46
- train_numb:  5 eps_start:  0.992
- Episode: 583, elapsed: 0:13:04.717450, Avg.Score: 13.05,  score 18.0, How many scores >= 13: 55, eps.: 0.10
- terminating at episode : 583 ave reward reached +13 over 100 episodes

7. fc1_units:  118 , fc2_units:  110
- train_numb:  6 eps_start:  0.988
- Episode: 634, elapsed: 0:14:14.761383, Avg.Score: 13.05,  score 21.0, How many scores >= 13: 60, eps.: 0.08
- terminating at episode : 634 ave reward reached +13 over 100 episodes

8. fc1_units:  86 , fc2_units:  78
- train_numb:  7 eps_start:  0.991
- Episode: 534, elapsed: 0:11:59.747946, Avg.Score: 13.03,  score 15.0, How many scores >= 13: 57, eps.: 0.12
- terminating at episode : 534 ave reward reached +13 over 100 episodes

# Testing Results

Train: 0, Test: 0, Episode: 639, fc1_units: 54, fc2_units: 46, eps_start: 0.99, Score: 8.0
Train: 0, Test: 1, Episode: 639, fc1_units: 54, fc2_units: 46, eps_start: 0.99, Score: 7.0
Train: 0, Test: 2, Episode: 639, fc1_units: 54, fc2_units: 46, eps_start: 0.99, Score: 6.0
Train: 0, Test: 3, Episode: 639, fc1_units: 54, fc2_units: 46, eps_start: 0.99, Score: 12.0
Train: 0, Test: 4, Episode: 639, fc1_units: 54, fc2_units: 46, eps_start: 0.99, Score: 10.0
Train: 0, Test: 5, Episode: 639, fc1_units: 54, fc2_units: 46, eps_start: 0.99, Score: 13.0
       Average Score:  9.33333333333
=========================================================
Train: 1, Test: 0, Episode: 634, fc1_units: 118, fc2_units: 118, eps_start: 0.992, Score: 12.0
Train: 1, Test: 1, Episode: 634, fc1_units: 118, fc2_units: 118, eps_start: 0.992, Score: 18.0
Train: 1, Test: 2, Episode: 634, fc1_units: 118, fc2_units: 118, eps_start: 0.992, Score: 14.0
Train: 1, Test: 3, Episode: 634, fc1_units: 118, fc2_units: 118, eps_start: 0.992, Score: 15.0
Train: 1, Test: 4, Episode: 634, fc1_units: 118, fc2_units: 118, eps_start: 0.992, Score: 13.0
Train: 1, Test: 5, Episode: 634, fc1_units: 118, fc2_units: 118, eps_start: 0.992, Score: 19.0
       Average Score:  15.1666666667
=========================================================
Train: 2, Test: 0, Episode: 613, fc1_units: 54, fc2_units: 46, eps_start: 0.993, Score: 14.0
Train: 2, Test: 1, Episode: 613, fc1_units: 54, fc2_units: 46, eps_start: 0.993, Score: 20.0
Train: 2, Test: 2, Episode: 613, fc1_units: 54, fc2_units: 46, eps_start: 0.993, Score: 19.0
Train: 2, Test: 3, Episode: 613, fc1_units: 54, fc2_units: 46, eps_start: 0.993, Score: 19.0
Train: 2, Test: 4, Episode: 613, fc1_units: 54, fc2_units: 46, eps_start: 0.993, Score: 19.0
Train: 2, Test: 5, Episode: 613, fc1_units: 54, fc2_units: 46, eps_start: 0.993, Score: 15.0
       Average Score:  17.6666666667
=========================================================
Train: 3, Test: 0, Episode: 629, fc1_units: 54, fc2_units: 46, eps_start: 0.988, Score: 7.0
Train: 3, Test: 1, Episode: 629, fc1_units: 54, fc2_units: 46, eps_start: 0.988, Score: 12.0
Train: 3, Test: 2, Episode: 629, fc1_units: 54, fc2_units: 46, eps_start: 0.988, Score: 18.0
Train: 3, Test: 3, Episode: 629, fc1_units: 54, fc2_units: 46, eps_start: 0.988, Score: 22.0
Train: 3, Test: 4, Episode: 629, fc1_units: 54, fc2_units: 46, eps_start: 0.988, Score: 17.0
Train: 3, Test: 5, Episode: 629, fc1_units: 54, fc2_units: 46, eps_start: 0.988, Score: 17.0
       Average Score:  15.5
=========================================================
Train: 4, Test: 0, Episode: 588, fc1_units: 54, fc2_units: 54, eps_start: 0.991, Score: 11.0
Train: 4, Test: 1, Episode: 588, fc1_units: 54, fc2_units: 54, eps_start: 0.991, Score: 8.0
Train: 4, Test: 2, Episode: 588, fc1_units: 54, fc2_units: 54, eps_start: 0.991, Score: 12.0
Train: 4, Test: 3, Episode: 588, fc1_units: 54, fc2_units: 54, eps_start: 0.991, Score: 16.0
Train: 4, Test: 4, Episode: 588, fc1_units: 54, fc2_units: 54, eps_start: 0.991, Score: 14.0
Train: 4, Test: 5, Episode: 588, fc1_units: 54, fc2_units: 54, eps_start: 0.991, Score: 16.0
       Average Score:  12.8333333333
=========================================================
Train: 5, Test: 0, Episode: 583, fc1_units: 54, fc2_units: 46, eps_start: 0.992, Score: 15.0
Train: 5, Test: 1, Episode: 583, fc1_units: 54, fc2_units: 46, eps_start: 0.992, Score: 12.0
Train: 5, Test: 2, Episode: 583, fc1_units: 54, fc2_units: 46, eps_start: 0.992, Score: 13.0
Train: 5, Test: 3, Episode: 583, fc1_units: 54, fc2_units: 46, eps_start: 0.992, Score: 16.0
Train: 5, Test: 4, Episode: 583, fc1_units: 54, fc2_units: 46, eps_start: 0.992, Score: 13.0
Train: 5, Test: 5, Episode: 583, fc1_units: 54, fc2_units: 46, eps_start: 0.992, Score: 15.0
       Average Score:  14.0
=========================================================
Train: 6, Test: 0, Episode: 634, fc1_units: 118, fc2_units: 110, eps_start: 0.988, Score: 12.0
Train: 6, Test: 1, Episode: 634, fc1_units: 118, fc2_units: 110, eps_start: 0.988, Score: 16.0
Train: 6, Test: 2, Episode: 634, fc1_units: 118, fc2_units: 110, eps_start: 0.988, Score: 14.0
Train: 6, Test: 3, Episode: 634, fc1_units: 118, fc2_units: 110, eps_start: 0.988, Score: 14.0
Train: 6, Test: 4, Episode: 634, fc1_units: 118, fc2_units: 110, eps_start: 0.988, Score: 19.0
Train: 6, Test: 5, Episode: 634, fc1_units: 118, fc2_units: 110, eps_start: 0.988, Score: 20.0
       Average Score:  15.8333333333
=========================================================
Train: 7, Test: 0, Episode: 534, fc1_units: 86, fc2_units: 78, eps_start: 0.991, Score: 14.0
Train: 7, Test: 1, Episode: 534, fc1_units: 86, fc2_units: 78, eps_start: 0.991, Score: 16.0
Train: 7, Test: 2, Episode: 534, fc1_units: 86, fc2_units: 78, eps_start: 0.991, Score: 6.0
Train: 7, Test: 3, Episode: 534, fc1_units: 86, fc2_units: 78, eps_start: 0.991, Score: 18.0
Train: 7, Test: 4, Episode: 534, fc1_units: 86, fc2_units: 78, eps_start: 0.991, Score: 12.0
Train: 7, Test: 5, Episode: 534, fc1_units: 86, fc2_units: 78, eps_start: 0.991, Score: 15.0
       Average Score:  13.5
=========================================================
