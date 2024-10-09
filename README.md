# Procedural Jellyfish
Video: https://youtu.be/mwlYWLkgUik

Description:
Bell and Arms: I learned from Elyssa Chou's tutorial
Veins: I grouped the vertices of the upper part of the bell and the vertices of the lower part separately, then selected some from the top as start points and some from the bottom as end points. Using the shortest path method, I shaped them into veins, and then used a sweep node to make them in 3D. Finally, I attached them to the bell.
Tentacles: I grouped the lower part of the bell and scattered points on it. Then I created lines and used copy to points to make the lines grow from these points. I used a group expression node to select the lowest points of the lines, and in vellum constraints, I applied hair and pin constraints to pin the tentacles to the bell. Using point deform and enabling pin to animation, I made the tentacles move along with the bell's animation. I also adjusted some parameters to make the tentacles move more vividly.
Organs: I first drew the shape of organs using the curve tool, and then used a sweep to make it in 3D. After that, I used the fuse and smooth nodes to make the organs smoother.

Extra Credit: I uploaded a HDRI photo as the enviromental light source and added a spotlight. Credit: https://www.freepik.com/free-ai-image/fantasy-marine-landscape-with-bioluminescent-nature_138352245.htm#query=hdri%20underwater&position=3&from_view=keyword&track=ais_hybrid&uuid=f2cb0449-4ff3-4272-91fa-c3063f5c2f2b
I then used and adjusted materials from the material palette and then rendered my jellyfish. 


