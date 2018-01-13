## Frequently Asked Questions

### BASIC
* *can't get into editor* -- set game params and mode properly, see [Before You Begin](tutorialguide.md) and [Setup](fundamentals/1_setup.md)
* *game crashes on start editor* -- get rid of mods and plugins, see [Setup](fundamentals/1_setup.md)
* *can't see background image* -- hit A a few times
* *can't get edited map loaded back in*  -- see [Testing Your Map](fundamentals/4_testing.md)
* *need big screen for properties window* -- (sorry, you do need a big screen for this)
* *can't get road end nodes to join* -- use alt-click to disregard Y position
* *can't get joined nodes apart again* -- use shift-click to unglue nodes
* *autosave annoying/slow* -- you can slow this down or turn it off with a tiny mod.  see [Tips & Tricks](fundamentals/6_tipsNtrix.md)
* *how to set truck start position* -- use S key, see [Tips & Tricks](fundamentals/6_tipsNtrix.md)
* *ouch, my scenery has ugly gaps* -- see [Maintain the Illusion](fundamentals/5_illusion.md)

### INTERMEDIATE
* *map stopped working on game update* -- delete defaults.ini file from **USER/editor** folder and try again
* *can't load custom background image* -- see [Custom Map Background Tutorial](./newmodule/1_imagery.md)
* *"index outside array boundaries" (exceeded stamp count)* -- 
```
Originally warning about exceeding stamp_count is set to 40, and a warning about exceeding road_length on the 330m.
To get rid of these warnings simply increase the value of these lines in the file /def/editor_data.sii and add this file in your .scs
```
* *"failed to register water level for uid xxxxx" error* -- two water planes with different heights, close together.  generally harmless.
* *ouch, running into invisible boundaries* (https://promods.net/viewtopic.php?f=36&t=1326&start=240)
* how to package my mod for sharing

### ADVANCED
* how to create a new city
* how to create a new business
* how to create custom signage
* controlling AI traffic flow
* how to modify game models
* how to introduce new models
