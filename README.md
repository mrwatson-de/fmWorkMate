[![fmWorkMate logo][]][fmWorkMate home]

# fmWorkMate
[Makes FileMaker Work]

fmWorkMate is a power toolkit for FileMaker Developers from MrWatson of [mrwatson.de][mrwatson.de] and [fmworkmate.com][fmworkmate.com]

  ![Winner of the FileMaker Magazine Award for best FileMaker Tool 2018][FMM-Award 2018]

## Congratulations!
You have found fmWorkMate, the award-winning, free, open-source productivity toolkit for FileMaker developers from [MrWatson]!

LOTS has changed in fmWorkMate!

- fmWorkMate is now simply FileMaker files; the runtime version is no more ;-D
- fmWorkMate is now OPEN SOURCE, available on [GitHub][fmWorkMate repo] and under a [MIT LICENCE][LICENCE] !  👀 😃
- There are *loads* of new functions!(1)

The consequence of this is

- You'll need to bring your own [MBS licence][MBS-Plugin] [BYOL],
- You can take a look under the hood
- You can help make fmWorkMate a better tool - and are heartily invited to do so!

It's a new era - enjoy!

Check out the Website (coming in 2025) for loads more information.

Happy FileMaking!

MrWatson

2025-04-15

(1) For the latest changes check the commit meeages on GitHub, or the first script in each file documents all changes.

![mrwatson.de logo][mrwatson.de logo]


## What is fmWorkMate?

fmWorkMate is part of a [growing basket of tools from MrWatson][GitHub starred repos] that aim to make your FileMaker work better, more productive, more fun and colorful.

![fmWorkMate Tools View][]

These are the 'bits': 

- `fmWorkMate` - The main Toolbox with 15+ tools - [Repo][fmWorkMate repo]
- a function-packed extension library
  - `fmCheckmate-XSLT library` - Over 300 extension functions for fmCheckMate - [Repo][fmCheckmate-XSLT repo]
- 4 external tools
  - `fmSyntaxColorizer` - separate tool to colorize your code and brighten up your life - [Repo][fmSyntaxColorizer repo]
  - `fmAutoMate` - separate tool to integrate the power of fmWorkMate right into your script workspace - [Repo][fmAutoMate repo]
  - `fmLaunchPad` - separate tool to launch your files - [Repo][fmLaunchPad repo]
  - `myMateJSON` - separate tool to explore your JSON - [Repo][myMateJSON repo]
- a FileMaker IDE Integration Module
  - `fmScriptWorkspace` - IDE Integration Module - [Repo][fmScriptWorkspace repo]

## Why use fmWorkMate & co.?

Simple!

### `It's effective`

- fmWorkMate makes your FileMaker databases work!

  - *finds bugs* (Layout Analysis w. fmCheckMate-XSLT)
  - *catches bugs* at inception (fmLogAnalyser's Bug-Off! Alarm)
  - helps you *see bugs* by [making wrong code look wrong](https://www.joelonsoftware.com/2005/05/11/making-wrong-code-look-wrong/)  (fmSyntaxColorizer)
  - lists bugs to *kill* (fmLogAnalyser ToDo list)
  - takes you to *exactly* where the bugs are (fmScriptWorkspace)
  - *avoids* bugs by allowing you to *generate code* (fmCheckMate fmTextMultiplier)
    - (Better than hand coding 5% bugs into your solution!)
  - **proves** you have no bugs (fmLogAnalyser [OK])

- fmWorkMate works how you work!
  - Here and now!
    - fmWorkMate is designed for **immediate** use (and instant gratification 😉 )
    - no need to wait hours for DDRs to be created and analysed
    - just click + solve!
  - Fast and efficient!
    - fmWorkMate is honed for rapid and repetitive tasks


### `It's powerful`

- fmWorkMate provides help in places you need them, where other tools - inc. FileMaker itself - fail:
  - catch errors **as you make them** (fmLogAnalyser & Bug-Off Alarm)
  - find errors in layouts - *in seconds* (fmCheckmate Layout analysis)
  - refactor code
    - relocate functionality to a new context (fmTextConverter)
  - find differences in scripts
- fmWorkMate soothes where FileMaker hurts
  - dock that stupid debugger script window into the script workspace with a click!
  - jump straight to that subscript *in an external file*
  - test field calculations *without* having to add all the (default) table names back in to the data viewer.


### `It's proven`

- fmWorkMate has been in development since 2008 as a hobby alongside my 24*7 FileMaker work,

- It's been used daily be myself (MrWatson), colleagues, and increasingly more FileMaker developers around the world

- fmWorkMate has proven itself to be a valuable tool capable of considerably increasing daily productivity and championing the quality of your FileMaker work

- fmWorkMate was awarded the [FileMaker Magazin Award for Best Tool in 2018][FMM-Awards 2018]

  ![FMM-Award 2018]

### `It's free`
- Always has been.
- But now it is[ open source too][fmWorkMate repo]!

### `It's wild`

- fmWorkMate is out of the incubator and ready to be wielded!

 🥳 🎉 🥂



---

## Installing fmWorkMate

### To Install fmWorkMate on your Mac:

1. Download the [latest release][fmWorkMate releases] of fmWorkMate from [GitHub][fmWorkMate repo]
2. Move the fmWorkMate folder into the Applications folder (recommended, but anywhere will do)
   - Note: If you also have any sibling tools ([fmAutoMate][fmAutoMate home],  [fmSyntaxColorizer][fmSyntaxColorizer home] or [fmLaunchPad][fmLaunchPad home]) place the folders alongside each other in order to reference these tools from within fmWorkMate

3. Install Plugins, as necessary

   - Download and Install the two plugins, if you don't already have them
     - [Base-Elements Plugin Download](https://docs.baseelementsplugin.com/article/522-downloads) (free, no licence required)
     - [MBS Plugin Download](https://www.monkeybreadsoftware.com/filemaker/)
   - Licence / Register the MBS Plugin
     - You can get a [trial licence for MBS Plugin here](https://www.monkeybreadsoftware.com/trial/trial-filemaker.shtml)

   - If your solution already uses and registers a licenced MBS Plugin *and* you are using fmWorkMate in the *same* FileMaker instance, the MBS Plugin does not need to be registered again.
   - Otherwise, you can get fmWorkMate to register the MBS-Plugin when it starts:
     - Open fmWorkMate in FileMaker and setup plugin registration
       - Click the (i) button, bottom right in fmWorkMate
       - Click The MBS [BYOL] button (BYOL=Bring Your Own Licence)
       - Enter your licence information
       - Press [Register MBS]
     - If you wish to hide your MBS licence information from prying eyes...
       -  Navigate to the second slider panel
       -  Click [Store Licence] to store the current licence information
       -  Return to the first slider panel
       -  Remove your licence information
       -  [OK]

4. Launch fmWorkMate in FileMaker
   You can 
   1. Open fmWorkMate in FileMaker **alongside your databases**
      - The quickest way to get started
      - Has some advanages to interact between fmWorkMate + your files (see [fmAutoMate][fmAutoMate])
      - However, can sometimes be difficult to navigte between database + tool windows 
   2. Open fmWorkMate **in a second FileMaker version/instance**
      - This has the advantage of being able to switch between databases and tools easily
      - (Did you know you it is possible to just duplicate the FileMaker app on Mac?)
   3. Use **fmLaunchpad with a customised fmWorkMate.app** 
      - [fmLaunchPad][fmLaunchPad home] makes it possible to start different FileMaker solutions in different FileMaker apps
      - This takes a [little setting up][fmLaunchPad setup fmWorkMate], but provides a pleasant runtime-like experience

### To Install fmWorkMate on your Windows PC

- Either (for limited, but tried and tested, functionality - since fmWorkMate has not been developed/tested further on Windows since the demise of runtimes):
  - Download and install the old [fmWorkMate Windows Runtime] for basic functionality
  - You can also install fmCheckMate-XSLT
- Or (for a better future for all Windows FM-Devs - but maybe not such a good inital experience  for yourself):
  - Help [contribute] to getting fmWorkmate running on windows!
  - Download and install fmWorkMate as for mac
  - Test it, log [issues here in GitHub](https://github.com/mrwatson-de/fmWorkMate/issues) and [join in][contribute]!

---
## Using fmWorkMate

Feel free to click around to get to know the tools.

For a more guided start, see the [fmWorkMate documentation](docs/README.md).

---

## KNOWN ISSUES

- Not everything is tested (but core stuff is *used* every day).

- You can break things. Test before you try.

- FileMaker itself does not copy & paste all objects 100% correctly (notably the Import Records script step and the calculation context table in field definitions)

- Pasting entire tables, scripts and custom functions creates new objects with new internal IDs. So you may want to just copy the *contents* of an object

---

## GET INVOLVED

Please help improve fmWorkMate for us all. See [CONTRIBUTING][contribute]

---

## POKE around

I nearly forgot: If you want to poke around and have a look at the guts of fmWorkMate, you'll need the 'secret' user/password: admin/admin

---

## Links

- fmWorkMate
  - [fmWorkMate home][fmWorkMate home]
  - [fmWorkMate repo][fmWorkMate repo]
  - [fmWorkMate discussions][fmWorkMate discussions]
  - [fmWorkMate wiki][fmWorkMate wiki]
  - [fmWorkMate issues][fmWorkMate issues]
- Related Tools
  - [fmAutoMate][fmAutoMate home]
  - [fmLaunchpad][fmLaunchpad home]
  - [fmSyntaxColorizer][fmSyntaxColorizer home]

[Base-Elements-Plugin]:https://docs.baseelementsplugin.com/article/522-downloads
[contribute]:CONTRIBUTING.md
[fmAutoMate home]:https://www.fmworkmate.com/fmautomate
[fmAutoMate repo]:https://github.com/mrwatson-de/fmAutoMate
[fmCheckMate-XSLT home]:https://www.fmworkmate.com/fmcheckmate-xslt
[fmCheckMate-XSLT repo]:https://github.com/mrwatson-de/fmCheckMate
[fmLaunchpad home]:https://www.fmworkmate.com/fmLaunchPad
[fmLaunchPad logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,256x256/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/4121d384-3011-46ac-ba5d-51f7d4aefa2e~110/original?tenant=vbu-digital
[fmLaunchPad repo]:https://github.com/mrwatson-de/fmLaunchPad
[fmLaunchPad setup fmWorkMate]:Setting_up_fmWorkMate_with_fmLaunchPad.md
[FMM-Awards 2018]:https://filemaker-magazin.de/magazin/fmm-award-preistraeger/
[FMM-Award 2018]:docs/img/FileMaker_Magazin_Award_IMG_9704_700px_small.jpg

[fmScriptWorkspace repo]:https://github.com/mrwatson-de/fmScriptWorkspace
[fmSyntaxColorizer home]:https://www.fmworkmate.com/fmsyntaxcolorizer
[fmSyntaxColorizer repo]:https://github.com/mrwatson-de/fmSyntaxColorizer
[fmWorkMate discussions]:https://github.com/mrwatson-de/fmWorkMate/discussions
[fmWorkMate home]:https://www.fmworkmate.com/fmWorkMate
[fmWorkMate issues]:https://github.com/mrwatson-de/fmWorkMate/issues
[fmWorkMate logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,128x128/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/ad76e3a4-92d7-4851-a8a4-7e7f88b8f159~110/original?tenant=vbu-digital
[fmWorkMate logo]:docs/img/fmWorkMate_ICON_200x200_sm.png
[fmWorkMate releases]:https://github.com/mrwatson-de/fmWorkMate/releases
[fmWorkMate repo]:https://github.com/mrwatson-de/fmWorkMate
[fmWorkMate Tools View]:docs/img/fmWorkMate-long-view-2021-07-27.png
[fmWorkmate tube]:https://www.youtube.com/channel/UCZk3uKObkoUT_x2mOV35Kxw
[fmWorkMate wiki]:https://github.com/mrwatson-de/fmWorkMate/wiki
[fmWorkMate Windows Runtime]:https://github.com/mrwatson-de/fmWorkMate-Archive-Win
[fmworkmate.com]:https://fmworkmate.com
[GitHub starred repos]:https://github.com/mrwatson-de?tab=repositories&q=&type=source&language=&sort=stargazers
[LICENCE]:LICENCE.txt
[MBS-Plugin]:https://www.monkeybreadsoftware.com/filemaker/
[MrWatson]:http://www.mrwatson.de
[mrwatson.de logo]:www.mrwatson.de_neon_128.png
[mrwatson.de]:http://www.mrwatson.de
[myMateJSON repo]:https://github.com/mrwatson-de/myMateJSON
[PLACEHOLDER TEMPLATES]:https://useTheFollowingTemplates
[ToolName home]:https://www.fmworkmate.com/toolname
[ToolName repo]:https://github.com/mrwatson-de/ToolName
