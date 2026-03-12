# Smart Adaptive Traffic Intersection Simulator

An Android-based simulation of an intelligent traffic control system that dynamically adjusts traffic light phases based on vehicle and pedestrian demand.

The goal of this project is to explore how adaptive signal control can improve traffic flow, reduce congestion, and increase safety for pedestrians and vulnerable road users.

---

## Project Overview

Traditional traffic lights operate on fixed timers regardless of traffic conditions. This project implements an **adaptive traffic signal controller** that evaluates real-time demand and adjusts signal timing accordingly.

The system simulates:

- Vehicle arrivals at an intersection
- Pedestrian crossing requests
- Dynamic signal phase changes
- Traffic flow through the intersection
- Performance metrics such as throughput and queue length

The simulation is visualized in real time through a custom Android view representing the intersection.

---

## Key Features

### Adaptive Signal Control
The traffic controller dynamically allocates green time based on demand:

- Vehicle queue length
- Pedestrian requests
- Anti-starvation logic to ensure fairness

### Traffic Simulation
Traffic arrivals are generated using a stochastic model to simulate real-world conditions.

### Pedestrian Support
Pedestrian crossings are handled safely with priority weighting and dedicated signal phases.

### Accessibility-Oriented Design
The system can be extended to support:

- Accessible crossing requests for visually impaired users
- Audio signals for crossing assistance
- Extended crossing time for mobility-impaired pedestrians

### Real-Time Visualization
A custom Android view renders:

- Traffic lights
- Road intersection
- Queue lengths
- Current signal phase
- Performance metrics

---

## Technologies Used

- **Java**
- **Android Studio**
- Custom Android Views (Canvas drawing)
- Event-driven simulation
- Adaptive control algorithms

---

## System Architecture

The project is structured into several main components:

**IntersectionState**

Maintains the current state of the system including:

- signal phase
- vehicle queues
- pedestrian requests
- performance statistics

**AdaptiveSignalController**

Implements the adaptive traffic signal algorithm responsible for:

- phase transitions
- demand-based green time allocation
- fairness and starvation prevention

**ArrivalGenerator**

Simulates stochastic vehicle and pedestrian arrivals at the intersection.

**IntersectionView**

Custom Android view that renders the intersection and traffic signals in real time.

**MainActivity**

Controls the simulation loop, UI interaction, and updates the visualization.

---

## Simulation Metrics

The system tracks performance metrics including:

- Average queue length
- Vehicle throughput
- Pedestrian crossings
- Signal phase duration

These metrics help evaluate the effectiveness of adaptive signal control.

---

## Future Improvements

Potential extensions include:

- Emergency vehicle priority
- Multi-intersection coordination
- Machine learning based traffic prediction
- Real-world sensor integration (IoT traffic detection)
- Hardware prototype using microcontrollers

---

## Motivation

Urban traffic congestion and pedestrian safety remain major challenges in modern cities. Adaptive traffic control systems offer a promising approach to improving intersection efficiency while prioritizing vulnerable road users.

This project explores how such systems can be designed, simulated, and eventually implemented using intelligent control strategies.

---

## Author

Banele Mjali  
BSc Computer Science and Economics  
University of the Witwatersrand
