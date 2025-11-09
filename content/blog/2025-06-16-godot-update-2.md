<!-- title: Godot and old devices part 2 -->
# Showcase

Windows 7/8/8.1 were dropped in Godot 4.5, but what's next.
In previous "Godot and old devices" article, I told about Linux solution, Web and Godot fork.
Today I will speak about later two options.

# Godot 4.5 for Web.

I have recently [workarounded the undeletable files bug](https://github.com/Yni-Viar/godot-web-editor-delete-workaround), by moving the unwanted file outside of the project
(inspired by [this pull request](https://github.com/godotengine/godot/pull/99769))
(it is not actually a solution - only a workaround, so I hope, that Godot devs will try to fix this problem or merge this pull request)

Later I came to the idea - why not create an "installer" for Godot Web for old PCs, that won't migrate to other OS/Windows 10-11.

I decided to use a batch file (and not C# program) - an easy way to create an installer and runner.

[The results are here (currently it is useless, because Godot 4.5 has not released yet...)](https://github.com/Yni-Viar/godot-web-launcher) - 
so you can use Godot 4.5 and later web versions in Windows 7 / 8 / 8.1. It also includes mentioned workaround as a demo file - I recommend to start projects based on this demo project.

...althrough you cannot export the project without a native version ☹️

# Community's native Godot 4.4 with patches, called GDLE

If I will have free time and Godot 4.5 comes out before 4.4.2 (which is unlikely to release, like 4.3.1, which was not released yet (and possibly, won't release)),
I can make a community-based Godot 4.4.x fork with Vulkan bugfix, and possibly other fixes, that weren't included in official 4.4.2 dev branch.

Unlike Web 4.5, this version can actually export to old devices.