View the Guide: http://scsmoddingguide.github.io/mappingguide/

# The ETS2/ATS Mapping Guide
Tutorials and documentation for the SCS software map editor.

The SCS map editor is an inbuilt feature of the ATS and ETS2 game engines (Windows version only).  It is a highly specialised 3d modelling tool oriented specifically to the construction of roads & terrain, and placement of all the set dressing, for an open-world driving sim. "Set dressing" in this case means vegetation, guard rails, traffic signs and lights, trains, street lighting, fuel stations, pedestrians, bridges, etc. -- all the stuff that makes the virtual world convincing and attractive.  The Map Editor is *not* a generic 3d modelling tool such as Blender.

Blender can be used to model objects (vehicles, props) for ETS2 and ATS, using appropriate plugins from SCS.  If you want to build your own truck, castle, or pedestrian, you will need to study SCS Blender Tools and read other guides.  The Map Editor is a higher-level tool, which allows you to build the 3d open world and place pre-existing models and other objects within it.  Using the Map Editor you can build your own standalone map, or create a mod that extends a standard map.  You can lay out cities, towns, business locations, fuel stations, border crossings, toll gates, highways, freeways, rural roads and more.

*The fundamental unit of the SCS world map editor is a segment of roadway.*  These segments are strung together to make a road map, with intersections, cloverleafs, overpasses etc. as desired.  The world is designed to be viewed from the roadways, with higher resolution objects near the road and lower resolution objects in the distance.  On each side of your roadway you create scenery, placing suitable objects (trees, rocks, buildings etc) to create the desired effect.  More advanced options allow you to create topography (hills, banks, mountainsides, rivers, ponds etc).  Tricky connecting objects like intersections and cloverleafs are provided (called "prefabs") to make your life easier.

The fundamental coordinate system of the SCS world map editor is an XYZ system with origin at (??? where is 0,0 anyway).  Z indicates height above sea level.  The game world consists of "sectors" defined by X and Y, containing terrain with varying Z values.

Your completed map project can be saved as a mod and loaded into the game.

There is very little information available to help new users learn the map editor or understand the game internals.  Documentation is patchy, often available in only one language or out of date.

That is why this project was started by Jack Kelly -- many thanks to Jack for his excellent "Intro to Mapping"!  Jack's no longer maintaining it, so I (being an SCS mapping n00b in need of doco) am volunteering to maintain and (I hope) extend it.

## License 
Thes files and documents contained within this guide are licensed under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license
