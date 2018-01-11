
This doc is a grab bag of topics, tips, links, etc gleaned by dogged trawling through entire "mapping help" threads on the promods and scs fora.  My plan is to organise it all by topic, provide an index, and publish -- so that n00bs have access to the most helpful material available.

Nico's guide
https://www.scribd.com/document/327182526/ATS-Mapping-Guide
https://drive.google.com/file/d/0B9Ji8vH_F8zneldUUE9yaVB6VkE/view

"Glenn52" SCS Editor Guide (PDF)
http://www.glenn52.com/scs_guides.html

Scribd PDF guide by Dave Crockett Jackson
https://www.ulozto.net/!MybfWbCX/euro-truck-simulator-map-editing-manual-pdf

Basics:  open the map editor and save your work
https://www.youtube.com/watch?v=clLEATRsIR0

The ProMods Advanced Tips series:
1. curves and banks: https://youtu.be/J9leGT5SH8Y
2: better bridges: https://youtu.be/C-eqesW3LlM
3: building interchanges pt 1: https://youtu.be/yWF0a9uUNmo
4: building interchanges pt 2: https://youtu.be/osFlxcwggbk
5: miniconsole and debugging: https://youtu.be/SG33bEwC5GQ
6: cutplanes https://youtu.be/7IFJttG9TRc
do not be put off by the low audio level.  these are worthwhile viewing.

http://forum.scssoft.com/viewtopic.php?f=172&t=190685

ETS STUDIO
http://www.ets2studio.com/p/download.html

Background
https://forum.scssoft.com/viewtopic.php?f=123&t=167214

oldish but still useful
https://www.promods.net/viewtopic.php?f=9&t=1326

Long long ProMods thread
https://promods.net/viewtopic.php?f=36&t=1326&start=10

adding models
https://forum.scssoft.com/viewtopic.php?t=231521

saving sectors
https://forum.scssoft.com/viewtopic.php?t=48851&start=10

import map?
https://forum.scssoft.com/viewtopic.php?f=5&t=192370&start=70

background again
https://forum.scssoft.com/viewtopic.php?t=167214

creating cities
https://forum.scssoft.com/viewtopic.php?f=182&t=208021&start=10

making water reflective
https://forum.scssoft.com/viewtopic.php?f=182&t=207999

How to find a troubled item by uid based on error message:
edit game_log with favourite text editor, find error message, copy UID;  in editor use F to bring up Find, paste UID into UID field, and Find will teleport you to exact location of node.  after that it's up to you to figure it out.

avoid crash on saving sign template
https://forum.scssoft.com/viewtopic.php?t=247057

triggers and sleeping
https://forum.scssoft.com/viewtopic.php?t=130115

a couple of video tutes
https://forum.scssoft.com/viewtopic.php?t=243098

find a prefab by its number
https://forum.scssoft.com/viewtopic.php?t=180589

what is a Traffic Area
https://forum.scssoft.com/viewtopic.php?f=11&t=221010

how to remove transparent no-go barriers
https://forum.scssoft.com/viewtopic.php?f=123&t=26469&start=10

how to add rivers
https://forum.scssoft.com/viewtopic.php?t=131290

how to set AI speed
https://forum.scssoft.com/viewtopic.php?t=146858
https://forum.scssoft.com/viewtopic.php?t=129621

Press F to find?

mysterious growing/shrinking mountains (what is a KDOP?)
https://forum.scssoft.com/viewtopic.php?f=111&t=204446&start=10

KDOP...  aren't you sorry you asked?
https://en.wikipedia.org/wiki/Bounding_volume

background image and map scaling
https://forum.scssoft.com/viewtopic.php?t=194514

make collisions visible for debugging
https://forum.scssoft.com/viewtopic.php?t=61231

customising jobs list (at gameplay time)
https://forum.scssoft.com/viewtopic.php?t=199114

cut and paste often-used objects, store outside cutplane
https://forum.scssoft.com/viewtopic.php?f=41&t=132271&start=40

understanding map scale
https://forum.scssoft.com/viewtopic.php?t=19693

rules of road segment creation
https://promods.net/viewtopic.php?t=18959

how to build a hill
https://promods.net/viewtopic.php?f=36&t=1326&start=80

brush doesn't work on prefabs

You can always attach square and dot even of same color, but never ever two dots of same color
red never goes with red
circle - square always connect regardless of color
circle - circle must be opposite color
Don't know with square - square though can't remember
When connected you drag one and the other will follow
intersection prefab has 2 green squares :-)  solves red/red impasse
red dots carry the item properties

connect unlike roads:
There are prefabs called "joints" - Just search in ( Are you using a ProMods as a base? , if yes, so try write "joint" )
Stuff like Joints will help you to connect rl 1 roads with rl 2 roads without seeing some odd stuff. There are 3 variations of them - with broken lines, single line or double lines.  Just search for "joint" :)

Bezier patches can impact performace if overused in a small area


Nico:
That is not an easy question to answer at all. I will try to cover them all quickly:

For overlays:
Add texture files (mat, tobj, dds) in material/overlay and also add def entries in the def/world/overlay.sii

Add countries: 
Make new country file in def/country/. Add the new file in the def/country.sii.

Add cities:
Same as countries but in def/city/ and def/city.sii.

Add ferries:
Same again but in def/ferry and def/ferry.sii. These also need to be added in the game with the ferry node. Also the prefab needs to have the ferry entrance option enabled to create a route.

Add license plates: 
You need to add lp data in /material/ui/lp/<country.name>/. Here you need texture files (mat, tobj, dds). Also you need a font for the license plates which are in font/license_plate/. Here you need texture files (mat, tobj, dds) and a font file (.font).

add cities tutorial bad link (malware warning) PM author
https://www.promods.net/viewtopic.php?f=9&t=253#p8845

structure of cities and companies files
https://promods.net/viewtopic.php?f=36&t=1326&start=520

add garage:
1. Place the garage prefab, then create a def file for it. Just look into a mod how definitions are done...
2. If you press F5 the satnav will appear. "A" will open a background map to see where you are compared to real Europe and how much space you have in that region to stay on scale.
3. For mapping you don't have to extract anything actually :)
4. ONLY ONE PER TOWN!

Hopefully this covers some of the questions.

add cities:

def-folder structure "mine that is":
city.mymod.sii
city and company folders.

city-folder has a file mytown.mymod.sii
Important line there is :
@include "/def/city/mytown.mymod.sii"
+ the other lines needed.

company-folder has gnt and norrfood folders
each of these has a editor-folder
editor-folder contains 
mytown.mymod.sii 

company_def : .mytown
city: mytown

gnt is "prefab: 283"
while norrfood has "prefab: 289"

Ok, that was overkill.

add cities (2)
https://www.promods.net/viewtopic.php?f=36&t=7581&start=170

Regarding prefabs and roads: I have to sometimes start a new road next to the prefab and then connect both.
Try just to make a simple road between 2 companies as a start, without anyprefabs, but add 2 different companies. And place a garage close to the road.
Might work?
+recheck all folders and sii files

add dealer: How do you add a dealer to a particular city, so that you don't get the error in the log that it doesn't exist in editor/id?
Well, I think you only have to place a dealer in map editor and then add a vehicle_brand line in that city definition file.

To get traffic lights at intersections tick "use semaphores" in the prefab.

the sign editor tutorial
https://www.promods.net/viewtopic.php?f=36&t=12021

how sign images work
https://promods.net/viewtopic.php?f=36&t=1326&start=200

making flags, gimp has dds plugin
https://promods.net/viewtopic.php?f=36&t=1326&start=370

tobj editor
https://forum.scssoft.com/viewtopic.php?f=41&t=53503

license plates
https://promods.net/viewtopic.php?f=36&t=1326&start=250

narrow road non-driveway doesn't work in route map
https://promods.net/viewtopic.php?f=36&t=1326&start=270

how to add a city
https://promods.net/viewtopic.php?f=36&t=1326&start=310

more on city add
https://www.promods.net/viewtopic.php?f=36&t=7581&start=430

SCS Models Editor by Nico
https://trucksim.org/threads/scs-models-editor.507/

i8n of city names
https://promods.net/viewtopic.php?f=36&t=1326&start=400

new garages and city def files
https://promods.net/viewtopic.php?f=36&t=1326&start=410

make bkgnd map
you can probably make your own by screenshotting google maps or mapy.cz and combining them in a photo editor.
Then you make it into a .dds, name it whatever you like (europe-bgn is the default) and point the def at it
-- editor_data.sii

2 different types of roads:  old style with hard coded markings, new style with dropdown menu skinning options
https://www.promods.net/viewtopic.php?f=36&t=7581&start=190

Q: Is there a prefab than connects "HW2b 2m" to "HW2b 5m"
A: You don't need a prefab. The game will widen or narrow the median if the connection between the two road sections is long enough.

road attributes can be saved as Default or as named Presets for easy subsequent re-use

roads don't blend properly where stitched
Are you using FLDs prefabs?
If so, remove the following files:
- /material/road/trans_0.dds
- /material/road/trans_1.dds
- /material/road/trans_2.dds
(2015)

Another question; how can I divide items like roads, fences, trees line like in the video (minute 5.40) ?
https://youtu.be/z6agMir_8fo
You click with the scroll wheel or the middle mouse button.

minicon value 2, 3, 4 : higher detail level:  2 is triangle count detail, 3 is draw call detail, 4 is element counts of each type
g_colbox 1 : turn on red collision boxes so you can see invisible barriers

Custom signs
You have two options. Either you edit ONLY the .dds file and save it under the SAME name, or you save it under another name, edit a TOBJ file and assign it to your new .dds file, then you edit a .mat file that points to your TOBJ file, also you'll have to add it in overlay.sii if you choose the second option. THEN you'll find the sign overlay under the name you've chosen as your .mat file.
Most people were saying that this procedure is tricky, but actually it's not, just give it a shot.
cristakey, 
Have you
a) Made a .mat file? and pointed it to the correct .tobj?
b) used TobjEdit to point the .tobj to the correct .dds?
c) made the dds using DXTbmp?
Sign images need four files to work:
- A DDS image file with your sign image
- A TOBJ file referencing to the DDS image
- A MAT file refering to the TOBJ
- A SII DEF-file refering to this mat file and the co-ordinates of the image elements. These definition files are found in /def/sign/atlas

more on signs:
https://www.promods.net/viewtopic.php?f=36&t=7581&start=150

make your own sign template
https://www.promods.net/viewtopic.php?f=36&t=7581&start=370

brush does not work on prefabs

custom billboards:
You need to change materials/looks on the model (billboard)
I can give you the specifics later (model name/path etc)
Images must in power of two and rectangular eg 512 x 1024

to give a mod high priority name it zzzMod, not aaaMod.

standalone map:
When creating a new profile, after adding your mod from the mod manager, (where you can choose your favorite truck or change your profile avatar face) there will be a "Module" dropdown where you should be able to select your alternative map.
also
https://www.promods.net/viewtopic.php?p=26628

underlay map
You can copy already existing files and just change file name. Try it.
.mat files - open with Notepad or Notepad++
.tobj files - open with ETS2Studio. This program has built-in TOBJ editor.

cutplanes explained
https://promods.net/viewtopic.php?f=36&t=1326&start=880

hookups and overlays
https://www.promods.net/viewtopic.php?f=36&t=7581&start=90

cut plane rules
simple object:  node must be behind cut plane
road segment:  both nodes must be behind
bezier patch:  master mode mst be behind
prefab:  all nodes must be behind

ferry connection issues
https://www.promods.net/viewtopic.php?f=36&t=7581&start=320

more on ferries
https://www.promods.net/viewtopic.php?f=36&t=7581&start=410

license plates
I think you don't have to set every road to Israel. I've never done that but I think you only have to change one prefab/road and then all roads connected to it will generate Israel license plates.
To get lower speed limit in city, I think you have to place Traffic area

what is an atlas
https://www.promods.net/viewtopic.php?f=36&t=7581&start=350

test . hotkey:
if you press this while click on a "building" node it will select all nodes in the structure
if you have a node selected and then press ., the next node should also be selected (extend selection)

terrain patching
I always us a combination: I use bezier patches to fill the large gaps (sometimes you need multiple) and I use road generated terrain right next to roads and prefabs to fill up the gaps between the road and the bezier patch (I usually set the terrain profile to down or d down 1 with a coeff somewhere between 0.2 and 2.0). Furthermore, I use terrain items for the bridge ends. You can find proper examples of this interchange landscaping near Kolding (DK) or Harwich (UK)
You need to set the "Noise" to 0% for it to be straight. For prefabs, the noise will only become 0% once every road connected to the prefab also has a 0% noise.

MOST COMMON PROBLEMS:
* map stopped working on update (Delete defaults.ini file from Documents/Euro Truck Simulator 2/editor folder )
* game crashes on start editor (empty your mods and plugins)
* can't see background image (hit A a few times)
* can't load background image (see tutorial)
* can't get road end nodes to join (use alt)
* can't get edited map loaded back in (workflow)
* exceeded stamp count (https://forum.scssoft.com/viewtopic.php?t=6005)
* autosave annoying/slow (https://forum.scssoft.com/viewtopic.php?t=23387  edit param)
* need big screen for map editor (oh well!)
* running into road boundaries (https://promods.net/viewtopic.php?f=36&t=1326&start=240)
* set truck start position (https://forum.scssoft.com/viewtopic.php?t=15970)

N00b Qs
https://www.promods.net/viewtopic.php?f=36&t=7581&start=190

Sometimes F6 will not work correctly with building items, because the node has not touched the ground correctly or the surface is not even.  The best solution is to delete the building item and build it again
1. Create a new fence.
2. Go to "item properties"
3. Click "reset offsets"
4. Click "set as default"
5. Now you can draw fences again without them being cracked like this.

You have to do something, to make far things look nice. Terrain can't suddenly end. Finish it with hill/forest. Something, that player will see instead of just terrain end. I think it was visible in latest video uploaded by your friend. There was a river that was just ending. Make it longer or make it turn right and hide behind a small hill, so it's not that obvious where it ends ;)
I know, at first (like August 2016) I took a look at West Berlin. 400 plain with %0 noise and in continue of it; plain (or 0.1 d down up) terrain, different field areas with brush, some fences, farm objects and at the end; tree line. Some towns in far away, country road bridges over highway and countless mini details.

The only worry was horizon and now it is cristal clear. 

UNANSWERED Qs

how to load standalone map
can Blender edit prefabs with stop lights

