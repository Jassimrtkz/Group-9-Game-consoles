# 🎮 Group 9 Embedded Game Console

The idea behind developing a multi-game embedded console as part of an engineering coursework assignment is described here. The device, coded fully in C and developed using the STM32 microcontroller, comprises three games inspired by the classics: **Micro Fighter** , **Tetris** , and **Flappy Bird**.

Unlike software-only implementations, this project operates under strict hardware and real-time constraints, requiring careful coordination between input handling, display updates, and system timing. The result is a responsive and interactive system that demonstrates practical embedded systems engineering rather than theoretical design.

---

## 🧠 System Overview

The system architecture is built around the idea of an event-driven system. Each game represents an individual system state.

Core design considerations included:
- Avoiding blocking delays to ensure responsiveness
- Ensuring constant processing of inputs (detection and debounce)
- Managing multiple hardware modules simultaneously with no timing issues
- Good code design for easy reusability, scalability, and readability

The system is an example of how embedded software has to find the right balance among hardware limitations, timing precision and efficiency.

---

## 🎮 Implemented Games

### 🥊 Micro Fighter
A fighting game that requires physical input from the user to start action sequences. The implementation will concentrate on:
- Fast and reliable input detection  
- Cooldown and action timing control  
- Immediate visual and audio feedback  

Interactivity and timely responsiveness are emphasized in this game.

---

### 🧩 Tetris
A well-structured, grid based game with collision detection and falling blocks. Important features include:
- Matrix/grid representation  
- Rotation and boundary validation  
- Continuous screen refresh logic  

Embedded systems programming with algorithmic considerations is shown here.

---

### 🐦 Flappy Bird
Vertical positioning accuracy is essential to avoid obstacles in this time critical game. This solution involves:
- Gravity and jump physics simulation  
- Obstacle spawning and movement  
- Score tracking and failure detection  

Real-time control and continuous updates are important aspects of this game

---

## ⚙️ Hardware Integration

Physical hardware is tightly coupled with this system:
- **STM32 Microcontroller** – core processing unit  
- **Push Buttons / Joystick** – user input  
- **LCD Display** – real-time game rendering  
- **LEDs** – status and event indication  
- **Buzzer** – audio feedback for actions and events  
- **(Optional) 7-Segment Display** – score/output display  

All HAL drivers have direct control over each hardware component making accurate scheduling crucial.

---

## 🧩 Software Design

Effective practices for embedded software design are demonstrated in the design of this project:

- Modular separation of game logic  
- Clear state-based control system  
- Non blocking timing using system ticks  
- Reusable input and output handling functions  

This allows the design to ensure that introducing new games doesn’t affect other functionalities.

---

## 🚀 Key Technical Achievements

- Real-time system with **no reliance on blocking delays**  
- Stable input processing using **debouncing and edge detection**  
- Multi-game integration within a **single embedded system**  
- Efficient handling of **hardware concurrency**  
- Clean and maintainable **modular C codebase**  

---

## 📂 Repository Structure
