# StarCraft 2 AI Comparisons

## Minigame - DefeatRoaches
### Repository
Link: [StarCraft 2 Reinforcement Learning](https://github.com/starcraft2-ai/rl-battle/)

### Agents
1. `Random agent`: as the name shows, it does things randomly
1. `A3C`: A3C method implemented in [our repository branch](https://github.com/starcraft2-ai/rl-battle/tree/A/C-online)
1. `A2C`: A2C method implemented in 
[our repository branch](https://github.com/starcraft2-ai/rl-battle/tree/joy-atari-loss)

### Results
| Metrics | Random agent | A3C | A2C |
| --- | --- | --- | --- |
| Mean Score | 1.81 | 3.4 | 13.69 |
| Max Score | 46 | 71 | 81 |


## Individual Comparison of different implmentation of Minigame
### Conparison Tool
See this [repo](https://github.com/starcraft2-ai/rl-battle/)

### Agents
1. `simon-a2c`: A2C method referenced from [a fork of simonmeister's repo](https://github.com/starcraft2-ai/simon-a2c), abbreviation as `simon-a2c`
2. `xhujoy-a3c`: [a fork of Xiaowei Hu's repo](https://github.com/starcraft2-ai/xhujoy-a3c)
2. `random agent`: as the name shows, it does things randomly

### Results
| Map | Training iters | simon-a2c | random agent | DeepMind human |
| --- | --- | --- | --- | --- |
| (mean) DefeatRoaches | 1000×16 = 16k | 5.74 | -4 | 41 |
| ( max ) DefeatRoaches | Same | 61.00 | 11 | 81 |
| (mean) DefeatZerglingsAndBanelings | 500×8 = 4k | 24.8 | 18.1  |  729 |
| ( max ) DefeatZerglingsAndBanelings | Same | 108.00 |72| 757 |
| (mean) MoveToBeacon | 5000×6 = 30k | 25.26 | 1.2 | 26 |
| ( max ) MoveToBeacon | Same | 30.00 | 3 | 28 |
| (mean) CollectMineralShards | 2000×4 = 8k | 23.84 | 18.5 | 133 |
| ( max ) CollectMineralShards | Same | 39.00 | 32 | 142 |
| (mean) FindAndDefeatZerglings | 500×8 = 4k | 4.82 | 5 | 46 |
| ( max ) FindAndDefeatZerglings | Same | 18.00 | 15 | 49 |
