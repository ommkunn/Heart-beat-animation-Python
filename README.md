# Beating Heart Animation in Python (Pygame)

## Overview

This project demonstrates a **beating heart animation** created using **Python and Pygame**.  
The idea was inspired by a scene from the drama *Lighter and Princess*, where a similar heart animation is rendered in a terminal using **C++**.

The objective of this project is **not to replicate the exact implementation**, but to recreate the concept using Python while understanding how graphical animations work.

---

## Background & Motivation

After watching *Lighter and Princess*, I became curious about how a beating heart could be generated purely through code. Since I had **not learned Pygame before**, I initially did not know that Python could handle real-time graphical animations like this.

To understand the approach, I explored the logic and concepts with the help of **ChatGPT** and **Claude**, focusing on learning rather than copying an existing solution.

This project represents an exploratory transition from a terminal-based C++ concept to a graphical Python implementation.

### Reference

![Reference Preview](https://github.com/ommkunn/Heart-beat-animation-Python/blob/main/Screenshot%20(145).png)

### What i got

![End Result](https://github.com/ommkunn/Heart-beat-animation-Python/blob/main/What%20i%20got.png)

---

## Tech Stack

- **Language:** Python 3  
- **Library:** Pygame  
- **Concepts Used:**  
  - Mathematical implicit equations  
  - Particle-based rendering  
  - Sinusoidal time-based animation  
  - Real-time rendering loop  

---

## Heart Shape Logic

The heart shape is defined using the following **implicit mathematical equation**:

### "(x² + y² − 1)³ − x²y³ ≤ 0"


### Explanation

- Random `(x, y)` coordinates are generated within a bounded range.
- Points satisfying the equation are selected.
- These valid points collectively form the heart shape.

---

## Heartbeat Animation Logic

- A time variable is continuously incremented.
- The heart scales dynamically using a sine function:

### "scale = base_scale × (1 + amplitude × sin(t))"


- This creates a smooth expand–contract motion resembling a heartbeat.
- The animation runs at **60 frames per second** for smooth visual output.

---

## Project Structure

├── heart_animation.py
└── README.md


---

## Installation

Ensure Python 3 is installed, then install Pygame:

```bash`
pip install pygame`

---
## License

This project is intended for **learning and experimentation purposes**.  
You are free to use, modify, and extend it.
