# Procedural Jellyfish

## Project Overview


https://github.com/user-attachments/assets/eeb5cc44-820f-48d7-a899-758d73e14b85


https://github.com/user-attachments/assets/e03c8345-b445-4f9b-8e5b-48e22b586277




---

## Inspiration
![jelly](https://github.com/user-attachments/assets/e975c671-e482-44f1-aac6-c0cf873d4e7d)
![_](https://github.com/user-attachments/assets/42d641c4-40ad-4746-9b7d-f6d0d76ebebe)

I tried creating a more animated jelly fish with more exaggerated movement and appearance.

## Bell & Arms

I followed the tutorial videos, playing around with different values and transformations to achieve the effect I wanted.

[Jellyfish Bell Setup Video](https://www.youtube.com/watch?v=J3X8BB0yNRE)

[Jellyfish Arms Setup Video](https://www.youtube.com/watch?v=A_oNXqx8XH4)

## Veins

I remeshed the jelly fish bell into triangles, and used two Groups to select some start and end nodes for Find Shortest Path. Then I used Smooth and adjusted the Shortest Path settings to achieve a more brain-like vein effect. Then I used Sweep to extrude the veins into rounded tubes, and Point Deform similarly to the jellyfish arms to attach the veins to move with the animated bell.

## Organs

I drew a Bezier Curve in a C shape, then used Sweep to make it 3D, and rotated it to make it conform more to the jellyfish bell shape above it. Then I copied it 3 more times, and used Point Deform with an Extract Centroid node to make the organs move with the bell.

## Tentacles

I followed the hair simulation youtube video to create my tentacles, making a group of points along the rim of the jelly fish to use with Copy To Points to extrude lines out. Then I simulated more natural movement using Vellum Hair with Vellum Solver, where I struggled to get the Vellum Solver to render the hair with the moving points group, but I fixed it by adjusting some Pin Type settings in Vellum Hair. 
