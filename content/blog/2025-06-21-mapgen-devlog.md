<!-- title: Evolution of my SCP-like procedural map generator -->
# The beginning
Back in 2023, I ported Juan's and Virtual's procedural map generator on Godot.
While Juan's was good (except the Containment Breach CC-BY-SA 3.0 license, which breaks compatibility with all third-party code,
because of license incompatibility - that's the reason why I hid SCP: Site Online from public),
Virtual's had drawbacks - that map generator just couldn't always connect all rooms.

I tried to port another procedural map generators (they were mapgen v.1, and mapgen v.2 - they were eventually removed (especially later, which was a copy of another map generator, which had no license))

But these first were not good enough.

# MapGen v.3

In 2023, I created a simple procedural map generator by a tutorial in Godot.

It was easy, but had drawbacks - there were too few hallways (straight hallways with 2 exits).

Because of this problems, I paused developing this map generator, and went to Juan's map generator (I nowadays regret of this choice because of incompatible license).

# MapGen v.5

After I knew CC-BY-SA issues, I dropped Juan's generator port, and began improving my own mapgen.
I moved to GDScript for better mod support, changed algorithm to AStar and added zone support - currently supporting only one direction (like SCP-CB generator).

In 5.1 update I added support for random doors (like *SCP: Secret Laboratory 14.0*) - but that time they were completely random.

And why I skipped v.4 - just because "it combined the power of Juan's mapgen and my old v.3 map generator"

# MapGen v.6
The most key features of 6.0-6.1 features were large rooms - I implemented checks for large rooms (in 6.0 only for endrooms).

In 6.2 changed the map heuristic.

# MapGen v.7
In version 7 of map generator I implemented increasing zones in both direction. Also implemented "Better map generation" - it should reduce "low amount of endrooms" problem.

In v.7.1 I added documentation and in 7.2 I added 2D version.

7.3 was mostly a bugfix (but received a minor - not a patch - version because of the core algorithm change)

# MapGen v.8
I reworked the map generator structure - to a backend and frontends for 2D and 3D, added *SCP: Secret Lab-like* checkpoints and hallway with specific door set (like 14.0 T-section armory) in v.8.0.

The map generator became feature-complete.

In v.8.1 fully implemented chances for single rooms.
And...

# ...Map generator became cross-platform!
I began to port to Unreal Engine - the only platform, that was missing a permissive open-source map generator. (Unity has a good third-party map generator)

The first step to it was native C++ generator. I finished porting at 2025-05-25.

The next step was Unreal Engine 5 - it was very hard, because I was newb to Unreal Engine, and didn't know about UE and C++ specific behavior, that lead me to non-working code - because UE5 documentation was very poor.

But I made it eventually (at the day of writing, Unreal Engine version is still W.I.P. - not all features are ported)!

# The final results.
![Map Generator in Godot](./content/images/mapgen_godot4.png)

![Map Generator in Unreal](./content/images/mapgen_ue5.png)

![Map Generator in C++](./content/images/mapgen_cpp.png)