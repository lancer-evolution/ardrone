# 概要

Parrot社のAR.droneを使った研究をするための開発環境の構築

## Run Simulator

tum_simulator
```bash
roslaunch cvg_sim_gazebo ardrone_testworld.launch
```
![](/pict/sim.png)

## Run Driver

For AR.drone
```bash
roslaunch tum_ardrone ardrone_driver.launch
```
```bash
rosrun ardrone_autonomy ardrone_driver
```
## tum_ardrone

state estimation
```bash
rosrun tum_ardrone drone_stateestimation
```
auto pilot
```bash
rosrun tum_ardrone drone_autopilot
```
gui
```bash
rosrun tum_ardrone drone_gui
```
↑Abobe launch
```bash
roslaunch tum_ardrone tum_ardrone.launch
```
![](/pict/autopilot.png)



