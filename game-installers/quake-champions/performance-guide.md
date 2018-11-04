HOW TO OPTIMIZE QUAKE CHAMPIONS 
================================================

Better frametimes = Smoother gaming experience
-----------------------------------------------
Your screen can only render as much FPS as Hz has. This mean, that having more FPS won't make the game faster, nor it's going to eliminate stuttering. How do we get rid of it then?


* Limit your FPS to 62 (The refresh rate of your screen+4%).
* Disable V-Sync
* Set your graphics to low

**Optionally**: 
If you want to experiment by yourself, you can enable the [frametimes graph](https://i.imgur.com/5UkiBri.png) with the env variable

    export DXVK_HUD=frametimes

You will see something like [this graph](https://i.imgur.com/5UkiBri.png). Take a good look to your Min and Max frametimes. The less difference there's between both values, the less stuttering you are going to experience.


Low FPS - Determining the cause
-----------------------------------------------
There are 3 possible causes for low FPS:

**CPU**
This is the most common issue. If you can, enable some kind of CPU monitor, and make sure that your CPU it's not working at 100% capacity. If so, you have a bottleneck there, and you need a more powerful CPU. 

**GPU**
Once your CPU is not working at 100% capacity, the better your GPU is, the more FPS you are gonna get. As simple as that. Luckly most modern GPUs can run QC at 60 stable FPS (yes, on linux too).

**MEMORY**
You need at least 4 Gb to run Quake Champions. If you don't, the game will run really slow, and possibly even make your PC frozen.


The game still gets stuck
-----------------------------------------------
There are two possible causes for this:


**You just installed the game**: 
Vulkan need some time to fill the shader cache. After a couple of matches, the FPS should be 100% stable. This also happens when you update your GPU drivers, or DXVK.


**QC is very bad optimized**: 
Sorry to be harsh here, but it's true. No matter how good your system is, you still are going to experience FPS spikes in 3 moments: When you die, when you respawn, and when you use a portal. This problem also exists on Windows. Luckly most of the time it's not very noticeable.



Other minor optimizations
-----------------------------------------------
Take a look to [Lutris performance guide](https://github.com/lutris/lutris/wiki/Performance-Tweaks).