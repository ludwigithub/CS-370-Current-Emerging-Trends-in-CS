# CS-370-Current-Emerging-Trends-in-CS

<b>Scenario</b><br>
You are working as an AI developer for a gaming company. The company is developing a treasure hunt game where the player needs to find the treasure before the pirates find it. As an AI developer, you have been asked to design an intelligent agent of the game for an NPC (non-player character) to represent the pirate. The pirate will need to navigate the game world, which consists of different pathways and obstacles, in order to find the treasure. The pirate agent’s goal is to find the treasure before the human player. This is commonly called a pathfinding problem, as the agent you create will need to find a path towards its goal.<br><br>
You have been provided with some starter code and a sample environment where your pirate agent will be placed. You will need to create a deep Q-learning algorithm to train your pirate agent. Finally, you have also been asked to write a design defense that demonstrates your understanding of the fundamental AI concepts involved in creating and training your intelligent agent.<br><br>
<b>Agent Specifications</b><br>
• You will use the Python programming language for this project, as well as the TensorFlow and
Keras libraries. These have been pre-installed in the Virtual Lab (Apporto).<br>
• The environment for your agent has already been designed as a maze (8x8 matrix), containing
free (1), occupied (0), and target (1 at the bottom right) cells, as below:<br><br>
 [ 1., 0., 1., 1., 1., 1., 1., 1.],<br>
 [ 1., 0., 1., 1., 1., 0., 1., 1.],<br>
 [ 1., 1., 1., 1., 0., 1., 0., 1.],<br>
 [ 1., 1., 1., 0., 1., 1., 1., 1.],<br>
 [ 1., 1., 0., 1., 1., 1., 1., 1.],<br>
 [ 1., 1., 1., 0., 1., 0., 0., 0.],<br>
 [ 1., 1., 1., 0., 1., 1., 1., 1.],<br>
 [ 1., 1., 1., 1., 0., 1., 1., 1.]<br><br>
• Your agent (pirate) should start at the top left. The agent can move in four directions: left, right,
up, and down.<br>
• The agent rewards vary from -1 point to 1 point. When the agent reaches the target, the reward
will be 1 point. Moving to an occupied cell will result in a penalty of -0.75 points. Attempting to
move outside the matrix boundary will result in a penalty of -0.8 points. Moving from a cell to an
adjacent cell will result in a penalty of -0.04 points, primarily to avoid the agent wandering
within the maze.<br>
• A negative threshold has been defined for you in order to reduce training time, avoid infinite
loops, and avoid unnecessary wandering.<br><br>
<b>Provided Elements</b><br>
Below is a brief description of the different elements involved in the game. Several elements have
already been given to you in the starter code. You will need to create the code for the Q-Training
Algorithm section yourself.<br><br>
<b>Environment</b><br>
(NOTE: You have been given this code)<br>
TreasureEnvironment.py contains complete code for your environment. It includes a maze object
defined as a matrix. The provided code supports methods for resetting the pirate position, updating the
state based on pirate movement, returning rewards based on agent movement guidelines, keeping track
of the state and total reward based on agent action, determining the current environment state and
game status, listing the valid actions from the current cell, and a visualization method for graphical
display of environment and agent action.<br><br>
<b>Experience for Replay</b><br>
(NOTE: You have been given this code)<br>
GameExperience.py contains complete code for experience replay. It stores the episodes, all the states
that come in between the initial state and the terminal state. This is later used by the agent for learning
by experience. The class supports methods for storing episodes in memory, predicting the next action
based on the current environment state, and returning input and targets from memory based on
specified data size.<br><br>
<b>Build Model</b><br>
(NOTE: You have been given this code)<br>
You have been given a complete implementation to build a neural network model in the
TreasureHuntGame Jupyter notebook. Make sure to review the code and note the number of layers, as
well as the activation, optimizer, and loss functions that are used to train the model.<br><br>
<b>Q-Training Algorithm</b><br>
----(NOTE: You will need to create this code)----<br>
You have been given a skeleton implementation in the TreasureHuntGame Jupyter Notebook. Your task
is to implement deep-Q learning. The goal of your deep Q-learning implementation is to find the best
possible navigation sequence that results in reaching the treasure cell while maximizing the reward. In
your implementation, you need to determine the optimal number of epochs to achieve a 100% win rate.<br><br>
<b>Play Game</b><br>
(NOTE: You have been given this code)<br>
You have been given a complete implementation of this function in the TreasureHuntGame Jupyter
notebook. This function helps you to determine whether the pirate can win any game at all. If your maze
is not well designed, the pirate may not be able to win, in which case your training may not yield any
result. The provided maze in this notebook ensures that there is a path to win and you can run this
method to check.<br><br>
<b>o	What do computer scientists do and why does it matter?</b><br>
Computer and information research scientists, including artificial intelligence specialists, invent and design new approaches to computing technology and find innovative uses for existing technology. They study and solve complex problems in computing for business, medicine, science, and other fields.<br><br>
<b>o	How do I approach a problem as a computer scientist?</b><br>
Step 1 – Identify the problem that must be solved.<br> 
Step 2 – Understand what the problem presents.<br>
Step 3 – Determine how to solve the problem.<br>
Step 4 – Develop a method to achieve the solution.
<br><br>
<b>o	What are my ethical responsibilities to the end user and the organization?</b>
As a computer scientist working with AI I will be responsible for data responsibility and privacy, fairness, explainability, robustness, transparency, environmental sustainability, inclusion, moral agency, value alignment, accountability, trust, and technology misuse.
<br><br>

<h6><i>How to become an AI and computer scientist - career girls - explore. Career Girls. (2023, September 25). https://www.careergirls.org/careers/computer-scientist/#:~:text=Computer%20and%20information%20research%20scientists,%2C%20science%2C%20and%20other%20fields. </h6>
<h6>Computer Programming Problem Solving Process. (n.d.-a). https://germanna.edu/sites/default/files/2022-05/Computer Programming Problem Solving Process.pdf </h6>
<h6>What is ai ethics?. IBM. (n.d.). https://www.ibm.com/topics/ai-ethics#:~:text=Examples%20of%20AI%20ethics%20issues,%2C%20trust%2C%20and%20technology%20misuse. </h6>


