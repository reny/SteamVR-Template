﻿# SteamVR-Template
I propose here a Steam VR Template. It's a work in progress and I would like very much that we all contribute to.

I've included the final Vive controllers, with the animated triggers. Just drag and drop the Vive_Pawn in your game and voilà!

To install, just unzip into the appropriate Templates directory like C:\Program Files\Unreal Engine[Version]\Templates for launcher version or 	[ForkLocation]\UE4\Templates for source version. Launch a new project, and you'll find it in the blueprint section.

Templates are always tested on 2 different systems before uploading. It works.

[B]As seen in other threads, there is currently a bug in multiplayer (local) mode. We have 2 Vive there but we'll wait until the ticket is resolved before working on multiplayer mode.[/B]

[B]Version 1.1 - UE4.11.0: April 6, 2016 (project files)[/B]
-Animated triggers in both controllers
-Map of all buttons/trackpad on controllers
-Toggle on/off debugging squares of controllers and/or base stations

[B]Version 1.2 - UE4.11.1: April 7, 2016 (project files)[/B]
-More precise animated triggers in both controllers

[B]Version 1.3 - UE4.11.1: April 10, 2016 -- now as a template![/B]
-Finger tracking on trackpad
-Trace line with trigger
-Teleportation with cone validation
-Toggle on/off debugging meshes of base stations
-Force feedback

[B]Version 1.4 - UE4.11.1: April 13, 2016[/B]
-Added animated "grabbing" mesh right hand (will be refined) -- can be used instead of right controller mesh
-Teleportation with trackpad à la The Lab
-Go/No go teleportation zones
-Force feedback following teleportation (different for each controller)

[B]Version 1.5 - UE4.11.1: April 14, 2016[/B]
-Reduced recourse to event tick
-Event tick on/off ([B]by default event tick is off -- press upper menu button to enable tick[/B])
-Addition of 2 moving platforms for testing purpose: one by simple actor move and another moved by matinee
-Toggable particles system at the 4 chaperone corners and at the center
-Teleportation on platforms is now possible -- without being moved (see bugs)
-Addition of a cone at the tip of the right trigger -- can be rotated

Demo v1.1 at [url]https://youtu.be/BYzwl1n-7gE[/url] 

[B]Not working yet[/B]
Object pickup (i.e. conductor's baton)

[B]Bugs[/B]
Debugging squares of controllers and base stations do not follow after teleportation
Cannot be moved while on moving platforms
While teleportation and interaction with meshes works, [B]it seems that the SceneRoot (initially at 0,0,0) doesn't move with the pawn[/B]. The previous 2 bugs probably are the result of this discrepancy).
Fading camera when clipping through no go zones (i.e. walls) will result in system crash -- whether UE4 or entire system (reboot) -- beware!

[B]To do list[/B]

1)Resolve bugs --- [U]primarily resolving moving SceneRoot will resolve most problems[/U]
2)Enable pickup

Also:
-Leap motion integration
-Adapt chaperone size to scene / scene to chaperone size (not sure if feasible/pertinent)
-Animated hands meshes (more)
-Teleportation particles system
