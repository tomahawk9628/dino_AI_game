# Dino Game AI #
## Game ##
The game itself was developed with the Pygame module

## Algorithm ##
The NEAT algorithm has been used to make a game bot. The population size were sat to 100.

## Executables ##
Executable files for the various games versions are available on Google Drive: 
</br>
https://drive.google.com/drive/folders/1Ja0M3glcI24QX3gdBDFocFeqnV16XQ_L?usp=sharing
</br>
Just download zip folder , unzip it and click on .exe file to play or observe. There are 3 exe files in the directory:
1. Dino_GG_KB_HighDifficulty.exe: Keyboard controlled high difficulty (both cactus and ptera as obstacles) playable game.
2. Dino_GG_KB_LowDifficulty.exe: Keyboard controlled low difficulty (only cactus as obstacle) playable game.
3. Dino_GG_AI.exe: AI controlled non-playable game. It just shows Ai learning to play the game using NEAT algorithm.

```bash
NOTE: Do not delete any other files or folder from extracted directory as it contains game dependencies.
```

## Dependencies ##
The game were created in pygame. And neat-python was used to run the neat algorithm.
```bash
pip install pygame
pip install neat
```


## Neural network
The neural network is a simple feed forward network with 5 inputs and 2 outputs.

Input nodes (5):
1. Dinosaur y-position
2. Next obstacle y-position
3. Next obstacle x-position
4. Obstacle after that's y-position
5. Obstacle after that's x-position

Output nodes (2):
1. Jump or not jump
2. Duck or not duck

## Fitness function
The genomes were rewarded with 0.1 points each tick they managed to stay alive. Given a frame rate at 60 ticks per second, the reward is equivalent to 6 points per second.

The genome with the highst score were selected.

