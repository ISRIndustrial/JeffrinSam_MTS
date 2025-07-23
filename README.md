# JeffrinSam_MTS
Synthetic Data Generation – Generate synthetic joint data for Unitree H1/G1 robots via imitation learning in Isaac Lab. Simulate and visualize in Isaac Sim, enhance with Cosmos for realism, and combine with teleop data to fine-tune Gr00t N1.5 for pick-and-place tasks, tested in Isaac Sim (Inference).

## Overview
This project focuses on synthetic data generation and model fine-tuning for pick-and-place tasks using Unitree H1 and G1 robots. Leveraging Isaac Lab, Isaac Sim, ROS2, and RoboMimic, we generate synthetic joint data, train policies, simulate environments, and fine-tune models to enhance robotic performance.

## Task 1: Synthetic Data Generation for Unitree H1
- **Objective**: Generate synthetic joint position data for Unitree H1 to train a policy for pick-and-place tasks.  
- **Method**: Use imitation learning in Isaac Lab to create 10 → 1000 joint configurations. Train a mimic policy using RoboMimic.  
- **Tools**: Isaac Lab, RoboMimic.  
- **Output**: Synthetic dataset and a trained policy for pick-and-place tasks.
  
![Unitree H1 Joint Configuration](https://github.com/ISRIndustrial/JeffrinSam_MTS/raw/main/H1fps.png)

![Unitree H1 Simulation Snapshot](https://github.com/ISRIndustrial/JeffrinSam_MTS/raw/main/H1/Screenshot%20from%202025-07-23%2011-07-44.png)

## Task 2: Simulation and Fine-Tuning for Unitree G1
- **Objective**: Simulate pick-and-place tasks for Unitree G1 and fine-tune the Gr00t N1.5 model.  
- **Method**: Create a simulation environment in Isaac Sim with a ROS2 node to interface with Gr00t N1.5. Collect teleoperation data from both the simulation and the physical Unitree G1. Fine-tune Gr00t N1.5 and evaluate performance in Isaac Sim.  
- **Tools**: Isaac Sim, ROS2.  
- **Output**: Fine-tuned Gr00t N1.5 model with evaluated performance metrics (e.g., success rate).

![G1 Pick-and-Place Demo](https://github.com/ISRIndustrial/JeffrinSam_MTS/blob/cbf5fa4c100230c65b94fe34c76bd34bab0169ce/pick.gif?raw=true)
![H1 Synthetic Data Preview](https://github.com/ISRIndustrial/JeffrinSam_MTS/blob/cbf5fa4c100230c65b94fe34c76bd34bab0169ce/1%20(2).gif?raw=true)

## Dependencies
- Isaac Lab  
- Isaac Sim  
- ROS2  
- RoboMimic  

## Notes
- Cosmos integration for data realism is under development.  
- Current performance shows a 6/10 success rate for pick-and-place tasks in simulation.

## Future Work
- Enhance data realism with Cosmos.  
- Improve Gr00t N1.5 performance to increase the success rate.  
- Expand physical teleoperation data collection.
