### Tips and Tricks for Easier Editing

#### I need more nodes here!  (Middle-Mouse-Click to add nodes to an object chain)

Say you have a road segment which you need to bend more gracefully, or you need to expand it a bit with a detour.  But you only have one segment and you can't really make it right by stretching its neighbours.  You could unsnap it from its neighbours, extend new segments and snap it all back together;  or you could generate new nodes inside the existing segment with Middle-Mouse-Click.  When you Middle-Click on a road segment's red handle, you introduce a new node at the mid point.

This is also handy for making nicely proportioned segments for e.g. a prefab to slot into.  You can subdivide a segment into 4 even parts quickly, then delete the two inner ones, leaving two nicely proportioned ramps for a bridge prefab to fit between.  You can do this same trick with "Building" (Series) objects like fences and hedges, introducing new nodes to make your long object more bendy and adjustable.   You can also remove existing nodes with Control-Alt-Middle-Click, but this doesn't always work.  If it doesn't work in any given situation, just delete one of the segments and drag the two severed ends back together.

#### I got an error message about UID (some long number)... how do I find it?  (use F with copy/paste of UID)

If you've seen one of these error messages like "Building item too short", with a long intimidating UID number, you might have tried the obvious:  bring up the dev con and try to copy and paste the UID number out of it -- but no, that doesn't work.  Your cursor won't highlight text from the dev con.  What to do?  It would be very tedious to type in the long number or look the instance up via the Content Browser.

So you use your favourite text editor to edit the game_log.txt file, find the error message, copy the UID, return to the map editor, hit F (this pops up the Find dialogue box) and paste that UID into the UID field (near the bottom of the popup).  Hit Find and you should be teleported instantly to the location of that troubled node.

#### I'm doing a whole section of highway that's pretty consistent... (use Default option)

If you have a road segment look-n-feel that you're going to use for an extended distance, set it as the Default.  Then every time you use E to create more road, it will have the same properties.

#### Cut and paste objects to save time

If you're placing rocks and other stuff that repeats in your map, you don't need to hit E repeatedly;  you can select an object, then hit ctrl-C to copy it.  When you paste, it doesn't appear instantly as your cursor, as it would in E mode.  Instead you get a crosshair cursor immediately after the Copy.  When you click somewhere with this crosshair cursor, the object is pasted there.

#### Merging objects

As you've noticed, most game objects don't have collision property -- trees can grow right through buildings, buildings can pass through one another, rocks are insubstantial.  This means you can build large rocky outcrops from repeats of smaller rock units, because they merge together pretty convincingly.  Give it a try -- by varying rotation and altitude you can avoid obvious repetition and make quite long rocky scarps, shelves, cliffs etc.

