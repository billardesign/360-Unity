# 360-Unity
## Creating a 3d environment for 360 Youtube and VR tools.
The idea behind this project was to create a room for the purposes of a character driven story
from a first person perspective, the viewer would take the role of the character and watch as the environment would change around her
showing what the character is experiencing with whether it personal, physical or psychological.
## Build 3D Box/Room
The first stage is to create the environment of the story which in this case is a room.
To create a room it is necessary to create a wall, to do this right-click in your hierarchy, go to 3D-object and select Cube.

![alt text][logo][1](https://cloud.githubusercontent.com/assets/20883838/17837022/414c7214-67b0-11e6-8f5b-eb0b5090e1a2.png)

After you have created a cube adjust its shape till it resembles one of the walls of your room, this can be done through the inspector or via the objects user-interface.
when it is the dimensions that you want copy the object and paste 3 more, these will all need to have their positions
individually adjusted and then placed under the same object category

![2](https://cloud.githubusercontent.com/assets/20883838/17837024/43a7e886-67b0-11e6-9e44-db35f8a0657e.png)

Now that you have a room built it is time to add assets to it, to do this you can either create your own using 3d modeling tools such as Maya, Z-brush, Google-Sketchup
and many others or you can import already made ones from the Unity Store or from Google-Sketchup.
## Lighting/Sunlight
To add light to your scene you will need to create game objects for the light the natural light will be automatically provided by the Unity
when your project is initially created, you can adjust it via its rotation to control intensity and time of day (dawn, dusk, noon etc).
if you want to add light source to one of your objects that you have create or imported then you will need to create a pointlight game object, this can be done via the GameObject tab.
## Camera Setup
When a new project is created a camera object will be provided, this acts as the main camera for the scene and game.
Place the camera where you want in the scene, for the purpose of creating a 360 vr experience place the camera in the center of your 3D enviroment,
the direction of the camera will not affect the vr as the 360 vr will allow the player to see in any direction.
## Panoramic Script
To create the 360 vr video it is necessary to attach a script that records your game using a panoramic tool,
this script can be found online in the Unity store for free [(click here)](https://www.assetstore.unity3d.com/en/#!/content/38755). 
This script comes with a Read Me file explaining how it functions, when you have installed the script into your assets folder,
drag and drop the script file from your assets on the camera game object in the hierarchy afterwards go to the camera GameObject and
through the inspector you can change the settings of the script file to what ever recording you wish to do.
## Camera Movement/Animation
If for you scene you wish to animate the camera/make it move around the scene you will need to use the animation window.
first select your camera GameObject, then proceed to the window tab at the top and select animation, this will open the animation window.
the animation will ask you to create an .anim file, this will be the file stores the animation sequence,
after creating the animation file you will be to start animating this.
the first step will be to record the start point of the camera GameObject,
to do this you will first need to add the properties of the GameObject that you wish to animate,
for the purposes of the camera you will need to select the position and rotation of the transform properties.
this will allow you to animate the camera in your scene. Now that you have the properties you can begin recording,
to record the starting point of the camera you will need to press the keyframe button,
this will record the cameras properties and set them as the start point of the animation.
the next step is to move the red vertical bar on the animation window to the next point you will want the camera to be and then press the keyframe
button one again you will then need to change properties of the camera to where you want it to be (i.e. position, rotation etc)
which will automatically record them to the keyframe that you previously selected.
## Creating a In-Game TV
To create a in-game TV you first need the video you wish to broadcast in MP4 format and it will also need to be imported into the assets folder,
after this is done begin the process by first creating a game object that will represent the screen of the TV or you can import a TV asset that you created or that you have taken from another source.
Place this tv asset where you wish it to be in the scene, now that you have your tv you will need to create a new material. this can be done through the project by right clicking and selecting create,
new material. make sure that the material is set to shader: diffuse. now you can apply the video to the material, drag and drop the MP4 file into the texture square of the material and then
apply the material to the game-object that is the tv. when this is done the image will be upsidedown so to fix that rotate the game-object until the orientation of the image is correct.
You have now created an in-game TV.
Here is a video tutorial of the process if needed: [(click here)](https://www.youtube.com/watch?v=-vd9Mdb2r34.)
