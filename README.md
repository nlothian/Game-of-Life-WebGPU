# Game of Life on WebGPU

![Simulation demo](demo.gif)

A lightweight exploration of Conway's Game of Life rendered with WebGPU. Built while following Google's _Your first WebGPU app_ codelab and extended with a few QoL features.

## Overview

The project renders a game of life grid directly on the GPU, allowing for large scale real-time interaction and rapid parameter tweaks. This was a learning opportunity to become familiar with WebGPU and GPU pipelines.

## Features

- GPU-driven Life simulation with double-buffered compute and render passes
- Mouse brush for painting cells, including adjustable radius and softness
- On-the-fly control over grid resolution, cell scale, and simulation rate
- Minimal toggleable UI panel

## Running Locally

1. Clone the repo and install a lightweight static server (e.g. `npm install -g serve`).
2. Start the server from the project root (`serve .` or `npx live-server`).
3. Open the provided local URL in a WebGPU-enabled browser ([check here](https://caniuse.com/webgpu)).

## Controls

- **Grid Size X/Y:** Resize the simulation in real time.
- **Cell Scale:** Adjust pixel size per cell for zoomed-in or overview looks.
- **Simulation Speed:** Change number of steps simulated per frame
- **Brush Size:** Defines the radius of painted cells when clicking/dragging on the canvas.

## Credits

Inspired by Google's [Your first WebGPU app](https://codelabs.developers.google.com/your-first-webgpu-app). Additional tweaks, UI, and interaction polish by Alex Lothian (July 2025).
