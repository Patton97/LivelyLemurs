# LivelyLemurs
SEP Project

---  
17/04|Luke- Added Fan  
Should plug and play  
Folder structure should be Content>TopDownBP>Interaction>Fan  
Folder structure matters for importing files so make sure it matches or you'll have to rebind textures and mats  
Edited folder Structure in git to support this, should work by just copying the 2 top level folders to TopDownBP  

---  
16/04|Luke - Added Lava  
Should plug and play, again player damage part is currently based on my Topdowncharacter.  
Folder structure should be Content>TopDownBP>DamageAreas>Lava  

---
15/04|Luke - Added Electric gate  
Requires MacroVars from my BaseAI folder for the nickel textures on walls, feel free to change to fit level.  
Otherwise should plug&play, though may need adapting towards different topdowncharacter for now.   
Folder structure should be Content>TopDownBP>DamageAreas>ElecWall   
If lightning material is unbound from the grid, open the blueprint and select all the meshes that are children under the grid component and re-apply the material to them  

---
08/04|Luke - Added Destructible wall  
Folder structure should be Content>TopDownBP>Interaction>DestructibleWall  
How to implement:  
Before moving to project, open plugins and enable Apex destruction.   
Then open the destructible mesh and click "Fracture mesh" on the top bar.  
Then open the blueprint and select the destructible mesh under destructible component.  
Unbind the cast to in the blueprint's event graph as it will be a bad cast unless you have a FirstPersonProjectile.  
You can use the following in the Player blueprint to test destruction until we have weapons:  
![Q to destroy](https://i.imgur.com/uemY9Dr.jpg)   

---

