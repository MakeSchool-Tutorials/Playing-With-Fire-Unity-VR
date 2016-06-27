---
title: "Playing With Fire"
slug: playing-with-fire
---

Today we are going to learn to turn our hands into balls of fire so we can dance around a little space with flaming fire hands.

>[action]
>Create a new 3D Unity Project.

<!-- -->

>[action]
>Then set the Scene by adding a plane. Make sure you put the plane at (0,0,0)

![image alt text](assets/image_0.png)

Now we are going to need to import SteamVR into the project so that we can get the hand controllers and control our HMD.

>[action]
>Open the Asset Store, search for SteamVR, and Download and import it.
![Download SteamVR](assets/image09.png "Download SteamVR")

<!-- -->

>[action]
>Click the "import" button to import once it downloads, and then "accept all" of the default settings. Unity should congratulate you for this wise decision.

![Download SteamVR](assets/import.png)

![Download SteamVR](assets/accept.png)

![Download SteamVR](assets/accepted.png)

The glowing blue box will be your walking play area. You will be able to walk around this region and interact with objects inside of it.

>[action]
>From the SteamVR/Prefabs folder add a Camera Rig and SteamVR Prefab.

![image alt text](assets/image_1.png)

The blue box represents the recommended walking area.

![The rig](assets/rig.png "Download SteamVR")

>[action]
>Next you want to build 4 walls, so please make 4 cubes and align them around the plane to give yourself 4 walls to be inside of.  We are going to do this so that we can have our lighting appear on the walls when we swing the fire around.

![image alt text](assets/image_2.png)

>[action]
>Now delete the Main Camera from your Scene.  We don't want it here, because the Prefab we dragged in already has a camera! If you leave this camera in, Unity will yell at you for having two Audio Listeners in your Scene. More importantly, you really don't want the old camera, because it's not connected to your HMD anyway!

![The camera](assets/camera.png)

We're going to get a cool fire effect to put on our hands from the Standard Assets. In order to do this next step, you will have needed to download Standard Assets when you downloaded Unity. If you don't remember whether or not you did, you probably did, because it should have been the default for you.

>[action]
>Import Standard ParticleSystem Assets (Assets->Import Package->ParticleSystem, and then click the "import" button).

![import particles](assets/importParticles.png)

>[action]
>Next delete the directional light from the scene so it’s dark, and add the FireComplex particle system (Standard Assets/ParticleSystems/Prefabs) to each of your hands.

![image alt text](assets/image_3.png)

We are going to modify this particle system to make it look a little more realistic.

>[action]
>Open the FireComplex particle system and change the SparksFalling section to use WorldSpace

![image alt text](assets/image_4.png)

>[action]
>Actually, change all of the different subsystems to use World Space (this means the particles will stay stationary when you move your hand instead of following your hand)

Next we are going to make the actual fire texture have a higher emission rate, and billboard differently so it looks more realistic while you move it around.

>[action]
>Please change these settings to this (Emission Rate = 10, Max Particles = 50, Render Mode = Billboard):

![image alt text](assets/image_5.png)

>[action]After you are done copy and paste the finished version of FireComplex into your other hand.

<!-- -->

>[action]
>Now lets run and test..

You should have two fireballs hanging in your hands that you can wave around! Really cool huh!
That is it!

If you'd like to try a challenge to extend this project, try any of the following:

- Make the fire shift through the colors of the rainbow!
- Make the fire emit faster or slower depending on how quickly you move your hands
- Make the fire briefly light the ground whenever it touches it!
- Put the fire at the ends of chains you can swing around from your hands like [fire poi](https://en.wikipedia.org/wiki/Poi_(performance_art))!  (This one's pretty challenging!)
