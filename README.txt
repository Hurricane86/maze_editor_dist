
A prototype of a maze editor made in three.js

The editor starts with a simple level already built.
You can enlarge the scenario using the UI (grid editing->generation)
setting proper values for a "clipping rectangle" without destructing what you have already edit. 
Be sure to enable the flag "override visibility" (otherwise you don't see anything)
 and then just click on "apply changes". 
Regenerating the grid with enabled the flag "reset cells" throw away your changes so be careful!

you can save and open a level always using the UI.
when a cell is selected (picking it with the left mouse or with ARROWS) 
you can choose the visibility and change/add/remove layers using the UI.
By default when you place a new layer it's set as "bridge". 
For now there are only three type of layers: platform, bridge and stairs.
Of course you can choose the layer height and the rotation (useful just for the stairs).

By default the camera is set as should be but an orbit camera is enabled for editing.
These are the controls:
left mouse button + mouse move                  => camera rotation
right mouse button + mouse move                 => camera panning
middle mouse button + mouse move or mouse wheel => camera zoom in/out

You can reset the camera using the UI and if you want play with the position of the camera by hand.

There is a dummy red cylinder as cursor (the "player") that you can move with W/A/S/D keys.

When "smart editing" is enabled you build the level moving the cursor directly.
Keep SHIFT pressed to go up or CTRL pressed to go down. Stairs, bridge etc are automatically placed!

other useful shortcuts:
up/down/left/right => to move it wherever you want without any constraint (but only on not-clipped cells).
numpad +/-         => to increment/decrement of one the height of the selected cell layer
numpad *           => to rotate the selected cell layer
numpad /           => to change the type of the selected cell layer
0-9                => to change the height of the selected cell layer (final height = base height + 0/9)