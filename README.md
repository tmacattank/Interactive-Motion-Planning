# Interactive Motion Planning
Codebase for adaptive interactive mixed-integer model predictive control (aiMPC): an optimal control-based interactive motion planning algorithm for autonomous vehicles.

- Real-time Software-in-the-loop simulation in CARLA with Human-in-the-loop capability.
- ROS (Noetic) for communication.

## Key dependencies:
- CARLA simulator
- Gurobi
- ROS Noetic
- MATLAB (data analysis)

### Test scenario illustration
Mandatory lane change scenario: a stopped truck on the right lane necessitates a lane change for the autonomous vehicle which needs to negotiate with a human-driven vehicle on the left lane.
![alt text](https://github.com/autonomous-viranjan/Interactive-Motion-Planning/blob/main/scenario.png)
- Blue vehicle is the ego vehicle and red vehicle is the human-driven neighboring vehicle (NV).

![shil](https://github.com/autonomous-viranjan/Interactive-Motion-Planning/assets/62226470/007e4ddd-783e-495a-a7bf-8f61333cc901)

aiMPC estimates NV's cost online and adapts the MPC.

### A case when ego merges ahead
https://github.com/autonomous-viranjan/Interactive-Motion-Planning/assets/62226470/80b97b3e-c7b9-4cf5-933c-67992a033649

### A case when ego merges behind
https://github.com/autonomous-viranjan/Interactive-Motion-Planning/assets/62226470/f22663f6-780c-471e-94e3-66f41bb8012c

### A case where the hunam-driven vehicle nature changes
https://github.com/autonomous-viranjan/Interactive-Motion-Planning/assets/62226470/bacb1f65-077f-4fc9-8c1b-87f18a4aafa8

- α\_p and α\_a are the estimated NV cost weights.
