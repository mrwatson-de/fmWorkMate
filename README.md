[![fmWorkMate logo][fmWorkMate logo]][fmWorkMate home]

# fmWorkMate
[Makes FileMaker Work]

fmWorkMate is a power toolkit for FileMaker Developers

...from MrWatson of www.mrwatson.de and fmworkmate.com

...and it's been in development since 2008 (as a hobby alongside my 24*7 FileMaker work),

...and it's been used everyday be myself, colleagues, and increasingly more FileMaker developers

...so let's call it Version 1.0, shall we?

 🥳 🎉 🥂

---

## Congratulations!
You now have the FREE OPEN-SOURCE version of fmWorkMate!

LOTS has changed since the last release!

- fmWorkMate is now OPEN SOURCE :-D
  - Not only open source, but [MIT LICENCE][LICENCE]
  - and avaliable on [GitHub][fmWorkMate repo]
- fmWorkMate is now simply FileMaker files.
  - and the runtime version is no more :-/
  - and (thus) you need to
    - bring your own MBS licence,
    - and download and install the [MBS-Plugin][MBS-Plugin] + [Base-Elements-Plugin][Base-Elements-Plugin] yourself.
      - *but you've probably got hose already :-)*
- There are *loads* of new functions!
  - I don't know where to start telling!
  - Take a peek in [fmWorkMate-Changes.txt](fmWorkMate-Changes.txt)

It's a new era! ... Please help make fmWorkMate better and contribute to a power tool for all FileMaker developers everywhere!

Happy FileMaking!

MrWatson

2021-06-11

![mrwatson.de logo][mrwatson.de logo]

P.S. fmWorkMate is not alone ... Check out my many other [real-good free tools][mrwatson.de].

---

## GETTING STARTED with fmWorkMate

![fmWorkMate logo][fmWorkMate logo w100]

fmWorkMate

1. Download fmWorkMate from [GitHub][fmWorkMate repo]
2. Move the fmWorkMate folder into the Applications folder (recommended, but anywhere will do)

3. Decide which FileMaker you wish to use to open the fmWorkMate files.
   
   TLDR: Just open fmWorkMate.fmp12 and get on with it
   
   You can 
   - either **open fmWorkMate with the same FileMaker** that you open your databases with
     - this requires you to hop between windows (which can be a **bit of a chore**, but might lead to some great integration possibilities later on)
     - just add fmWorkMate to your FleMaker favourites and you are good to go
   - or **open fmWorkMate with a second FileMaker** instance/version
     - this keeps fmWorkMate seperate from your databases, making it **easier to work with**
     - **On Windows** you can open fmWorkMate in a second FileMaker **only with a different version of FileMaker** on your system
     - **On Mac** there is a more elegant solution:
       1. Create a **seperate FM-app**
          - Duplicate your FileMaker Pro app, and rename it to 'fmWorkMate.app'
          - Place it in the fmWorkMate Folder alongside the fmWorkMate files
          - For added comfort, you can also replace the app's icon using the icon in the Finder
            - See [How to change Mac app icons](https://9to5mac.com/2019/01/17/change-mac-icons/)
          - You *could* stop here, and just open the fmWorkMate app and click the  fmWorkMate favourite...
            - ...but we can do better than that...
       2. Use **fmLaunchpad** (with fm19 - or fm18)
      
         ![fmLaunchPad logo][fmLaunchPad logo w100]

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

4. You're good to go - have fun! :)

---
## GETTING TO KNOW the Tools

![fmWorkMate Tools View][fmWorkMate Tools View]

Take a look at all those tools! // and that image is *old!* ;-)

Or check out the [fmWorkMate homepage][fmWorkMate home]

Or watch stuff on the [fmWorkMate YouTube channel][fmWorkMate tube]

---


## GETTING STARTED with fmCheckMate

![fmCheckMate logo][fmCheckMate logo w100]

fmCheckMate is the core tool of the toolbox.

You can

- **convert** FileMaker objects on the **clipbard to/from FileMaker** (fmxmlsnippet) XML
  - which alone is *great* for transfering code to/from a remote computer!
- search & replace the XML 
  - **rename variables**
  - **move code to a different layout context**
- view / edit the XML.
  - in the built-in XML-editor, or
  - in an external editor
- and - with the fmCheckMate-XSLT Library - you can perform hundreds of (quite frankly amazing) functions to analyse, change and transform your XML. (See below)

### fmCheckMate Modes

fmCheckMate has some different modes of operation

- Convert/Transfer
  - which just converts the clipboard, but does not display the XML
- Internal Editor (small or large)
  - for quick editing & transforming of your XML
- External Editor
  - for power-editing in your preferred editor
- Analysis mode
  - for quickly selecting appropriate analysis functions with 


### fmCheckMate Setings

Open the Settings (CMD+9) to choose the mode.

Another CMD+9 takes you to the detailed settings.

There you can

- turn tips on/off
- define window size / behaviour
- etc.



---

## GETTING STARTED with the fmCheckMate-XSLT Library

![fmCheckMate-XSLT logo][fmCheckMate-XSLT logo w100]

1. Install the fmCheckMate XSLT Librabry
   - Download the fmCheckMate XSLT Librabry from [GitHub][fmCheckMate XSLT repo]
   - Move the fmCheckMate folder into your Documents folder
2. Load the fmCheckMate XSLT Librabry into fmCheckMate
   - The first time you open the XSLT Chooser (by pressing the [T] button in the internal editor / CMD+T(ransform)) the fmCheckMate XSLT Library should be loaded into fmCheckMate
   - If not, use the reload button (or CMD+8)
3. Transform your Code
   - Copy some FileMaker objects (CMD+C)
   - Start fmWorkMate and choose fmCheckMate (CMD+2)
   - Convert the Clipboard (Big button or CMD+ALT+C(onvert) or CMD+2)
   - In the XSML-editor layout press the [T] button (or press CMD+T(ransform))
   - Choose a function
     - Change view & Browse the functions, or
     - Search by name
     - Filter by type
    - Press Return to Apply


  

---

[More is coming]

---

## KNOWN ISSUES


- Not everything is tested (but core stuff is *used* every day).

- You can break things. Test before you try.

- FileMaker itself does not copy & paste all objects 100% correctly (notably the Import Records script step and the calculation context table in field definitions)

- Pasting entire tables, scripts and custom functions creates new objects with new internal IDs. So you may want to just copy the *contents* of an object

---

## GET INVOLVED


Please help improve fmWorkMate for us all.

Got an issue?

Let us know -> [issues on GitHub][fmWorkMate bugs].

---


## POKING around

I nearly forgot.

If you want to poke around and have a look at the guts, you'll have to use the 'secret' user/password: admin/admin

---

## Links

- [fmWorkMate home][fmWorkMate home]
- [fmWorkMate wiki][fmWorkMate wiki]
- [fmWorkMate repo][fmWorkMate repo]
- [fmWorkMate bugs][fmWorkMate bugs]

[fmWorkMate bugs]:https://github.com/mrwatson-de/fmWorkMate/issues
[fmWorkMate home]:https://www.fmworkmate.com/fmWorkMate
[fmWorkMate wiki]:https://github.com/mrwatson-de/fmWorkMate/wiki
[fmWorkMate repo]:https://github.com/mrwatson-de/fmWorkMate
[fmWorkMate logo]:fmWorkMate_ICON_200x200_sm.png
[fmWorkMate logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,128x128/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/ad76e3a4-92d7-4851-a8a4-7e7f88b8f159~110/original?tenant=vbu-digital
[fmWorkMate Tools View]:https://imageprocessor.digital.vistaprint.com/crop/0,0,420x1332/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/db4884b9-c073-467e-9cb8-f2c136ba13cf~110/original?tenant=vbu-digital
[fmWorkmate tube]:https://www.youtube.com/channel/UCZk3uKObkoUT_x2mOV35Kxw

[MBS-Plugin]:https://www.monkeybreadsoftware.com/filemaker/
[Base-Elements-Plugin]:https://docs.baseelementsplugin.com/article/522-downloads
[mrwatson.de logo]:www.mrwatson.de_neon_128.png
[mrwatson.de]:http://www.mrwatson.de

[fmLaunchpad home]:https://www.fmworkmate.com/fmLaunchPad
[fmLaunchPad logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,256x256/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/4121d384-3011-46ac-ba5d-51f7d4aefa2e~110/original?tenant=vbu-digital
[fmLaunchPad repo]:https://github.com/mrwatson-de/fmLaunchPad

[fmCheckMate logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,1562x992/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/f751064a-5344-49a0-b891-f838b5318889~110/original?tenant=vbu-digital

[fmCheckMate XSLT home]:https://www.fmworkmate.com/fmcheckmate-xslt
[fmCheckMate XSLT repo]:https://github.com/mrwatson-de/fmCheckMate
[fmCheckMate-XSLT logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,426x365/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/135c8327-b2ee-4d68-a1a8-c93d15ed02fa~110/original?tenant=vbu-digital
[LICENCE]:LICENCE.txt