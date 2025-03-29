
# HelloThreePointsSetup  
Learn how to use the *Three Points* project, which enables measuring, loading, and calibrating rooms in Unity3D using the Quest 3.  

## How to Load a Level  

### Using Three Exact Mesh Points  

#### Setup:  
1. Scan the room using the *Three Points* building tool (or another method).  
2. Place a *Three Points* tag at the exact mesh positions using vertex snapping ('V').  
3. Attach the `transform3` script to these points.  
4. Add the `movable` script, linking it with `transform3` and the scene that will move accordingly.  

#### Loading:  
- Whenever a triangle with these exact measurements is detected in the register, the corresponding level will be loaded or repositioned.  

### Using Ground Markers  

#### Setup:  
- Place stickers on the ground forming a rectangle-triangle (e.g., 5m x 1m).  

#### Loading:  
- Add and submit the three marked points on the ground.  

### Using a Table  

#### Setup:  
- Place a table in the scene.  
- Ensure it has defined **height, depth, and width** (depth and width are mandatory).  

#### Loading:  
- Add and submit three points (right, left, and front-left) to load the table into the scene.  

## Loading a Room Using 3D Printed Anchors  

*(Feature not yet implemented)*  

You can load a room using triangulation, but you need to remember the three anchor points.  

### Calibration Setup:  
1. Attach three **3D-printed anchors** to the room using double-sided stickers.  
2. Place the controller into each anchor without moving it.  
3. A triangulation is generated, enabling level reloading.  
4. Manually adjust the level to fit the real room as accurately as possible (e.g., using the *Three Points* loader).  
5. Save the triangulation data along with the level.  

### Reloading Calibration:  
- Position the controller at the three printed anchors and wait.  
- The level should automatically reload.  
