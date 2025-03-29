# HelloThreePointsSetup
Learn about how to use the project Three Points that allows to measure, load and calibrate room in Unity3D with Quest3




## Load a level ?

## From Three exact mesh points

Setup:
- Scan a room with three point building tool (or else)
- Put a Three Points tag at the exact mesh point positions (using snapping 'v')
- And the script 'transform3'
- Add the script 'movable' with the transform3 and the scene to move with it.

Loading:
- Every time you submit a triangle with this exact measure, if in the register, the level will be moved (or loaded) 

### From mark on the ground

Setup:
- You just put some sticker on the ground like 5x1 meter rect triangle
Loading:
- You Add and submit the three point on the ground.

### From Table

Setup:
- Put a table in your scene
- It must have a height+ (Depth+ Width)
  - The Depth and Width is mandatory.  

Loading
- You add and submit three points right, left, front left to load the table.
   


## Load room using 3D Print tag

Not coded Yet.
![image](https://github.com/user-attachments/assets/2fab89e9-cb40-4b63-8ca4-c9301ca84a47)

You can load a room using triangulations.
But you need to remeber what where the three anchor point.

And other way to do it.

Setup calibration:
- You anchor with double side sticker 3 printed anchors.
- You fit the controller in the print and don't move it for the three anchors.
- A triangle is generated that will allows to reload the level.
- Now take you level and by "hand" make it fit the best you can in the room
  - For example by using the three points loader.
- Save the triangulation of the anchor with the level.

Relaod calibration:
- Put the controller and wait at the three printed anchor.
- The level should reload automaticaly


 
