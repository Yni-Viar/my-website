<!-- title: September 2025 update -->
# Internal Eternal troubles

Back at Devlog 3 times, I itegrated Humanizer addon, which is a MakeHuman port.
I initially thought that it is a re-implementation. How much I mistook...

Humanizer IS a MakeHuman port and IS licensed under AGPL, which is not good for game,
so, unfortunately, makes Devlog 3 progress null and void.

# Human Generator

Luckily, I found another MIT-licensed abandoned human generator, and it
uses native Godot node system (Humanizer tried to replicate MakeHuman style).

Because it is necessary for Internal Eternal, I already forked from original repo, 
and will try my best to improve it (as Internal Eternal, it is my 2nd priority right now).
If you are interested, here is [the repository, feel free to contribute!](https://github.com/Yni-Viar/gd-character-creation)

Let's talk about first priority - SCP: Containment Procedures!

# SCP: Containment Procedures

I have done large work during this month.

## Settings menu

![Settings](./content/images/scp_cont_pr_settings_progress.png)

I'm really proud of my first ever keybinding system (none of my games used keybinding,
even Internal Eternal - I will later port this feature)

SCP: Containment Procedures previously lacked Settings system. Until upcoming 5.0 update (Expansion part 2)

## Camera rework.

### Camera movement hotkeys

Previously, camera system and movement was... not good.
For changing view you need to hold right mouse button. And so many times.

I recently implemented hotkeys for quick movement.

### Third-person mode

Previously, the game did not have a truly immersive mode. It looked like a RTS.
Finally, I decided to implement a 3rd person camera, along the usual look.

## Other changes

In the beginning of 5.0 development, I added dormant mode to SCP-023, thus allowing it to spawn
in Safe mode!

Also, I added more probs, now for Class-Ds'

And finally, an important message:

# Godot 4.5 and old Windows.

Godot keeps saying, that they don't support Windows 7, 8.0 and 8.1.

It is true for the first two ones. But for the latter...

It **is working natively on Windows 8.1 laptop!** I created a test project with label and Stencil-buffered mesh (which is a new Godot 4.5 feature). Both the Godot editor and exported project were working! Also, I checked the code, and no Windows 8.1 support was broken.

That means, that SCP: Containment Procedures 5.0 (and Internal Eternal) will be updated to Godot 4.5, and Windows 7-8.0 support will be removed 😢... Except Windows 8.1!