# Jellyfish

Simple jellyfish following base homework instructions



https://github.com/user-attachments/assets/0a0c8510-78f5-42d9-bb5b-08e3ffa5e5b0

# Veins
Using the non-extruded bell shape, I re-meshed and, using two group ranges, added the shortest-path node to create veins.
To add some slight curvature, I applied the smooth node and proceeded to sweep before applying the final point deform node.

# Organs
I used a drawn curve, resampled it, and then used a sweep node before subdividing it and adding a mountain node for surface deformation.
To make four organs, I used a copy node to rotate by the number of organs before using the same point deform technique from the arms.

# Tentacles
Using the sides from the poly-extruded bell, I applied a blast node and a match-size with a circle + ray node to get points for my hair (a mix of the tutorial and advice from a friend).
I attached hairs by using the copy node onto the points on the circle and then used a vellum hair solver.


