# Setting up fmWorkMate as a Separate App using fmLaunchPad


Here is how you can use [fmLaunchPad][fmLaunchPad home] to create a separate [fmWorkMate][fmWorkMate home] app.

**On Windows**

...you can open fmWorkMate in a second FileMaker **only with a different version of FileMaker** on your system

**On Mac**

...there is a much more elegant solution using fmLaunchPad.

Once you have [downloaded fmWorkMate from GitHub][fmWorkMate repo]...

1. Create a **seperate FM-app** for fmWorkMate
    - Duplicate your FileMaker Pro app (in your Applications folder), and rename it to 'fmWorkMate.app'
    - Place it in the fmWorkMate Folder alongside the fmWorkMate files
    - For added comfort, you can also replace the app's icon using the icon in the Finder (See [How to change Mac app icons](https://9to5mac.com/2019/01/17/change-mac-icons/))
    - You *could* stop here, and just open the fmWorkMate app and save it as a FileMaker favourite...
    - ...but we can do better than that...

2. Use **fmLaunchpad** (with fm19 - or fm18)

    ![fmLaunchPad logo][fmLaunchPad logo]

    [fmLaunchPad][fmLaunchpad home] is a cool little starter file 🚀 rocket you can 'programme' to open the file you really want to open.

    You'll be setup in just 3 or 4 steps:

- [Download fmLaunchPad from GitHub][fmLaunchPad repo] and place it next to fmWorkMate
    - or, alternatively, place the fmLaunchPad *folder* next to the fmWorkMate *folder* in your Applications folder

- Setup the FileMaker starter file -> fmLaunchPad
    - In fm19+
    - Open your fmWorkMate.app
    - In Preferences set the starter file to start fmLaunchPad
    - Close it again
    - Note: the starter file is valid for all fm18 and higher!
    - In fm18 (if you have no fm19)
    - While originally you could only set the starter file during installation of the FileMaker Client, it is also possible to set the preference from the command line. 
    - See ["Setting FileMaker’s startup file from CLI" from Beezwax](https://blog.beezwax.net/2020/06/09/setting-filemaker-startup-file-from-cli/)

- Open your fmWorkMate App again
    - We have lift off! 🚀
        
    With a bit of luck fmLaunchPad should open and automatically launch the fmWorkMate file :D

    If not, fmLaunchPad might need tweaking (and in these very early days of release 1.0 it is quite likely):
- Tweak/Setup fmLaunchPad
    
    Since the FileMaker startup file setting is a global setting which applies to all FileMaker version >= 18, you will also have to set up the starting conditions for your OTHER FileMaker files

    - Start fmLaunchPad again
    - Press the Abort button to stop the mission
    - Switch view (button top right) to see all the rocket's modules
    - Remove, reorder or setup the rocket's modules as necessary
    - Each module represents a different starter-mission
        - Left is the mission's start condition
        - Middle is the destination file you want to reach
        - Right are mission settings (try out capsule)
    - See the documentation in [fmLaunchPad][fmLaunchpad home] for details how to do that!

3. You're good to go - have fun! :)

[fmWorkMate repo]:https://github.com/mrwatson-de/fmWorkMate
[fmWorkMate home]:https://fmWorkMate.com/fmworkmate
[fmLaunchPad home]:https://fmWorkMate.com/fmlaunchpad
[fmLaunchPad logo]:https://raw.githubusercontent.com/mrwatson-de/fmLaunchPad/main/fmLaunchPadLogo_256_sm.png
