Dead Trigger - PortMaster Port

A highly experimental and **extremely fragile** port of Dead Trigger 1 to ARM Linux handhelds (R36S and similar), built on top of [BinaryCounter's Bogodroid](https://github.com/binarycounter/Bogodroid) — a highly experimental framework for running NDK Android apps on ARM Linux.


## ⚠️ SET BINDS LIKE THIS FOR OPTIMAL GAMEPLAY
L1= shoot
r1= aim
x=reload
l2= previous weapon
r2= next weapon
move right= left stick right
move up = left stick up (stops right stick movement glitches, should result in up and right like image below
pause= start
BUTTONS MAY HAVE TO BE REPEATEDLY INPUTTED UNTIL REGISTERED PROPERLY!
<img width="640" height="480" alt="IMG20260708234501" src="https://github.com/user-attachments/assets/6b071484-4aa2-4d1f-b015-44834d7cbf24" /># 


This port uses Bogodroid's `unityloader` shim to get the game's Unity runtime booting on-device. It works, but it is held together with duct tape and good intentions.

## ⚠️ Status: Experimental / Unstable

This is **not** a polished, plug-and-play port. Expect:

- UI/HUD clipping issues (the game's native 16:9 Unity canvas doesn't map cleanly onto 4:3 handheld panels like the R36S's 640x480 display)
- Possible instability, crashes, or degraded performance depending on your device
- Rough edges anywhere Bogodroid's Android-compatibility shimming has to improvise

If something breaks, that's expected at this stage — this is a first-boot-working proof of concept, not a finished, QA'd release.

## ⚠️IMPORTANT⚠

**You MUST use Dead Trigger version 2.1.0.**

Other versions of the APK/game data are **not guaranteed to work** and may fail to boot, crash, or behave unpredictably under Bogodroid's shim. This port was built and tested specifically against 2.1.0.

Place your obtained Dead Trigger 2.1.0 game data in:

```
deadtrigger/gamedata/
```

The port will not function correctly (or at all) if the wrong version is used or the game data is placed elsewhere.

## Credits

- [BinaryCounter](https://github.com/binarycounter/Bogodroid) — for Bogodroid, the framework that makes running this NDK Android app on ARM Linux possible at all


## Disclaimer

You must own a legitimate copy of Dead Trigger. This repository does not include or distribute game data. This port is provided as-is, with no guarantees of stability, performance, or compatibility across devices.
