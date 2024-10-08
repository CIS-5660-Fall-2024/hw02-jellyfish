# Procedural Jellyfish

## Project Overview
This a procedural jellyfish using Houdini. 

### Result
![Jellyfish](./output.gif)
[Video](./assets/output.mp4)

### Features
- Jellyfish modeling
- Animation
- Lighting
- Rendering
<img height="500" alt="Jellyfish Parts" src="/assets/JellyfishParts.png">

---

## Reference

[Geometry Nodes Documentation](https://www.sidefx.com/docs/houdini/nodes/sop/index.html)
[VEX Documentation](https://www.sidefx.com/docs/houdini/vex/functions/index.html)


## Houdini FAQ
[File Cache Node](https://www.youtube.com/watch?v=00s9YWDWFs0) - How do I use the File Cache node? Where does it save and how do versions work?
- Drop down the file cache node and the data will be save in disk. It saves time by caching the simulation data, so we don't need to recalculate everu time which saves time for rendering and playback.

[Simulation Caching](https://www.youtube.com/watch?v=jwIuzB9FkX0) - Why is my timeline turning blue/orange? Why isn't my simulation updating even though I made changes?
- Blue means houdini has all the geometry information cached in memory. Orange means the cache is out of the date. Houdini saves old information until users explicity tell it to update the information, cause sometimes we dont want to resimulate right after and freeze everything.

