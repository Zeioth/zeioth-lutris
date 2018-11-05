HOW TO OPTIMIZE QUAKE CHAMPIONS 
================================================

Better frametimes = Smoother gaming experience
-----------------------------------------------
Your screen can only render as much FPS as Hz has. This means, that having more FPS won't make the game faster, nor it's going to eliminate stuttering. How do we get rid of it then?


* Limit your FPS to 62 (The refresh rate of your screen+4%).
* Disable V-Sync.
* Set your graphics to low.

**Optionally**: 
If you want to experiment by yourself, you can enable the [frametimes graph](https://i.imgur.com/5UkiBri.png) with the env variable

    export DXVK_HUD=frametimes

You will see something like [this graph](https://i.imgur.com/5UkiBri.png). Take a good look to your Min and Max frametimes. The less difference there's between both values, the less stuttering you are going to experience.


Low FPS - Determining the cause
-----------------------------------------------
There are 3 possible causes for low FPS:

**CPU**: 
This is the most common issue. Enable the CPU monitor of your operative syste, and make sure that your CPU is not working at 100% capacity. If this is the case, then you have a bottleneck.

**GPU**: 
Once you have discarded a CPU issue: The better your GPU is, the more FPS you are gonna get. As simple as that. In some cases, havig the last version of Wine, DXVk, and your GPU drivers, can help to increase FPS.

**MEMORY**: 
You need at least 4 Gb to run Quake Champions. If you don't have enough RAM, the game is gonna run very slow, and if you run out of virtual memory, your game will crash.


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



Oh man this sucks... There's something else I can do?
-----------------------------------------------
Overclock your hardware. I only recommend this option if you have tried all the other points of this guide, but still can't get as much FPS as your screen refresh rate. Overclocking is safe 99% of the time, but remember, the consecuences are always YOUR responsability. Do it only if you know what you are doing.

**CPU**: 
Overclocking your CPU you can usually get up to 25% extra performance.

**GPU**: 
Overclocking your CPU you can usually get up to 25% extra performance.

**MEMORY**: 
Overclocking your RAM you can usually get up to 0% extra performance. (Don't believe me? Try it)
