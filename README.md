# arkanhockey
Arkanhockey BETA file (only index file) - the game and the platform is in beta and I will definitely rewrite to clean up and fix a number of known issues hence the code might change completely from one day to another.

ArkanHockey is a top-down game built using a platform I'm developing that I plan to call "Arkan".

>The platform will allow easy implementation of game logics, sprites animation, physics, a simple input controls, both by multitouch and by keyboard / mouse. Cross compatible between different devices and different browsers aiming to run smoothly on mobile devices (not necessarely high-end devices).

* No external libraries
* Garbage collector friendly (aim to reduce GC as much as possible)
* Object pooling - Array pooling
* Sprite images for animations, either using an image or using canvas to create a sprite
* Sound either with <audio> tag (supporting multiple layers or 1 layer) or Web Audio API (with support for both the old Web Audio API and the new). The use of audio is always the same across all the modes: audio1.play() audio1.pause()
* Rendering - 3 modes: Canvas precaching, rendering images, render anew all the times
* Physics - Shapes avail: blocks, circles or dot supported. In the future will add triangles and maybe custom geometries. All objects can be "triggers", can associate actions once 2 or more objects collide together. Objects can also be "static" (not affected by gravity nor pushforce but other objects bounce against this one), "dynamic" (affected by pushforce and gravity and can be controlled by the user), "phantom" (not affected by gravity nor pushforce from other objects, other objects are not influenced by this object but code detects when 2 objects overlap each other)
* API for mouse / keyboard events - inputs
* Custom image fonts can be used in .png format
* Some debugging functionality like time spent on rendering or logics or physics etc...
* HTML5 storage, save and load game data
* Offline - game can be played offline with HTML5 caching
* Full screen mode ready - needs some more work
* API to create and handle menu and buttons

