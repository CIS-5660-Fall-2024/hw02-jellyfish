# Procedural Jellyfish
## Result
![](jellyfish.gif)
![](jellyfish_bg.gif)


## Implementation Details
### Bell and Arms
The bell was modeled based on a twice-bent linear line. Once the line bent to the desired shape, the Revolve Node was used to generate the Bell-Like model.
The arms were modeled using a twisted linear line and a noise function. 
![](attr.png)

### Veins
The veins were created by using the shortest path algorithm applied on the Bell surface edges.
![](vein.png)

### Organs
The organs were created from a linear twice-bent line as well.
![](organ.png)

### Extra
- Four different materials assigned to the models
![](mat.png)
- HDRI background environment
- Mantra animation render scene
