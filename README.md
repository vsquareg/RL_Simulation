# RL_Simulation

**Work in progress**

This project is meant to be the decision making module of the autonomous bot for participation in the Robomasters AI Challenge. It utilizes pyMunk and pyGame to simulate in 2-D the enemy and friendly bots in the designated arena (as provided). It attemtps to explore all the arising possibilities during the match and find the best decisions to take under given circumstances.

## Dependencies
- pyMunk
- numPy
- pyGame
- matplotlib
- keras
- tensorflow (for computational backend)

## Files
- **learning.py :** Exploration and training of the deep neural network.
- **nn.py :** Defines the deep neural network layers and loss function using keras.
- **playing.py :** Runs the game after training (no exploration).
- **plotting.py :** Converts csv files generated during training into graphs for visualization and further optimization.
- **arenaGame.py :** Defines the characterticis of the arena and bots, alongwith running the pyGame simulations.

## Installing Dependencies

### pyGame

pyGame dependencies install:

`sudo apt install mercurial libfreetype6-dev libsdl-dev libsdl-image1.2-dev libsdl-ttf2.0-dev libsmpeg-dev libportmidi-dev libavformat-dev libsdl-mixer1.2-dev libswscale-dev libjpeg-dev`

pyGame install:

`pip3 install hg+http://bitbucket.org/pygame/pygame`

### pyMunk

Physics engine 

Download using:

`wget https://github.com/viblo/pymunk/archive/pymunk-4.0.0.tar.gz`

Unpack:

`tar zxvf pymunk-4.0.0.tar.gz`

Install:

`cd ..`
`python3 setup.py install`

### numPy, matplotlib, keras, tensorlow

Install using:

`pip install library_name`

## Training

`python3 learning.py`

Model would be saved to the folder 'saved-models'. Parameters for training can be adjusted from the file 'learning.py' itself.

## Playing

`python3 playing.py`

Model name can be changes from the file itself.

## Plotting

`python3 plotting.py`

**Entire project extended and modified from https://github.com/harvitronix/reinforcement-learning-car/**
