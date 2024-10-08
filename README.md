# Procedural Jellyfish

## Submission (Charles Wang)

https://github.com/user-attachments/assets/6117aad4-0e4d-4e37-86dc-818edc1deb84

## Bell and arms

I did nothing too special here, just followed the videos. I did adjust a few of the parameters though.

## Veins

Following Elyssa's videos, I used nodes to group by range to select points at the "top" and "bottom" of the bell, which become the start and end points of the shortest path node. I use resample and smooth nodes to make it less follow the triangles on the mesh, and then did point deform to make it move along with the bell.

## Organs

To create the organs, I started with a single line and use the bend node to bend both ends of the tips into a horseshoe shape. I then used the sweep node to create geometry for it, transformed it a little from the center, and copied 3 more copies of it. I then used the mountain node to slightly make the four organs look slightly different.

## Tentacles

For the tentacles, I used the vellum simulation just like the arms, except I changed the gravity to -18 so that the tentacles would stay down instead of jumping around. To make it follow the bell, I output the side geometry from the poly extrude node from the bell, which I then converted to points, which I used the copy a single line node from. I used a poly wire to give the curve actual geometry.
