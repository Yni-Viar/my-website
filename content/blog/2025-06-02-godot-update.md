<!-- title: Godot and old devices -->
Today I won't speak about my project news. Today I will speak about Godot update.

# Godot 4.5 and old devices.
In upcoming Godot 4.5 update there are not so much changes (the most notable changes
are AccessKit integration (as accessibility feature) and Specular Occlusion for LightmapGI), as were in Godot 4.4.

But the system requirements are raised:

x86-64 (64-bit PC) [CPU requirements](https://github.com/godotengine/godot/pull/59595) are raised to SSE 4.2 (which is not critical).

Android OS minimal API [raised](https://github.com/godotengine/godot/pull/106148) to API 24 (Android 7 Nougat) (which is worse, because even Unity minimal requirements are a bit lower - Android 6 Marshmallow).

Also, Windows 7, 8 and 8.1 support is about to get [dropped](https://github.com/godotengine/godot/pull/106959) from Godot (Windows 7 support is broken by AccessKit integration, and Windows 8/8.1 support was dropped intentionally)

# Possible solutions.
The first one is Supermium + Web server + Godot Web Editor/Game.
- Pros:
    - this is the easiest solution, since Supermium work even on Windows XP.
- Cons:
    - Godot Web editor [is very limited](https://docs.godotengine.org/en/stable/tutorials/editor/using_the_web_editor.html). You can only create or edit the project (but not export and even delete files)

The second solution is to move on to Linux (only for old Windows 7/8/8.1 PCs)

And the third one I will tell you later.

# Godot ports
I saw a project, where Godot 2.1 was ported to Windows XP (I did not test it currently, because Godot 2.x is very old compared to Godot 4.x)

This idea came to me - after Godot 4.5 releases, I *may* create a fork of Godot Engine to support Godot 4.4 as unofficial LTS for old devices, <s>because I like the old Frutiger-Aero designs of Windows 7, having an ability to switch easily to Basic or Classic themes in there, and as for Windows 8.1, it does not spy on you... And I have a working Android 6 device!</s>.

# Why not Godot 3.x
Godot 3.x lacks some good Godot 4 features (as for example typed arrays or simple multiplayer solution)