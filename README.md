# Procedural Jellyfish  

## Project Overview  
I created a procedual jellyfish animation in Houdini for my Procedural Computer Graphics Class.  

https://github.com/user-attachments/assets/436f6ac0-829b-494a-9b0f-48a421c55d95

Scallopping was done by first assigning an angle attribute to all vertices in the bell:  
![image](https://github.com/user-attachments/assets/67d7a3db-fa5d-4b1f-888a-64cd74c39ff4)  
And then adding along their normals to vertices that are close to even divisions of 360. We also moved vertices down with amplitude based on their y-pos.  
![image](https://github.com/user-attachments/assets/a0ffe708-8c42-4853-9309-26e25673d4ea)  
 
