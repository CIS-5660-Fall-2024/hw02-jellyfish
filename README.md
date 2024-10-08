# Procedural Imposter Jellyfish

## Project Overview
In this homework, I created a... Jellyfish?

Just kidding, it's an octopus.

<img src="https://i.imgur.com/Nq92CNV.png"> 
<img src="https://i.imgur.com/5NTJJtX.png">
Gif: https://i.imgur.com/0ExZguv.gif

---
## Head
The head was created by bending a line using a combination of bend nodes, then revolving it and deforming it further with a mountain node. The head was given solidness through an extrude node as well. To create some veins on the octopus' head, I remeshed it selected some randomly scattered points at the top of the head, as well as some points near the middle of the head, and used the shortest path node. I also used the resample node to smooth out the veins, and used a sweep node to give it some volume.

## Tentacles
For the octopus's tentacles, I created a line with multiple points. In a for-each loop, I deformed the line with noise based on the iteration number in an attribute wrangle node since I wanted differently-shaped wiggles for each of the tentacles. Then, once I had the deformed line, I extruded a tube along the line, letting it taper off as it got closer to the end to create some varying thickness. I also added an additional tube on top of the tentacle to make it fuse more smoothly with the head.

## Suckers
I first created a sucker object that is a tube with a few extrude nodes applied on it. Then I selected the edge loops on the underside of the base tentacle, and used group promote to turn the group into a point group. Now that I had a point group, I used copy to points to create the suckers on the underside of each tentacle. 

I also wanted the suckers to shrink in size as the tentacle grew more narrow, so I created an attribute wrangle node to scale each sucker based on its Y-position.

## Webbing
Using a bunch of Poly Bridge nodes, I bridged the gaps between the tentacles and added a bit of deformation for that nice curve. This part is not as procedural, because I made the tentacles using a for-each loop. 

## Background
To create some seaweed and algae in the background, I ran some cloth simulations on a plane that was deformed using noise like in the instructions. 

## Rendering
I attempted to render this with Karma, with a few simple red and blue materials.
