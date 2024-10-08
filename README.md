# Procedural Jellyfish : Lewis Ghrist

#Bell / Veins
The bell was made using the instructed method with a base curve deformed using bend nodes and revolving the curve to form the base shape. From there that surface is extruded and some slight noise is added to give the shape some variation. From the base mesh, I group some 'start' points towards the top of the bell and some 'end' points towards the bottom edge which are used with a shortest path node to create the veins. Values in the bend nodes and a transform node animates the bell to deform like it is swimming.

![][Bell_V1.png]

#Organs
The organs are made up of a simple bent capsule shape copied around in a circle and a larger structure made from a simple smoke simulation turned into polygons and mirrored across the xy and zy planes.

![][OrgansImage_V1.png]

#Tenticles
The tentacles where made using an edge swept along a base curve and then mirrored for symmetry. This allowed me to adjust the size of the tentacle using a curve which adjusts pscale. The result is then deformed using a lower frequency curl noise and a higher frequency aa noise. This is then twisted about the base curve axis and copied around to get multiple tentacles. This setup is put through a cloth simulation with a bit of noise to give the underwater effect. 

![][10_V1.png]

#Arms
The arms were made by copying some base edges to a circle whose points are on the inner side face of the bell's extrusion. These lines are then run through another cloth sim to get the deformation. 

![][Arms_V1.png]

#Materials
The materials is a mix of attribute magic and a camera fall of node. These are passed through some gradients and used to drive base color, emission, and opacity. The render is done in Karma and some bloom and color adjustments were made in post usin Davinci Resolve. 

![][Jelly_Vid_V1]