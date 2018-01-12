## Editing in the Fast Lane

The conventional wisdom, as discussed in Testing Your Mod, is that you must exit the game after saving your map, repackage/reload the mod,
and restart the game.

However, if you'd like to skip these steps, there is a way.  Recall that there are two essential folders in the SCS game world.  One we'll 
call **INSTALL** -- that's the folder where the ETS2 or ATS binaries and base files were installed.  It looks like this:

![INSTALL folder](img/INSTALL_folder.PNG)

The other we'll call **USER**.  That's the one where you keep your profiles, your mod folder, and other stuff specific to your personal install of the game.  It looks like this:

![USER folder](img/USER_folder.PNG)

If you want to avoid the quit/repack/reload/start cycle, here's how.

In your **USER/mod** folder, make a folder called *YourMapName* (this must match the name of the mbd file that you're saving).

Within this **USER/mod/*YourMapName*** folder, make a LINK to **INSTALL/base/map**

![The link called 'map'](img/LINK_map.PNG)

If you do this right, then when you go to **USER/mod/*YourMapName*/map**, you will find yourself in **INSTALL/base/map**

You might, of course, be editing more than one map at a time.  You might have saved more than one *YourMapName*.mbd file and *YourMapName* folder in **INSTALL/base/map**.  That doesn't matter.  If you are working on more than one map mod, just put another folder in **USER/mod** with the second map name, and in that folder put the same LINK to **INSTALL/base/map**.

Making these links in Windows is not as straightforward as I'm used to (coming from 'nix territory).  You might be able to use mklink, or the extension HardLinkShellExt_64, or the Windows Power Shell "new item" command.  Here's a thread that covers the topic.  Good luck!

https://superuser.com/questions/1020821/how-to-create-a-symbolic-link-on-windows-10




