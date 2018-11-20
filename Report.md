In this project I solved a double-jointed arm environment where the goal of the agent was to maintain its position at the target location for as many time steps as possible.

The task was episodic and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

### Learning Algorithm:

The algorithm I used to solve the environment is DDPG - Deep Deterministic Policy Gradient.

I tried different network architectures for the model. I introduced more layers to actor and critic algorithms with different nodes, but none of these helped improve training. Below is the result for one of such unsuccessful attempts.

![Alt text](/Unsuccessful_training_results.png?raw=true "Unsuccessful Training Results")

Then I tried batch normalization with a simple two fully connected layer architecture with 128 nodes each layer. This improved training drastically.

Hyper parameters I used for the final ddpg algorithm:

![Alt text](/Hyperparameters_used.png?raw=true "Hyperparameters Used")


### Plot of Rewards:
Below is the plot and the final training average scores over 100 episodes.

![Alt text](/Final_results.png?raw=true "Final Training Results")

![Alt text](/Plot_of_average_score.png?raw=true "Plot of Scores")

### Ideas For Future Work:
I would like to try different alsorithms like PPO, A3C for both the first and the second version of the environment. I would be interested to see how these algorithms would perform with respect to each other in both these environments.
