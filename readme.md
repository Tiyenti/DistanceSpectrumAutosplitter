# Distance Spectrum Autosplitter
This is a Spectrum plugin that provides automatic splits, resets, and an IGT timer for Distance speedruns
through LiveSplit Server.

This is very early in development. I haven't actually used this in a full run yet, so I don't know if
everything works properly (it should). This currently supports both Adventure, Sprint SS, and Challenge SS
runs. All Levels may or may not be added due to complexity.

If you want to play the game without having the timer split a bunch on you, just stop the server in LiveSplit.
It should handle it just fine.

**Note**: It is not yet decided whether or not using Spectrum will be allowed for runs, so this might be useless.
We'll see. 

## How to use
First, install the LiveSplit Server component: https://github.com/LiveSplit/LiveSplit.Server/releases

After you've done that, you need to add the LiveSplit Server component to your layout. Then right-click on
LiveSplit, go into the Control submenu, and select Start Sever. Note that you must do this every time you
start LiveSplit. The plugin will attempt to connect to the server immediately once loaded - if it fails,
it will re-attempt just before you start a run.

Note: If you want to use RTA timing, you will have to start the timer manually; do not use the automatic
start for timing runs in real time, it is not accurate to the timing method actually used. You won't have
to worry about anything if you use IGT, though, apart from the fact there is no game time field on the sr.c
boards yet. So you probably won't want to actually use that part of the autosplitter yet.

You then need to install Distance Autosplitter plugin. Grab the latest .dll from the
[releases page](https://github.com/TntMatthew/DistanceSpectrumAutosplitter/releases), and drop
it in your `Distance_Data/Spectrum/Plugins` directory. And you're done - the timer will
automatically start once IGT begins, and will split after each level is completed.