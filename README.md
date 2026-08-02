# robot-dog-2D
# 🦾 Quadruped Robot - Mechanical Design

A simple quadruped robot mechanical design created in **Onshape** as part of the Smart Methods Robotics training program.

## 📌 Overview

The goal of this project is to design the mechanical structure of a quadruped robot and understand the basic principles of robotic locomotion, joint movement, and stability.

## ✨ Features

- Simple robot body design
- Four articulated legs
- Two joints per leg (Hip & Knee)
- Revolute joints for rotational movement
- Mechanical assembly in Onshape
- Motion testing using Assembly Mates
- Designed for future servo motor integration

## ⚙️ Mechanical Specifications

| Item | Description |
|------|-------------|
| Robot Type | Quadruped Robot |
| CAD Software | Onshape |
| Number of Legs | 4 |
| Joints per Leg | 2 |
| Total Degrees of Freedom | 8 DOF |
| Proposed Actuator | MG996R Servo Motor |

## 🦿 Leg Design

Each leg consists of two mechanical segments:

- Upper Leg (Hip Link)
- Lower Leg (Knee Link)

The two-link design increases the robot's range of motion and allows smoother walking compared to a single rigid leg. Each joint is connected using a revolute joint, enabling rotational movement similar to biological quadruped robots.

## 🚶 Walking Gait

The robot is designed to use a **Crawl Gait**, where one leg moves at a time while the remaining three legs maintain stability.

## 🔩 Actuator Selection

The **MG996R Servo Motor** was selected for this design because:

- Provides accurate angular position control.
- Delivers approximately **11 kg·cm** torque at 6V.
- Suitable for lightweight robotic prototypes.
- Easy to interface with microcontrollers such as Arduino.
- Commonly used in educational robotics projects.

 ## 📐 Preliminary Torque Calculation
 
 The effective leg length was estimated by combining the upper and lower leg segments.

A preliminary torque calculation was performed for one hip joint.

**Assumptions:**
- Leg length: **53.6 mm (0.0536 m)**
- Estimated leg mass: **0.05 kg**
- Gravity: **9.81 m/s²**

**Calculation:**

Force = Mass × Gravity

Force = 0.05 × 9.81 = **0.49 N**

Torque = Force × Distance

Torque = 0.49 × 0.0536 = **0.026 N·m**

The calculated torque is significantly lower than the output torque of the selected **MG996R servo motor**, making it suitable for this mechanical design.

## ⚖️ Stability

The robot is designed with a symmetrical body to improve balance.

The battery, controller, and other electronic components are intended to be placed near the center of the chassis to keep the center of gravity low.

The selected Crawl Gait also increases stability by keeping three legs in contact with the ground while one leg moves.

## ⚠️ Expected Challenges

- Joint friction
- Servo torque limitations
- Balance during walking
- Mechanical interference between moving parts

## 📸 Preview

<img width="1012" height="681" alt="Screenshot 2026-08-01 180519" src="https://github.com/user-attachments/assets/c8514ac2-63f9-4f92-b898-76bba15c81c9" />


## 🛠️ Software Used

- Onshape

