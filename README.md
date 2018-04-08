# LivelyLemurs
SEP Project

---
08/04|Luke - Added Destructible wall  
How to implement:  
Before moving to project, open plugins and enable Apex destruction.   
Then open the destructible mesh and click "Fracture mesh" on the top bar.  
Then open the blueprint and select the destructible mesh under destructible component.  
Unbind the cast to in the blueprint's event graph as it will be a bad cast unless you have a FirstPersonProjectile.  
You can use the following in the Player blueprint to test destruction until we have weapons:  
![Q to destroy](https://i.imgur.com/uemY9Dr.jpg)   

---
