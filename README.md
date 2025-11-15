[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/JB8SDF9g)
# LAB3
Note:

The demo script `adarrt.py` is written for Python 2 and is provided for reference only.

In Lab 3, both Python 2 and Python 3 versions of the script are already included in the Docker images provided (as referenced in the Overleaf file), depending on which version you choose to use.

The Lab 3 simulation supports both Python 2 and Python 3 implementations; however, the real-world lab only supports Python 2.

## Example Commands to Run Each Question

### 1. Default RRT Simulation (Question 3)

Runs the basic RRT planner without any smoothing. The robot executes the raw, unsmoothed RRT path.

```python
python ~/ros_ws/src/lab3/adarrt.py --sim
```

### 2. Smoothed Trajectory (Question 4)

Enables trajectory smoothing using ada.compute_smooth_joint_space_path() after the raw RRT path is generated.

```python
python ~/ros_ws/src/lab3/adarrt.py --sim --smooth
```

### 3. Goal-Biased Sampling (Question 5)

Enables goal-biased precise sampling: the RRT sampler will sample near the goal state with probability 0.2 and also lower the eps.

```python
python ~/ros_ws/src/lab3/adarrt.py --sim --smooth --precise 0.2
```
