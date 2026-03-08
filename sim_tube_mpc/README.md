# Python MVP Simulation for Ellipsoidal Tube MPC

This README provides an overview of the Python MVP simulation for Ellipsoidal Tube Model Predictive Control (MPC) used in a 10-dimensional quadrotor environment. The simulation includes necessary models and disturbance dynamics for effective control strategies.

## Requirements
- Python 3.x
- numpy
- scipy

## Files Included
- `requirements.txt`: Dependencies for the simulation environment.
- `quad10_model.py`: The quadrotor model in a 10D state space.
- `disturbance.py`: Models disturbances affecting the quadrotor.
- `ellipsoid_tube.py`: Implements the ellipsoidal tube MPC logic.
- `simulate_mvp.py`: The main simulation script that utilizes the above models.

## Usage
1. Install the requirements:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the main simulation:
   ```bash
   python simulate_mvp.py
   ```
