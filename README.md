# Project 2: Continuous Control: README file

### 1. Introduction

The objective of the project is to train agents in the "Reacher" environment, where a set of double-jointed arms (aka the agents) have to stay within a target location. The agents have to stay within the target location, and for each timestep that the agents are inside the goal location, they are provided a score of +0.1. The goal of the agents is to maximize the reward. The environment is considered "solved" if the agents collect an average reward of 30 over 100 consecutive episodes.

Within the environment, each agent has a state associated with it. The space state consists of 33 variables that include the position, rotation, velocity, and angular velocities of the arm.

The available actions consist of four numbers in a vector, which correspond to the torque applied to the two joints. The values in the actions space should be in the range -1 to +1.

At each timestep, the agent has to select the action which will allow it to stay inside the target location.

### 2. Installing dependencies
To able to run the training environment, the following dependencies need to be installed:
Setup your environment per the instructions found in the README file in the following [link](https://github.com/udacity/deep-reinforcement-learning#dependencies)

Download the Unity environment from the link below that matches your operating system:
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

Please note that the environments above correspond to the second version of the project, which has twenty agents in the environment.

### 3. Running the scripts
The main file that will take care of initializing the environment, doing the training, and running a trained agent in the environment is the Continuous_Control.ipynb file. Before running this file, ensure that the following files are at the same location as the Continuous_Control.ipynb file:
- dqn_agent.py
- model.py
- Reacher.app
- checkpoint.pth

### 4. Importing all the libraries
To import all the required libraries, run the block of code in the first section of the Continuous_Control.ipynb script. This section is titled "Importing Libraries".

### 5. Taking random actions in the environment
To have an agent take random actions in the environment, follow the steps below:
1. Restart the jupyter notebook kernel
2. Run the code in section 1 of Continuous_Control.ipynb: "Importing Libraries"
3. Run the code in section 2 of Continuous_Control.ipynb: "Opening the environment and taking random actions"

### 6. Training an agent using Deep Deterministic Policy Gradient (DDPG)
To train an agent using DDPG, follow the steps below:
1. Restart the jupyter notebook kernel
2. Run the code in section 1 of Continuous_Control.ipynb: "Importing Libraries"
3. Run the code in section 3 of Continuous_Control.ipynb: "Training an agent"

### 7. Run a trained agent in the environment
To run a trained agent in the environment, follow the steps below:
1. Restart the jupyter notebook kernel
2. Run the code in section 1 of Continuous_Control.ipynb: "Importing Libraries"
3. Run the code in section 4 of Continuous_Control.ipynb: "Run environment using a trained agent (by importing a checkpoint)"

### 8. References
Please note that the code used originates from the DDPG code that was provided in the Udacity Deep Reinforcement Learning class, and then modifcations were done to make it applicable for the specific environment that was solved. Similarly, some of the content of the README file originates from the Udacity Deep Reinforcement Learning class, as well as from my submission for the first project of this class.