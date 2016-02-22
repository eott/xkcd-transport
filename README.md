# Xkcraftia Transportation Map

This project is a topological map of the various transportation modes on the main map of
the xkcd Minecraft server (xkcraftia).

## Notes on the data
* There are probably typos and abbreviations in the node names of the edge data. When using
the data by hand, this is not a problem, but the data needs cleanup before being able to be
handled by an automatic import.
* Many stations are not really a single point, but spread out. So while two edges may meet in
a node in the map, their connection in the Minecraft world is not immediately obvious.
* This data only covers the Overworld and only the largest connected subgraph of all transportation
nodes. The nodes are also not a complete list of points of interest.
* Where no names were obvious, I chose them arbitrarily.
* Not all walkways are listed. I tried to only list the major ones or those that are the only connection
to certain nodes. Still, this is fairly arbitrary.
* The xyz-coordinates of nodes are very inaccurate. I only gathered and used them so I could pinpoint
the nodes roughly on a geographic map.

## Notes on the map and how to use the data
* I mapped the raw data in a graphml file with the program yEd. I used custom nodes and edges that are similar
of those used in metro maps. Unfortunately I can't be bothered to make the palette available for all, but it's
not that much work anyway.
* The rendering of yEd leaves some things to be desired, such as nodes and text being rendered behind edges.
* There is **a lot** of potential to make the map prettier, such as choosing pathed edges instead of straight ones
and choosing smarter text positioning.
* I should have made the legend as vector graphics, but raster graphics were easier at the time.