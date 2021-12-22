# So what is RZDoom?
It will be a minimal, stripped-down version of ZDoom 2.8.1 with bug fixes, my additions and my optimisations for many systems.

# Why is it needed?
In my own opinion, ZDoom is too big with too many additions for one person to properly maintain. I'm not interested in pleasing everyone, I don't care about supporting impossibly old systems (XP) or having pointless X64 assembly when our processors are plenty fast enough without it.

So this will contain features I deem 'sensible' for a Doom source port.

# Differences

You will notice differences to ZDoom 2.8.1, largely about the difference in Sound Systems / Backend Choices.

As RZDoom now uses FMOD Studio (not the legacy FMOD Ex) sound API as standard, support was dropped for a number of sound backends and outputs (because FMOD Studio removed them).  These are the 'HRTF' lowpass output, XMA, Direct Sound etc..

Windows only WASAPI, and ASIO remain (WASAPI being the default on all modern Windows).
Linux only ALSA and Pulse Audio.
macOS only Core Audio.

Wildmidi, Timidity, Fluidsynth, OPL etc..  remain as you remember them.

# Notices
Master branch is inherently unstable, expect bugs if you compile from there. Feel free to report anything you wish, I'll be happy to work with you on them. Of course, I do debug it myself often.
