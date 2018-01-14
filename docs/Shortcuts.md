# Keyboard short cuts and mouse actions

As you've seen by now, there is a lot of repetitive selection of tools and of menu items in the map editing process.  Why not make life easier and use some of the handy built-in shortcuts?  Here's a list of things you can do with keyboard and mouse.

To the right of the editor menu are lists you can select from, but it is easier to use *shortcut keys*, a list of which 
follows (Standard Qwerty, in parens Azerty Keyboard)

Key | Result
------------ | -------------
A (Q) | toggle background map on or off. If you don’t have any, you will see some red text.
B | Use the brush tool (use sparingly if at all) (see bottom of page for details)
C | Camera view -- toggles between overhead (editor) view to on the “fly” (roadside view) very useful tool to enable you to see how your roads will look at runtime and to aid with precise item placement
D | Delete item by selecting the red node. (You can also select item(s) and use the Delete key on your keyboard).
E | New item
F | Find
G | Add sign tool
H | Height tool
I | Import item
CTRL-I | Isolate selection
CTRL-ALT-I | Hide selection
CTRL-SHIFT-I | Exit isolation
M (,) | Move item
N | Node properties
P | Item properties
Q | Put the background map
R | Rotate item on X, Y or Z (select which axis on the toolbar)
S | Place Start Position (the start-car) (**NOTE**: no longer bound as of this writing)
. (dot) |  hold down while clicking to select *all* nodes of a Building (Series) object;  click, then hit dot (.) to *extend* selection to include more and more nodes (expanding outward from original selection)

Number keys (not keypad;  numbers above QWERTY row):

Key | Result
------------ | -------------
1 | Road
2 | Prefab
3 | Building
4 | Model
5 | Company
6 | Services point (allows you to add custom services and refueling points)
7 | Cut plane (creates a zone that the engine doesn’t need to load at startup but will load when you approach the zone (not really used))
8 | Mover (such as hot air balloon, wind turbine, windmill and so on)
9 | City (This is the option used to add city entities to your map)


Action/Key | Result
------------ | -------------
Right Click/Drag | move the map
Left Click/Drag | select / extend selection / move a selected object
Middle Click | create new node on existing road segment
CTRL-ALT-Middle-Click | delete node from welded series of road segments (may not always work)
ALT Click/Drag | force connection of nodes
SHIFT Click/Drag | disconnect connected nodes
Mouse Hover over node | remembers node height and uses it for next object placement?
Page Up | fast - zoom.
Page Down | fast + zoom.
Scroll up (on the mouse wheel) | slow + zoom.
Scroll down (on the mouse wheel) | slow - zoom.
F5 | toggle mini-map.
KP -, KP + | Rotate the start car
F6 | drop object(s) to ground
ALT F6 | align object(s) to ground vertically 
SPACE | switch to editor mode (visible handles) in flycam view
KP - twice | spawn cars on lines
KP * | after spawning car, this will change the vehicle type

In FREE CAM mode only:

Key|Result
------------ | -------------
UP   | lift object(s) 
DOWN | lower object(s) 
END  | rotate object(s) around X axis (SHIFT-END  for other way round)
DEL  | rotate object(s) around Y axis (SHIFT-DEL  for other way round)
INS  | rotate object(s) around Z axis (SHIFT-INS  for other way round)

In AERIAL VIEW (overhead cam) only, and only when *more than one* object selected:

Key | Result
------------ | -------------
CTRL-R  | rotate several selected objects around shared Y axis clockwise 1 degree
SHIFT-CTRL-R  | rotate several selected objects around shared Y axis counter-clockwise 1 degree
ALT-R  | random model rotation dialog

**NOTE:** if you are using a non-Windows keyboard you may not have an INS key.  The standard Apple keyboard, for example, does not have this key.  You can remap keyboard keys under Windows by using any one of a number of keymap applications.  On the Extended Apple Keyboard (with integral numpad) the F16-19 keys seem to map well.

**Special Prefab Select**

To select ONLY the main node of a prefab:
   * With item (p) or node properties (n) mode active, perform direct click on node while pressing right ALT key

**Brush mode:**

* To use brush: enter brush mode (B), click on white quad
* Brush pick: enter brush mode (B), SHIFT-click on brushed (red) quad


Hat tips to Kentora and others!
https://forum.scssoft.com/viewtopic.php?t=129971

[<- Tutorial 5 - Immersive Illusion](5_illusion.md) --- [Main Index ->](index.md)

