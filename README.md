

# 🚦 Automatic Traffic Light System with Pedestrian Button

This project implements an automatic traffic light system with a pedestrian button using **Simulink** and **Stateflow**. The project is divided into two milestones: an automatic traffic light system based on timers and a system with a pedestrian push button to control traffic and pedestrian lights.

## 📋 Project Overview

- **Milestone 1**: Automatic traffic light system controlled by a timer.
- **Milestone 2**: Traffic light system with a pedestrian button for dynamic control.

## 🛠️ System Components

- **Simulink Blocks**: 
  - **Counter Limited Block**: Controls timing for the lights (0-15 seconds).
  - **Relational & Logical Operator Blocks**: Evaluate conditions to switch traffic lights based on the timer.
  - **Lamp Block**: Visual representation of traffic light states (1 for on, 0 for off).
  - **Button Block**: Pedestrian button that triggers light changes.

- **Stateflow**:
  - Used to manage the overall logic and flow of the system, especially for handling the pedestrian button interaction.

## 💡 Features

### Milestone 1: Automatic Traffic Light System

- **Green Light**: Activated for the first 7 seconds.
- **Yellow Light**: Activated for the next 3 seconds.
- **Red Light**: Activated for the remaining 6 seconds, allowing pedestrians to cross.
- **Pedestrian Light**: Corresponds to the traffic light, turning green when the red traffic light is on and vice versa.

### Milestone 2: Traffic Light with Pedestrian Button

- **Pedestrian Button**: When pressed, the traffic light transitions to yellow for 3 seconds, then turns red, allowing pedestrians to cross.
- **Traffic Control**: After the pedestrian crossing period (6 seconds), the system resets to its initial state until the button is pressed again.

## ⚙️ Design & Methodology

### Milestone 1

1. **Counter Block**: The counter runs from 0 to 15 seconds, controlling the traffic and pedestrian lights based on the timer values.
2. **Logical Conditions**: The system checks the timer conditions and switches the lights accordingly:
   - Green light (0-7 seconds)
   - Yellow light (7-10 seconds)
   - Red light (10-16 seconds)

### Milestone 2

1. **Button Integration**: A momentary push button is used to interrupt the automatic flow.
2. **Stateflow Logic**: The system enters a new state when the button is pressed, turning the yellow light on for 3 seconds, followed by a red light and green pedestrian light for 6 seconds.
3. **Reset Mechanism**: The system returns to the green traffic light until the button is pressed again.

## 🔍 Results

- The system successfully demonstrates an automatic traffic light with dynamic pedestrian control using a push button.
- Visual feedback is provided using lamps to show real-time states of the traffic and pedestrian lights.

## 🧑‍💻 Members

- **Shirin Shujaa** (s3983427)
- **Dinh Ngoc Minh** (s3925113)
- **Ngo Nhat Anh Khoa** (s3924481)

