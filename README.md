# Micromouse Autonomous Robot

An ESP32-S3 autonomous maze-solving robot that combines sensing, maze mapping, route planning, and closed-loop motion control.

![Micromouse robot](https://haribood.github.io/micromouse1.jpeg)

## Overview

The robot uses four infrared sensors, wheel encoders, and IMU feedback to navigate a maze. C/C++ firmware maps the maze and plans a route to the target, while motor drivers execute movement under feedback control.

## Hardware and software

| Component | Role |
|-----------|------|
| ESP32-S3 | Embedded controller |
| Four IR sensors | Maze and wall sensing |
| Wheel encoders | Motion feedback |
| IMU | Orientation feedback |
| Motor drivers | Motor actuation |
| C/C++ firmware | Mapping, route planning, and motion control |

## Control and navigation

1. Read sensor feedback to observe the robot's surroundings and motion.
2. Update the maze map and plan a route to the target.
3. Execute movement with closed-loop motor control.
4. Use feedback to correct motion as the robot progresses.

The project combines navigation decisions with a **500 Hz motion-control loop**, equivalent to one update every 2 ms.

## Reported performance

- Motion-control frequency: **500 Hz**.
- Stopping accuracy: **1 mm or better**, as reported in the project portfolio.

These figures describe the build's reported results. A detailed test procedure and measurement dataset are not included in this repository yet.

## Project media

The photo above comes from my portfolio. Additional photos and demonstrations are available in the [project gallery](https://haribood.github.io/#projects).

## Repository status

This repository currently contains project documentation. Firmware, wiring diagrams, a bill of materials, and calibration instructions have not yet been uploaded, so this is not yet a reproducible build package.

## Author

[Haridev Nambood](https://github.com/haribood) — electrical engineering student at the University of Houston.

[Portfolio and project details](https://haribood.github.io/#projects)
