
## Decorating Your World

The next step in map building is to decorate your map with convincing details.  We've introduced this topic already with the Properties
of road segments:  we've seen how procedural vegetation can be generated to populate the sides of the road with trees, bushes, flowers, etc; and we've seen how materials can be selected to give the terrain each side of the road a distinctive look (ploughed field, grassland,
desert, etc), as well as to vary the road surface colour and texture.

Now we'll take a closer look at all the cool set-dressing available in the Map Editor.

There are three main object types you'll be using to decorate your map:  Prefabs, Models, and Buildings.

You've already worked with *Prefabs*, in the form of road intersections.  There are quite a few other types of prefab.  In general, any "active" area of the map (a place where you interact with the scenery in some way) is a prefab.  These include gas stations, freight terminals, ferry terminals, sleeping areas, etc.

*Models* are by far the most common object type you'll use when dressing up your bare map.  Models include just about everything:  buildings, trees, parked vehicles, people, bridges, statues, cows, chickens, all kinds of stuff.  Some models are animated;  others are static.

*Buildings* are a curious class which does not, for some reason, only include buildings.  "Buildings" includes items that can be generated along a path, such as extensible fencing and railings, lines of trees for boulevards and wind breaks, etc.

[WIP... to be continued]

(Don't forget about) The Vegetation Sphere is an attribute of a terrain or road segment, activated by a button at the BOTTOM of the Properties popup window.  Despite its name, the Vegetation Sphere is actually a NO-Vegetation-Sphere:  it defines a region in which the procedural vegetation generator will not place objects.  This can be handy if you want to locate a building in a wooded area, for example.  Instead of having to hand-craft a woodland around the building, leaving a clearing for it, you can just fill up your terrain with generated woodland but add a Veg Sphere of appropriate diameter where you want the building to go.

The vegetation generator will simply not place any objects which would fall within the perimeter defined by the sphere's intersection with the terrain.  So you'll see a handy circular or oval patch where you can place your building without trees growing through the walls and roof.  The Veg Sphere only prevents procedural vegetation, not placement of individual tree/shrub models. It will not prevent you from adding some trees by hand, if you do want some growth closer to the building than the clearing perimeter.  Hint:  a few hand-placed trees can camouflage the artificial shape of the clearing.  
