# AI Self-Driving Car Simulation

This repository showcases a simulation project for AI-based self-driving cars implemented in Python. The simulation integrates **neural networks** and **NEAT (NeuroEvolution of Augmenting Topologies)** to enable cars to learn and improve their driving performance autonomously.

## Project Overview
This project demonstrates the following key concepts:

- **AI Neural Networks**: The self-driving behavior is powered by neural networks.
- **NEAT Algorithm**: Used to evolve the neural networks to enhance driving capabilities.
- **Physics-Based Car Simulation**: A lightweight simulation that enables virtual cars to interact realistically with the environment.

The project includes multiple components, such as car physics, configuration files, and a main script for execution.

---

## Features

1. **Car Simulation**: Basic simulation of self-driving cars with realistic behavior.
2. **NEAT Integration**: Cars evolve and improve over time using the NEAT algorithm.
3. **Fully Configurable**: Parameters for the neural networks, cars, and environment can be tuned easily.
4. **Visualization**: Real-time graphical representation of the cars and their behavior in the environment.

---

## File Structure

```
📂 AI-SelfDriving-Simulation
|-- car.py                # Handles car physics and movement logic
|-- road.py
|-- world.py
|-- vect2d.py
|-- config_variables.py   # Stores all configurable variables for the simulation
|-- config_text.txt      # Configuration file for NEAT algorithm
|-- node.py
|-- main.py               # Main file to run the simulation
|-- README.md             # Project documentation
```

---

## Requirements

Make sure the following dependencies are installed:

- **Python 3.8+**
- **pygame** (For graphical visualization)
- **NEAT-Python** (For evolving neural networks)

You can install the dependencies using:
```bash
pip install pygame neat-python
```

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/gurinder-25/Protoype_AI
   ```

2. Run the simulation:
   ```bash
   python main.py
   ```

3. Watch as cars evolve and learn to navigate the environment over multiple generations!

---

## How It Works

1. **NEAT Algorithm**:
   - NEAT evolves neural networks generation by generation to optimize their performance.
   - Each car acts as an individual in the population and is evaluated based on its fitness (e.g., distance traveled).

2. **Car Logic**:
   - The `car.py` file controls the movement and collision logic for each car.
   - Sensors detect nearby obstacles, and the neural network decides the next action (e.g., steer, accelerate).

3. **Configuration**:
   - All NEAT-related parameters can be modified in `config_text.txt`.
   - Simulation variables like car speed, sensor range, and number of generations are stored in `config_variables.py`.

---

## Future Improvements
This project can be extended to include:
- Advanced environments (e.g., intersections, traffic signals).
- More complex neural network architectures.
- Reinforcement learning methods in addition to NEAT.

---

## Author
Created by **GURINDER SINGH**

---

## Acknowledgments
- **NEAT-Python** library for evolutionary neural networks.
- **Pygame** for the visualization framework.

