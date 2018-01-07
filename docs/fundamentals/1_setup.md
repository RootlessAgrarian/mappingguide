# Tutorial 1 --- Basic Editor Setup

This tutorial will help you set up your game correctly for using the map editor.  
* *Please note that the SCS Map Editor works only in the Windows version of the game(s).*  While Linux and Mac users can do some modding of vehicles etc. by way of def files and portable tools, actual map editing is possible only with Windows.  I am an OSX (Steam) ETS2 user, and having tried several approaches I finally installed Parallels on my Hackintosh, which works well enough to play 3d games (and run the map editor --RA).

## 1. Enabling the Editor

Navigate to your user folder -- ```C:\Users\<username>\Documents\Euro Truck Simulator 2``` by default -- and open ```config.cfg``` in a text editor.

Find the line ```g_developer "0"``` and change the value to ```"2"```. Then find ```g_console "0"``` and change the value to ```"1"```.

You might also wish to enable the miniconsole by setting g_minicon to 1, as above with g_console and g_developer.  This will enable a small (4 or 5 line) console overlay at the top of your screen, so you can see any error messages in real time.  The editor will work with or without this option, so it's up to you;  but many modders find the miniconsole useful.

Next time you launch the game, you'll be able to load the editor using the console command ```edit```. 

Before you do this however, you should make one more change to enable saving of maps.

## 2. Enabling Saves

The editor saves maps to a directory in the _executable_ folder, however this folder does not exist by default, and the editor produces an error rather than saving if the folder does not exist.  (Many new users are immediately confused by this!)  You need to create it.

Go to your executable folder -- ```C:\Program Files (x86)\Steam\steamapps\common\Euro Truck Simulator 2``` by default -- and create a folder called ```base```, then another folder inside this one called ```map```.

That's it! you're almost ready to start mapping.  Just a couple more prep steps... first, make sure you don't confuse the editor with 3rd party mods.

## 3.  Get rid of all mods other than those absolutely necessary for your mapping project

The map editor is not kindly disposed towards a stack of contrib mods.  You may have incompatible mods kicking around, which you usually don't notice because you're careful never to load them into the same profile.  But the editor loads whatever it finds in your mod folder, in alphabetical order -- it doesn't care about profiles.  Best practise is to remove all mod files from your mod dir, other than things (like contrib models and buildings) that you really need for your map.  Now that you've cleaned up your mod folder, there's just one more setup detail...

## 4.  Configure your game to run in Windowed mode

The editor runs best not in full screen mode, but in Windowed mode.  Depending on your version of the game, you may set this option in Steam launch preferences or in the game options.

### A Note on loading saved maps

The process for loading maps is somewhat laborious, as the editor can only use game files that are currently loaded by the game.

You should complete the next tutorial in a single sitting if possible, but if you need to load your saved project right now for any reason, skip to tutorial 3 --  the process of loading your maps into the game is explained there.

[<- Back to Index](../index.md) --- [ Tutorial 2 - Creating a basic map ->](2_firstmap.md)
