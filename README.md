# Demo-Game
COSC 4324 Computer Game Development I - Final Project 12/03/2021

For this assignment you will modify the GX demo program.

Create a program using the GX Toolkit that has the following features:
1) A textured ground plane. 
2) A textured sky dome. 
3) At least 20 moving targets.  These can be any 3D model including a camera-facing billboard.  The targets can move in any manner including a random direction.  Use frustum culling before drawing each target.
4) Ability to move the camera with the WSAD keys and mouse rotation (as in previous recent homework assignments).
5) Pressing the LEFT mouse button will shoot a ray from the camera location into the screen along the view vector - the direction vector (heading) that defines the direction the camera is looking.  Your ray should have unlimited range and you should test against all targets that are currently rendered (do not test against targets that were culled during view frustum culling – they are not on the screen).  In addition, play a sound effect each time the LEFT mouse button is pressed.
6) If the ray collides with any target’s bounding sphere (or box, your choice):
    - Remove the target from rendering (don’t draw it anymore)
    - Play a sound effect (once for each target)
7) Play a background sound effect (such as music) continuously in the background.
8) For each target removed from the game draw an alpha-blended 2D graphic (icon) at the top of the screen.  Draw up to 10 icons, 1 for each target removed. 
9) You must ‘shoot’ targets 3 times before the target is eliminated.  Keep track of the number of hits each target has taken.
10) Each time a target is hit display a text message above the target using a camera-facing billboard drawn near the target’s current location.  The text message should remain on the screen for one second. 
11) While the ‘hit’ message is on screen is should move up the y axis.  Over the course of one second it should move up a distance of approximately twice the height of the billboard.  So, for example, if the billboard is 1 foot in height then over the course of the 1 second it appears on screen it will move up the y axis approximately 2 feet.
