Imphenzia PixPal Palette Version 1.1

License: CC0 - Creative Commons 0 - Public Domain.

You can do what you want with it =)

I have included:
* The textures themselves.
* The .blend-file with material set up with the textures and sample assets.
* A Unreal Engine 5.3 project with material and sample assets.
* A Unity 2023.1 URP project with material and sample assets (no reflections)
* A Godot 4.1 project with material and sample assets (no reflections)

The materials in the Blend-file, the Unity project, the Unreal Engine
projectm and the Godot project have the correct texture settings, material and
shaders for texture quality, emission, to work.

The Blend-file and the Unreal Engine projects have environment and object
reflection enabled.

Note that Unity URP and Godot do not support reflection out of the box
so it won't reflect the the surroundings like in Blender and Unreal Engine.


*** VERY IMPORTANT INFORMATION ************************************************

If you create your own materials, take the following into consideration:

1. USE NEAREST NEIGHBOR FILTERING

If you use the textures in a game engine, make sure you set the filtering to
Nearest Neighbor or Closest (it should NOT be bilinear or bicubic - it smears
the textures since the colors are only one pixel in width.

2. DO NOT USE COMPRESSION

If you use compression on the textures in a game engine, the colors will be
incorrect. Disable any form of compression on the texture - it needs to be
pixel perfect.

3. DO NOT USE MIPMAPS

The pixel perfect textures are already as small as they can be so it is
advised to disable mipmapping, especially in Unreal Engine where Nanite
can create artifacts around edges of low poly objects.


*** VERSION HISTORY ***********************************************************

1.0 Initial Release

1.1 Added Godot 4.1 project (thanks Flynsarmy!)
    Updated Unreal Engine project to Unreal Engine 5.3
	Added emission strength parameter in game engine projects to control bloom.
	Changed Unreal Engine texture disable mipmap which caused Nanite artifacts.


THANK YOU!

Please subscribe to my YouTube channel, https://www.youtube.com/imphenzia

And enjoy the rewards as a patron on https://www.patreon.com/imphenzia