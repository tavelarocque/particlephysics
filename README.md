[particlephysics-README.md](https://github.com/user-attachments/files/26127110/particlephysics-README.md)
# Particle Physics Simulator

An interactive browser-based physics simulation that renders hundreds of particles bouncing and colliding in real time — built entirely with the HTML5 Canvas API and vanilla JavaScript.

![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Canvas API](https://img.shields.io/badge/Canvas_API-black?style=flat)

## Live Demo

[View on GitHub Pages](https://tavelarocque.github.io/particlephysics)

## Features

- **Real-time particle simulation** — dozens of particles with independent velocity, mass, and direction
- **Collision detection** — particles react when they hit each other and the canvas walls
- **Smooth animation** — powered by `requestAnimationFrame` for a consistent 60fps game loop
- **Interactive canvas** — built purely on the HTML5 Canvas API, no libraries

## Tech Used

- Vanilla JavaScript — object-oriented particle system, vector math, game loop architecture
- HTML5 Canvas API — 2D rendering context, `requestAnimationFrame`
- CSS — full-screen layout, dark background

## Getting Started

1. Clone the repo
   ```bash
   git clone https://github.com/tavelarocque/particlephysics.git
   cd particlephysics
   ```

2. Open `index.html` in your browser — no install or build step needed

## Project Structure

```
particlephysics/
├── index.html   # All simulation logic and rendering in one file
└── README.md
```

## How It Works

Each particle is represented as an object with properties for position (`x`, `y`), velocity (`vx`, `vy`), radius, and colour. On every frame:

1. Each particle's position is updated by its velocity
2. Boundary collision is checked — velocity is reversed on the relevant axis when a wall is hit
3. Particle-to-particle collision is detected using distance calculations between centres
4. The canvas is cleared and all particles are redrawn

## What I Learned

- Implementing a game loop using `requestAnimationFrame`
- Vector math for velocity, direction, and collision response
- Managing and updating many independent objects efficiently on the canvas
- Frame-by-frame rendering without any external libraries
