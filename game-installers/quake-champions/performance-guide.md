HOW TO OPTIMIZE QUAKE CHAMPIONS 
================================================

Better frametimes = Smoother gaming experience
-----------------------------------------------
Your screen can only show as many FPS as Hz supports. This means, that having more FPS won't make the game faster, nor it's going to eliminate stuttering. How do we get rid of it then?


* Limit your FPS to 60 (The refresh rate of your screen).
* Disable V-Sync.
* Set your graphics to low.

**Optionally**: 
If you want to experiment by yourself, you can enable the [frametimes graph](https://i.imgur.com/5UkiBri.png) with the env variable

    export DXVK_HUD=frametimes

You will see something like [this graph](https://i.imgur.com/5UkiBri.png). Take a good look to your Min and Max frametimes. The less difference there's between both values, the less stuttering you are going to experience.

**For Gsync/Freesync monitor users:** You must unlimit your FPS and enable Vsync in the game settings in order to use this feature. Also, make sure you enable it in your drivers settings, and in your screen.


Low FPS - Determining the cause
-----------------------------------------------
There are 3 possible causes for low FPS:

**CPU**: 
This is the most common issue. Enable the CPU monitor of your operative system, and make sure that your CPU is not working at 100% capacity. If this is the case, then you have a bottleneck.

**GPU**: 
Once you have discarded a CPU issue: The better your GPU is, the more FPS you are gonna get. As simple as that. In some cases, havig the last version of Wine, DXVK, and your GPU drivers, can help to increase FPS.

**MEMORY**: 
You need at least 4 Gb to run Quake Champions. If you don't have enough RAM, the game is gonna run very slow, and if you run out of virtual memory, the game will crash.


The game still gets stuck
-----------------------------------------------
There are two possible causes for this:


**You just installed the game**: 
Vulkan need some time to fill the shader cache. After a couple of matches, the FPS should be 100% stable. This also happens when you update your GPU drivers, or DXVK.


**QC is not 100% optimized**: 
Sorry to be harsh here, but it's true. No matter how good your system is, you still are going to experience FPS spikes in 3 moments: When you die, when you respawn, and when you use a portal. This problem also exists on Windows. Luckly most of the time it's not very noticeable.

**Check your mouse polling rate**: 
Some people experience a [known](https://github.com/doitsujin/dxvk/issues/1001) bug where using a polling rate of 1000 causes stuttering in all wine games. The cause of this issue are some motherboard manufacturers. Upgrading your motherboard firmware can fix this issue in some hardware (Confirmed for MSI B350 Tomahawk Arctic).


Other minor optimizations
-----------------------------------------------

* Take a look to [Lutris performance guide](https://github.com/lutris/lutris/wiki/Performance-Tweaks).
* [Setup your mouse](https://github.com/Zeioth/zeioth-lutris/blob/master/game-installers/quake-champions/mouse-guide.md).


Results you can expect
-----------------------------------------------
As long as your hardware has no bottlenecks, you can expect this kind of performance. [See video](https://www.youtube.com/watch?v=oHMOgV-8heM&t).
