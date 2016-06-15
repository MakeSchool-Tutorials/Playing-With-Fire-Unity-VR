---
title: "Playing With Fire"
slug: playing-with-fire-VR
---

Today we are going to learn to turn our hands into balls of fire so we can dance around a little space with flaming fire hands.

Step 1:

![image alt text](assets/image_0.png)

Let’s start the scene by adding a plane, make sure you put the plane at (0,0,0)

Also add a Camera Rig and SteamVR plugin from the SteamVR folder.

![image alt text](assets/image_1.png)

Next you want to build 4 walls, so please make 4 cubes and align them around the plane to give yourself 4 walls to be inside of.  We are going to do this so that we can have our lighting appear on the walls when we swing the fire around.

![image alt text](assets/image_2.png)

Next delete the directional light from the scene so it’s dark, and add the FireComplex particle system to each of your hands, we are going to modify this particle system to make it look a little more realistic.

![image alt text](assets/image_3.png)

Open the FireComplex particle system and change the SparksFalling section to use WorldSpace

Actually, change all of the different subsystems to use World Space (this means the particles will stay stationary when you move your hand instead of following your hand)

![image alt text](assets/image_4.png)

Next we are going to make the actual fire texture have a higher emission rate, and billboard differently so it looks more realistic while you move it around.  Please change these settings to this:

![image alt text](assets/image_5.png)

After you are done copy and paste the finished version of FireComplex into your other hand.

Now lets run and test..

You should have two fireballs hanging in your hands that you can wave around!  Really cool huh!

That is it!
