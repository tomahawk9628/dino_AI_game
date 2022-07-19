# Dino Game AI(Work In Progress) #
## Game ##
The game itself was developed with the Pygame module
```bash
pip install pygame
```
##Algorithm
The NEAT algorithm has been used to make a game bot. The population size were sat to 100.




## Dependencies ##
The game were created in pygame. And neat-python was used to run the neat algorithm.
```bash
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

