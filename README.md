# OpenSim-SecondLife-Rigging-Guide

Hi everyone! This is a guide on how to rig and import custom models inside OpenSim/OSGrid/Second Life.
We will be using a vanilla Blender installation (As of time of writing this, version 4.5.3, but every other version should be fine). No weird addons or other programs.
So, let's start. (This guide assumes you know how to use Blender and have some basics about rigging and fixing models/vertex groups. I will try my best to write it simple and easy for everyone!)

0. Download the OpenSimSimpleSkeleton.blend from the repo and open it inside Blender. You will see something like this:

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr1.png)]

That's the default SL model. We need to delete it. Click it with left mouse button, then right click and press delete.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr2.png)]

Now, it should be like this:

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr3.png)]

1. Import your model (Here you are on your own, since there are tons of different models format and ways to acquire them!)
After the import, you should have something like this:

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr4.png)]

2. Move the model and allign to the SL Skeleton.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr5.png)

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr6.png)]

Be sure to Apply the Visual Geometry to Mesh as you see here, so that the mesh remains in T-Pose!

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr7.png)]

3. Remove the old Vertex Groups (if any) to clean up the model properly.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr8.png)]

4. Remove the original skeleton of our imported model (if any).

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr9.png)]

If your model reset their default pose when the skeleton is deleted, simply move it back to their original spot by rotating and resizing the mesh.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr10.png)]

5. Go in Edit Mode and optimize the model by Merging all vertices (this can help us a lot by semplifying the rigging process)

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr11.png)]

6. Choose the Skeleton and the Model, click CTRL+P and click Armature Deform with Automatic Weight. If everything has been done properly, the rigging should be automatic and not throw any issue. If Blender throws us some errors, we need to split manually some mesh elements to semplify it (My best bet is to always separate hair, accessories and extra clothes from the model).

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr12.png)]

The mesh looks fine, even if some stuff is not properly rigged! We need to fix it manually. Let's go into Edit mode after clicking the model.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr13.png)]

For comfort, I usually leave on all the armature options as you can see here, so that I can properly choose the faulty meshes and fix them easily and in real time.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr14.png)]

Now it looks fine!

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr15.png)]

7. Lets put back the model in T-Pose and select both skeleton and the mesh, so that we can export them.

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr17.png)]

8. Export them as Collada (.DAE)

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr18.png)]

Be sure to check those options!

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr192021.png)]

9. Let's import it into OpenSim/SL:

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr22.png)]

It looks nice! Texture-less, but nice! Now we need to check the following options in the various tabs: Generate normals and Include joints positions.

10. Let's click Calculate Weight and Cost.

11. Let's import our textures separately (Yeah, it's boring, I know!)

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr26.png)]

12. Let's wear our mesh from our inventory and apply textures on it (Click on it -> Modify -> Select Faces -> Apply textures in the correct faces)

At the end of the day, you should have something like this:

![alt text](https://github.com/IlBowmany/OpenSim-SecondLife-Rigging-Guide/blob/main/Screenshots/Scr28.png)]

It looks nice overall! It may need some more tweaking, but for the purpouse of this guide, I think it is more than enough!

Thanks for following the guide, hope you enjoyed it. See you on the OpenGrid!







