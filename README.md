# BiologicalSimulation 🌱🧬

A Python simulation of biological interactions using Pygame. This simulation includes entities such as Bots, Red Blood Cells (RBCs), Tumors, Immune Cells, and Viruses, each with unique behaviors and interactions.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Classes and Their Roles](#classes-and-their-roles)
6. [Future Improvements](#future-improvements)
7. [License](#license)

## Introduction 📚
This project is a biological simulation designed to model interactions between various entities. The entities include:
- **Bots** 🤖
- **Red Blood Cells (RBCs)** 🩸
- **Tumors** 🎗️
- **Immune Cells** 🛡️
- **Viruses** 🦠

The simulation visualizes how these entities move, interact, and influence each other's behaviors in a controlled environment.

<p align="center">
  <img src="https://github.com/Rishit-katiyar/BiologicalSimulation/assets/167756997/8a9d382a-711f-4bad-aeae-0a6bb2108ce2" alt="image_15" width="200"/>
  <img src="https://github.com/Rishit-katiyar/BiologicalSimulation/assets/167756997/b01d2224-4f2c-4629-8b4f-0a7ff27017a8" alt="image_20" width="200"/>
  <img src="https://github.com/Rishit-katiyar/BiologicalSimulation/assets/167756997/9cc864a8-b589-4e49-a898-abe9befc7545" alt="image_5" width="200"/>
  <img src="https://github.com/Rishit-katiyar/BiologicalSimulation/assets/167756997/25b4df89-6b16-4848-888f-6074bcb8c470" alt="image_10" width="200"/>
</p>

## Features ✨
- Randomly generated entities with unique attributes.
- Movement and interaction logic for each entity.
- Collision detection and response.
- Energy and lifecycle management for Bots.
- Basic biological behaviors such as mutation, apoptosis, and DNA repair.

## Installation 🛠️

### Prerequisites
Make sure you have Python 3.7 or later installed. You can download Python from [python.org](https://www.python.org/).

### Step-by-Step Guide

1. **Clone the Repository**
    ```bash
    git clone https://github.com/yourusername/BiologicalSimulation.git
    cd BiologicalSimulation
    ```

2. **Create a Virtual Environment**
    ```bash
    python -m venv venv
    ```

3. **Activate the Virtual Environment**

    - On **Windows**:
        ```bash
        .\venv\Scripts\activate
        ```
    - On **macOS/Linux**:
        ```bash
        source venv/bin/activate
        ```

4. **Install the Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

5. **Run the Simulation**
    ```bash
    python simulation.py
    ```

### Requirements
Make sure to have the following libraries installed, which are listed in `requirements.txt`:
- pygame

To install them, run:
```bash
pip install pygame
```

## Usage 🚀

### Running the Simulation
After following the installation steps, run the simulation using:
```bash
python simulation.py
```

### Interacting with the Simulation
- The simulation window will open, displaying all the entities.
- The Bots will move around, interacting with RBCs, Tumors, Immune Cells, and Viruses.
- Press `ESC` or close the window to stop the simulation.

## Classes and Their Roles 🧑‍🔬

### Bot Class
- **Attributes**: Position, direction, life, energy, mutation rate, DNA damage, cycle progress, genes, inventory, skills.
- **Methods**: `move()`, `sense_tumor(tumors)`, `interact_rbc(rbcs)`, `apoptosis()`, `update_energy()`, `mutate()`, `repair_dna()`, `cell_cycle()`.

### RBC (Red Blood Cell) Class
- **Attributes**: Position, velocity.
- **Methods**: `move()`.

### Tumor Class
- **Attributes**: Position, growth rate, life, cytokines.
- **Methods**: `move()`, `proliferate()`, `undergo_apoptosis()`, `release_cytokines()`.

### ImmuneCell Class
- **Attributes**: Position, life, attack rate, antigen, response strength.
- **Methods**: `move()`, `attack_tumor(tumors)`, `attack_virus(viruses)`.

### Virus Class
- **Attributes**: Position, life, infectivity.
- **Methods**: `move()`, `replicate()`.

### CustomEnvironment Class
- **Attributes**: Lists of Bots, RBCs, Tumors, Immune Cells, and Viruses.
- **Methods**: `reset()`, `step()`, `render(screen)`.

## Future Improvements 🌟
- Enhance the interaction logic between entities.
- Introduce new entity types and behaviors.
- Add more detailed graphics and animations.
- Implement a GUI for more interactive controls.
- Include more sophisticated biological processes.

## License 📜
This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.
