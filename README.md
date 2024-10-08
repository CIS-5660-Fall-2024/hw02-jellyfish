# Procedural Jellyfish

## Project Overview

https://github.com/user-attachments/assets/58e3a03c-8b41-42ed-944c-642a0c715fa8


## Bell and Arms
I followed Elyssa Chou's tutorials:

[Jellyfish Bell Setup Video](https://www.youtube.com/watch?v=J3X8BB0yNRE)

[Jellyfish Arms Setup Video](https://www.youtube.com/watch?v=A_oNXqx8XH4)

## Veins
I used remesh to triangulate the bell shape, then I created two groups for the start and end points respectively. I then used the Find Shortest Path node to create the vein shape and used subdivide, smooth, and fuse to make the veins look more natural. I then used the sweep node to give the veins width and used point deform to make the veins follow the motion of the bell.

## Organs
I bent a line, mirrored it, and transformed it to get the shape of a singular organ. I then used the sweep node to give it width and the mountain node to make the surface less uniform. I used point deform to follow the motion of the bell.


https://github.com/user-attachments/assets/890d0b1c-b17c-43e6-9e74-a5570b3bdd36



## Tentacles
I used [this video](https://www.youtube.com/watch?v=LN4XXaHQkmU) to simulate the tentacles like hairs


If I have extra time I would try rendering the jellyfish!
