# Dino Game AI #
## Game ##
The game itself was developed with the Pygame module
```bash
pip install pygame
```
You can also play it yourself by making the dino jump with the space bar.

## Agent ##
The agent file would contain the following modules
    -game
    -model
    Training:
        -state = get_state(game)
        -action = get_move(state)
            -model.predict()
        -reward, game_over, score = game.play_step(action)
        -new_state = get_state(game)
        -remember
        -model.train()

## Game(Pygame) ##
The Game.py file would contain the following modules
    -play_step(action)
        ->reward, game_over, score

## Model(Pytorch) ##
The Model.py file would contain the following modules
    Linear_QNet(DQN)
        -model.predict(state)
            ->action