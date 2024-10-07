# Procedural Jellyfish

## Project Overview

I created my jellyfish with a the help of a combination of the given resources, figuring out my own solutions, and searching for other examples online

### Jellyfish

The bell and arms of the jellyfish were mostly built from the tutorial videos which were given to us. In short, the bell was made from bending a line primitive, revolving it around the vertical axis, extruding to give thickness, and using slight noise to make it less perfectly round. The arms were made from grids made wavy with VEX scripting, and twisted around before having cloth sim applied.

The jellyfish's veins, organs, and tentacles were made with more self-driven ideas. The veins came from generating shortest paths between a random selection of points around the remeshed bell. The cost function for the shortest path function was adjusted so that there was less cost for nodes higher in the y-axis, which incentivized the generation of paths upwards on the bell, rather than randomly around it.

The organs came from bending a line, rotating it so it laid flat and copying it around the y-axis, and then copying a sphere to the points along the lines. The spheres were fused with their neighbors, remeshed, smoothed, and adjusted with Mountain noise to create a kind of bumpy, goopy-looking organ system. 

The tentacles were relatively simple. I grabbed the bottom-most point of every line that was created when revolving around the y-axis for the bell, and I created a new line that dangled from that point. I then applied a hair simulation to the lines, and swept a circle along them to give them thickness.

### Scene

I also created a simple scene for the jellyfish to live in. This was a couple of coral formations and a sandy "floor". The corals were circles swept along bent lines and extruded (then fused/smoothed in the case of the large yellow coral) with a mountain node applied for some . Then, in the material for the corals I used fractal noise to create fine displacement to make them appear very rough. Similar noise was applied to create their blotchy coloration.

Simlar to the jellyfish's bell, the ground was a bent line revolved around the y axis. I then applied very slight mountain deformation to the remeshed result. The material for this was a lot more involved than the corals. The displacement is a combination of x-axis-stretched voronoi noise displaced with a sine function to break up the "rigid" feeling of its straight edges, and fractal noise to create finer bumps. The color was originally a flat brownish yellow. It was then modified by subtracting a dark color value based on fractal noise to create non-uniformity. After this, using the same voronoi noise output that drove the displacement map, a light color was added to the sand so that the higher ridges created by the noise appear slightly lighter in color.

## Rendered Video

https://github.com/user-attachments/assets/a4e268cc-9293-41b9-a943-5587e3cf3ad4


## Submission
- Fork this repository
- Update your README
    - Please delete the assignment README text
    - A description of your project
    - A video of your animated jellyfish ([video](https://www.youtube.com/watch?v=gXtDd1lPDmc) of how to save a video of your viewport out of Houdini)
- Create a pull request to this repository
- Submit your Houdini file to Canvas along with a link to your pull request
(Don't upload your houdini files to github -- it's a pain to upload big/binary files. Just canvas is fine!)
