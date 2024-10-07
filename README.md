# Jellyfish Project

## Overview
This project involves creating a dynamic jellyfish model using procedural modeling techniques and custom materials. The initial steps for constructing the jellyfish's bell and arms were based on a tutorial video, while additional components were designed using resources available on the project's GitHub page.

## Implementation Details

### 1. Veins
- The veins were created by defining the start and end points, then connecting them using the shortest path algorithm.
- To introduce randomness, a `group range` node was used, giving the veins a more natural appearance.

### 2. Organs
- The organs were generated starting from a basic line, which was then modified using a `bend` node.
- A `sweep` operation was applied, adding randomness to the scale ramp to make the shape more organic.
- The resulting geometry was copied into four pieces and attached to the bell animation using a `point deform` node.

### 3. Tentacles
- The tentacles were constructed following the tutorial steps up until the `group expression` stage.
- A `point deform` node was used to attach the tentacles to the main body before passing them into the `vellum solver`.
- Solver data was customized to create a more natural movement for the tentacles.
- The simulation was saved to a file cache, similar to the approach used for the arms in the tutorial.

## Extra Credit

- **Materials:**
  - `Glass` material for the bell.
  - `Metal` material for the veins and tentacles.
  - `Plastic` material for the organs.
  - `Red velvet` material for the arms.

- **Lighting and Environment:**
  - An underwater HDRI skybox was added to create a realistic environment.
  - A point light was placed inside the jellyfish to enhance lighting effects and visibility.

- **Rendering:**
  - The final scene was rendered using Mantra.
  - All 100 frames were compiled into a video using Adobe Media Encoder.
