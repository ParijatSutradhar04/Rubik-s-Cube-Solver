# Project Report: Rubik's Cube Solver using Reinforcement Learning

## Introduction
This project aims to develop an intelligent system capable of solving a Rubik's Cube using reinforcement learning (RL). A graphical user interface (GUI) based on Tkinter has been created, allowing users to interact with the cube by making moves or entering a valid shuffle by selecting colors on each face. The core of the project involves simulating cube movements, creating a reinforcement learning environment using Gym, and training RL agents to solve the cube.

## GUI Interface
### Design
The GUI interface, built with Tkinter, provides an intuitive platform for users to interact with the Rubik's Cube. The main features include:
- **Move Execution**: Users can execute standard Rubik's Cube moves.
- **Color Selection**: Users can select and place colors on each face of the cube to input a specific shuffle.
- **Shuffle Validation**: The system checks for the validity of the entered shuffle to ensure it represents a solvable cube state.

### Functionality
- **Move Interface**: Buttons and controls for executing moves such as rotations of each face (U, D, L, R, F, B).
- **Color Input**: A color palette for selecting and placing colors on the cube faces, ensuring a valid configuration.
- **Visualization**: Real-time 3D visualization of the cube's state to reflect user interactions and movements.

## Reinforcement Learning Environment
### Simulation of Cube Movements
The Rubik's Cube movements are simulated to reflect realistic behavior. This involves:
- **State Representation**: Encoding the cube's state in a format suitable for RL algorithms.
- **Move Simulation**: Implementing the logic for cube rotations and transitions between states.

### Gym Environment
The Gym library is used to create a custom environment for the Rubik's Cube. Key aspects include:
- **Action Space**: Defining the possible moves (actions) the agent can take.
- **Observation Space**: Representing the cube's state for the agent to observe.
- **Reward System**: Designing a reward mechanism to guide the agent towards solving the cube.

## Reinforcement Learning Agents
### Algorithms
Two reinforcement learning algorithms were employed to train the agents:
- **Double Deep Q-Network (DDQN)**: Enhances the traditional DQN by reducing overestimation of Q-values, leading to more stable and accurate learning.
- **Proximal Policy Optimization (PPO)**: A policy gradient method that improves training stability and sample efficiency.

### Training Process
- **Self-Learning**: The agents learn by repeatedly shuffling and solving the cube autonomously.
- **Exploration and Exploitation**: Balancing exploration of new moves and exploitation of learned strategies.
- **Long-term Training**: Extensive training sessions to allow the agent to experience a wide variety of shuffles and develop robust solving strategies.

### Results
The trained agents demonstrated the ability to solve the Rubik's Cube from various shuffled states. Key performance metrics include:
- **Solving Accuracy**: The percentage of successfully solved cubes.
- **Move Efficiency**: The average number of moves taken to solve the cube.
- **Learning Curve**: The progression of the agent's performance over training iterations.

## Conclusion
This project successfully developed a Rubik's Cube solver using reinforcement learning, integrating a user-friendly GUI and advanced RL algorithms. The system's ability to autonomously learn and solve the cube showcases the potential of RL in complex problem-solving tasks. Future improvements could involve optimizing the training process, enhancing the GUI for better user experience, and exploring additional RL techniques for improved performance.
