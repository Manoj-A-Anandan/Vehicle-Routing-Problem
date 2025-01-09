# Vehicle Routing Problem (VRP) with Genetic Algorithms

This repository implements a solution to the Vehicle Routing Problem (VRP) using Genetic Algorithms (GA). The problem involves optimizing the routes of multiple vehicles to visit a set of locations while minimizing total travel distance and balancing the workload across vehicles.

## Features
- **Random Location Generation**: Generate random coordinates for locations and a central depot.
- **Genetic Algorithm Implementation**: Use the DEAP library to configure and execute the GA.
- **Multi-Objective Optimization**: Minimize total travel distance and balance vehicle workloads.
- **Visualization**: Display optimized routes using Matplotlib with unique colors for each vehicle.

---

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Implementation Details](#implementation-details)
4. [Example Output](#example-output)
5. [Contributing](#contributing)

---

## Installation

1. Clone the repository:
    ```bash
   git clone https://github.com/yourusername/vehicle-routing-problem.git
   cd vehicle-routing-problem
2. Install required libraries:
   ```bash
   pip install matplotlib deap
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Vehicle_Routing_Problem.ipynb

##Usage

1.Open the Vehicle_Routing_Problem.ipynb file in Jupyter Notebook.
2.Configure problem parameters in the notebook:
    num_locations: Number of locations to visit (e.g., 20).
    num_vehicles: Number of vehicles available (e.g., 3).
3.Run all cells to execute the genetic algorithm and visualize the results.

##Implementation Details
Problem Setup
    Locations: Randomly generated (x, y) coordinates within the range [0, 100].
    Depot: Fixed at (50, 50) as the starting and ending point for all vehicles.
Genetic Algorithm
    Representation: Each individual is a permutation of location indices.
Fitness Function:
    Objective 1: Minimize total travel distance.
    Objective 2: Minimize workload imbalance (measured as the standard deviation of distances across vehicles).
Operators:
    Crossover: Partially Matched Crossover (cxPartialyMatched).
    Mutation: Shuffle Mutation (mutShuffleIndexes).
    Selection: Tournament Selection.
Visualization
    Matplotlib is used to plot the optimized routes.
    Depot is marked as a red cross, locations as blue dots, and routes are drawn with unique colors for each vehicle.
    
##Example Output
Optimized Routes
    Depot is marked as a red cross (x).
    Locations are marked as blue dots.
    Each vehicle's route is represented with a distinct color.
Example visualization:

File Structure
```bash
.
├── Vehicle_Routing_Problem.ipynb   # Main project notebook
├── README.md                       # Project documentation
└── example_routes.png              # Example output visualization

##Contributing
Contributions are welcome! To contribute:

1.Fork the repository.
2.Create a new branch for your feature:
```bash
git checkout -b feature-name

3.Commit your changes:
```bash
git commit -m "Add new feature"

4.Push your branch:
```bash
git push origin feature-name

5.Submit a pull request.


