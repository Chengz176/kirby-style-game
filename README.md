# Kirb Run
## Description
Kirb Run is a Kirby-like game implemented with [TypeScript](https://www.typescriptlang.org/), [Kaboom.js](https://kaboomjs.com/), and [React](https://react.dev/), and built with [Vite](https://vitejs.dev/). This project was based on the repo and tutorial[[2](https://github.com/Chengz176/kirby-style-game#references)] created by [JSLegend](https://github.com/JSLegendDev), and additional features and modifications were implemented. The main purpose of this project is to learn and have some experience on TypeScript and different packages, frameworks, and algorithms.

## Details About the Game
- Spritesheet is from the repo created by JSLegend
- The player controls a character called Kirb to explore the map and the goal is to reach the exit door
- There will be enemies to prevent player from reaching the door
  - **Guy**: The enemy wanders around on the platform
  - **Flame**: The enemy that can jump and throw fireballs
  - **Bird**: The enemy that flies around where a truncated normal distribution sampler, implemented based on the algorithm proposed by Nicolas Chopin[[1](https://github.com/Chengz176/kirby-style-game#references)], is used in determining the direction to fly
- Kirb can inhales enemies, shoot stars, and absorb abilities from enemies
- There will be a timer to keep track of time and a mini-map to keep track the position of the player relative to the map
- Each map is generated by a map generator implemented with references on WFC SimpleTiledModel[[4](https://github.com/Chengz176/kirby-style-game#references)] and N-WFC[[5](https://github.com/Chengz176/kirby-style-game#references)].
- The map generator can generated the map with a seed generated by a pseudorandom number generator implemented based on Lehmer random number generator [[3](https://github.com/Chengz176/kirby-style-game#references)].
- Two different game modes
  - **Select Map**: Play a specific map by providing the seed of the map
  - **Rounds**: Play a certain number of rounds where the map of each round is generated by the generator 

## Demo
Try out the game [here](https://chengz176.github.io/kirby-like-game/)

## References
[1] Chopin, N. (2012). Fast simulation of truncated Gaussian distributions. arXiv preprint arXiv:1201.6140

[2] JSLegend, "Kirby like Platformer Game made with TypeScript + Kaboom.js", https://github.com/JSLegendDev/Kirby-like-ts

[3] "Lehmer random number generator", https://en.wikipedia.org/wiki/Lehmer_random_number_generator

[4] Maxim Gumin, "WaveFunctionCollapse", https://github.com/mxgmn/WaveFunctionCollapse

[5] Nie, Y., Zheng, S., Zhuang, Z., & Song, X. (2023). Extend Wave Function Collapse to Large-Scale Content Generation. arXiv preprint arXiv:2308.07307



