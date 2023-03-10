# Genetic algorithm python

## Problem

The problem under consideration is the landing of a rocket whose engine can be turned on or off every second. The engine is accelerating like a vertical rocket. The task is to land. That means having a low speed at a certain altitude. The bit pattern under consideration is the engine settings each second. Flight lasts a maximum of 200 units, hence we consider vectors of 200 bits.


Parameters of given problem:
- landing gain = 2000
- crash penalty = -1000
- height = 200
- starting velocity = 0
- gravity acceleration = 0.09
- force generated by engine = 45
- mass of fuel lost per second = 1
- landing height = 2
- maximum velocity during landing = 2
- roulet selection parameter = 1200


All parameters can be changed in [RocketSimulation.py](../RocketSimulation.py)
## Algorithm

[Algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm)
uses one-point crossover, roulette wheel selection with parameter. We look for best two parameters:
- crossing probability: the larger it is, the greater the exploitation
- mutation probability: the larger it is, the greater the exploration

## Required libraries
- random
- statistics
- abc
- copy
- numpy