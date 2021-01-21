## ML-Agents Navigation
![gif](images/trained.gif)

The objective of this project is to train a machine learning agent to navigate around a large square world, collecting yellow bananas and avoiding blue ones.

## Environment
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. The goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

## Dependencies
Make sure you have python 3.6 installed and a virtual environment activated, then install the required packages torch, numpy and unityagents. They can be installed using pip:
```
python pip install torch 
```

## Running the Project
Browse to the project directory and run `train.py` to begin training. The trained weights are saved to the file `checkpoints.pth` once the required score is reached.

```
python train.py
```
Run `play.py` to watch an episode where a smart agent navigates around the world using the trained data.