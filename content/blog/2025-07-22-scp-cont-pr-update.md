<!-- title: SCP: Containment Procedures big update -->
# Update 2.0
## Added SCP-914
I added SCP-914, which has an unlimited creativity to make new tasks.

![SCP-914](./content/images/scp_cont_pr_screen2.png)

Currently, only 4 tasks are added and you cannot refine a NPC.

## Added Maintenance Zone (previously used in SCP: Unstable Dimension)
Previously in 1.0.0, this zone was hidden in the files and was not usable.

I decided to make a return of Maintenance Zone in this update.

I fixed bugs in Map Generator (updates 8.1.2-8.1.4), introduced checkpoints and I integrated this zone + I moved SCP-812 here.

\[Screenshot deleted in 2025.11.09\]

## Miscellaneous
I rewrote pointer script to include also a ShapeCast!

ShapeCast is used for following NPCs or picking items (they were incroduced with SCP-914),
while RayCast will continue to be used as point-to-walk.

Also you can disable music 🙂

## 2.0.1 Bugfix update

### Android optimizations

Since Update 2.0 increase zone size for checkpoints and added a whole new zone, optimization on mobile devices got worse...

I reduced visible range of the map and disabled Glow and Reflection probes on all of Android.

### Bugfixes
- Scientists at SCP-650 containment chamber now have IK disabled (previously they looked strange)
- You cannot pick-to-follow MTFs, Chaos Insurgency, hostile SCPs and scientists at SCP-650 chamber
- Labels at checkpoints are supporting translations!
- Made color of SCP-812 waterfall more realistic
- Tried to fix bug, where Chaos Insurgency event was not called if there was SCP-347 MTF task.

# Conclusion

SCP; Containment Procedures is my second project which I am currently doing, and it
will stay non-commercial for foreseeable future.

Currently, it is on the second priority due to Internal Eternal development, but it can be first priority, when I am finding the job - 
because this game is not commercial (and also GPL-licensed) (unlike Internal Eternal in the future), it is much easier to continue this game in free time.