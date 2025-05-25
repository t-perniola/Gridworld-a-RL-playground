# Gridworld-a-RL-playground
The Gridworld environment is one of the most naive choices that can be made for the purpose of testing RL algorithms.
In particular, we created two different types of the gridworld environment: a standard one, with a starting and an ending cell, which represents the agent's final goal, and a second one, similar to the first one but enriched with diamonds, that act as intermediate rewards.
The notebook contains most of the approaches to deal with the RL tasks. We experimented all the three different "paradigms" of methods to solve the RL problem:
1) the tabular approach
2) the value approximation methods
3) the policy gradient methods

Starting from the Tabular approach, we tried to:
1.1) experiment the contextual multi-armed bandit problem, before delving deeper into the RL problem;
1.2) solve the prediction problem using the TD(0) approach;
1.2) solve the control problem using both the SARSA and the Q-learning algorithms (TD methods);

Then, we changed to the Value approximation methods, where:
2.1) to solve the control problem, we used the DQN algo (that is a value-approximation version of Q-learning) in the standard gridworld environment, with and without the experience replay mechanism, in order to highlight the differences in the performances obtained by the agent.
2.2) as before but in the diamond gridworld.

Finally, we tried the Policy gradient methods:
3.1) REINFORCE with and without the baseline
3.2) A2C
3.3) PPO
