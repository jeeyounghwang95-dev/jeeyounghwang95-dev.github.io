---
title: "roboHand"
excerpt: "A Unity 3D robot-arm game that teaches the real-world limitations of Vision-Language-Action (VLA) models through gameplay<br/><img src='/images/robohand-screenshot.png'>"
collection: portfolio
---

![roboHand gameplay](/images/robohand-screenshot.png)

## Overview
roboHand is a first-person robot-arm manipulation game built in Unity, designed to let players experience — through gamification — the core challenges real VLA (Vision-Language-Action) models face: ambiguous natural-language instructions, visual confusion between similar objects, and the lack of tactile feedback when inferring grip force.

VLA models are becoming increasingly important in physical AI and robotics, yet intuitive educational tools for understanding them are scarce. Traditional robotics education has low accessibility due to hardware cost and safety concerns, and simulator-based education often struggles with learner motivation. roboHand tackles this gap through game mechanics.

## Tech Stack
- **Engine**: Unity
- **Language**: C#
- **Input**: Unity Input System

## Gameplay
- Players control the robot arm's XZ movement, vertical pick-up motion, and gripper force directly via keyboard (arrow keys, spacebar, Z/X)
- 9 missions total, each with a 30-second time limit — +100 points on success, -30 on failure

## Game Mechanics Mapped to VLA Concepts
| Game Element | Corresponding VLA Challenge |
|---|---|
| Ambiguous natural-language mission text (e.g., "Put the red fruit in the red bowl") | Language ambiguity / instruction interpretation |
| Mixed objects with similar color/shape (apple/pomegranate/mango, broccoli/artichoke, etc.) | Visual object-classification limits |
| Lighting phase changes (day → evening → sunset → night) | Recognition invariance under changing environments |
| Gripper force control (too weak = slips, too strong = crushes) | Grip-force control without tactile input |
| VLA insight popup shown after success | Concept explanation and metacognitive reflection |

## Educational Design
- A mission pool built around color, shape, and material confusion lets players directly experience real VLA failure modes
- An immediate feedback loop — explaining the cause of failure (wrong object/bowl) and allowing retries — helps learners infer for themselves why a VLA model might make mistakes
- Lighting shifts every two missions so the same object can be perceived differently depending on the environment

## Potential Applications
A low-cost way to build intuition for how VLA models work and where they fail, without needing physical robots — and one that could be extended into a human-vs-AI comparison learning platform by integrating an actual VLA inference engine.

## My Role
- Designed and implemented the full Unity game system (robot-arm control, gripper physics, mission/game state management)
- Designed the content and research mapping VLA education concepts onto game mechanics

## Links
- [GitHub](https://github.com/jeeyounghwang95-dev/roboHand)
