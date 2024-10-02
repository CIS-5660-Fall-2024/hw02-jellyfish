# Procedural Jellyfish

My project is a blue jellyfish:<br>
![image](https://github.com/user-attachments/assets/a2fe3238-27db-4be7-87bc-92f498e9f5cd)

For the bell, I followed what we did in class closely, and animated it moving up and down. The other body parts all follow the movement. The veins are shortest paths from a group on top to the bottom of the bell, the arms are twisted grids simulated using cloth simulation. To get the underwater effect, I decreased gravity and added velocity damping. The tentacles are hair simulation, where I added lines to a torus at the bottom of the bell, then I swept a tube that had a decreasing size as it went down to make it look better. The hair sim also had added forces to make it seem like it was flowing in water, and I addded wind drag and velocity damping to slow down movement. The organs are just bent and copied lines that were swept over. 

EC:<br>
![image](https://github.com/user-attachments/assets/da0b3be8-cf49-4267-b481-ebe2563abbd6)
![image](https://github.com/user-attachments/assets/d3f6b34c-7c7f-42fe-ac17-c269a846ea31)

For EC, I added L-System coral to the scene. The L-System is similar to a tree but with shorter branches, more branches and probailities attached to every branch to make it seem more random. I also added colour to each coral using materials (I used material nodes to make sure the coral didn't shine in the scene, which was happening before). For the background, I couldn't find an underwater hdr for some reason so I just used the sky.

Render: (the coral materials didn't show up in the render and the background angle is different for some reason, see video for an idea of what the scene actually looks like)
![image](https://github.com/user-attachments/assets/ef76be21-03ae-403f-8381-f23d60ae590b)

Video: https://github.com/virajdoshi02/hw02-jellyfish/blob/main/jellyRecording.mp4
