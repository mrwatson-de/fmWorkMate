[![fmWorkMate logo][fmWorkMate logo]][fmWorkMate home]

# fmWorkMate Documentation
[Makes FileMaker Work]


# Welcome

Welcome to the new home of fmWorkMate documentation.

I hope the documentation will flourish here!

Please give feedback & ideas in [discussions][fmWorkMate discussions] or on the  [issues tab][fmWorkMate issues]!

## What is fmWorkMate?

fmWorkmate is a collection of free Tools from MrWatson for FileMaker database developers.

It's a toolbox *full of goodies* that you can use in your daily work as a FileMaker developer to make  your daily job easier, more productive and more colorful.

## Contents


- Setting up 
  - If you haven't got fmWorkMate installed and started yet, first see [Getting started with fmWorkMate](../README.md#getting-started-with-fmworkmate)
  - If you have multiple versions of FileMaker see [Setting up the target FileMaker app][Target FileMaker]
- [fmWorkMate Interface](#fmworkmate-interface)
- [Navigating in fmWorkMate](NavigatingInFmWorkMate.md)



## fmWorkMate Interface

Here it is (as of 2021-10-29):

![fmWorkMate Tools View][fmWorkMate Tools View]

When fmWorkMate is opened you are presented with a list of tools

- Click a [tool](#getting-to-know-the-tools) to launch it
- Grey keys to the right of buttons inidicate the shortcut key for that button
  - Press <img src="img/CmdCtrl_31_green.png" height="16"/> + the shortcut key(s) to launch the tool
> Note: This documentation uses the symbol  <img src="img/CmdCtrl_31_green.png" height="16"/> to indicate the operating system specific command invocation key: Command key on Mac and Ctrl key on Windows

- The grey arrows indicate a tool will be opened in the target FileMaker  (rather than the current FileMaker - because some tools need to interact with FileMaker directly.)

Other features on the page, from top to bottom:

  - <img src="img/fmWM_SwitchFMButton.png" height="24" style="vertical-align:-30%;"/> - [Current Target FileMaker indicator][Target FileMaker] → If you have set up multiple FileMaker targets, you can click here to target a different FileMaker instance.
  - <img src="img/fmWM_NewsButton.png" height="48" style="vertical-align:-90%;"/> → shows latest news from MrWatson
  - <img src="img/fmWM_HelpButton.png" height="16"/> → Tool Help & Settings
  - <img src="img/fmWM_VersionButton.png" height="12"/> - Version number → About, Tool Versions and Credits pages
  - <img src="img/fmWM_InfoButton.png" height="16"/> → fmWorkMate Settings



## GETTING TO KNOW the Tools

Here is a quick overview of the tools (as of 2021-09-28)

### The Developer Tools

The Developer Tools form the (original) core of the fmWorkMate toolbox:

[`fmCheckMate`](fmCheckmate/README.md)
- fmCheckMate is the central tool of the fmWorkMate toolbox.
- It converts the clipboard between FileMaker code and its XML representation.
- It thus enables the transfer of code to/from remote machines with copy & paste.
- You can edit your code in the inbuilt xml editor, for example to rename script variables.
- With the `fmCheckMate-XSLT Library` you can Analyse, Change and Transform your FileMaker code - in ways that will make your jaw drop!

`fmCheckMate-XSLT Library`
 - The `fmCheckMate-XSLT Library` is a [separate repository][fmCheckMate-XSLT repo] providing a set of functions (XSL Transformations and shell scripts to be precise) which `fmCheckMate` uses to Analyse, Change and Transform your FileMaker code.
 - This is the most powerful aspect of the toolbox, and not to be missed!

`fmLogAnalyser`
- fmLogAnalyser is a viewer for the FileMaker import.log (and other log) files.
- It turns pasted/imported broken code into a to-do list!
- With its Bug-Off! Alarm fmLogAnalyser helps you catch every single possible bug **before** they infiltrate your database code - by alerting you *immediately*!

`fmDBAnalyser`
- fmDBAnalyser is maybe the oldest tool in the toolbox.
- It reports information about the tables, fields, layouts, scripts, value lists in your database.

`fmSyntaxColorizer`
- fmSyntaxColorizer is the best way to make your script and calculation code colorful *and meaningful*.
- It is an external tool, so see the [fmSyntaxColorizer homepage][fmSyntaxColorizer home] for more.

### The Text Tools

The Text Tools provide basic text manipulation functionality

`fmTextConverter`
- fmTextConverter is a tool to perform multiple substitutions
  - It is indeed a (very souped-up!) wrapper for the Substitute function
- It makes it possible to convert code betweeen contexts (eg: SalesOrder → Invoice / SO → INV )

`fmTextDiff`
- fmTextDiff is a text diffing tool
  - It is a wrapper around an online diffing service…
    - …at least, until someone has time to implement a webviewer based diffing algorithm! ;-)
    - …So be aware, if you use it, that your code is being passed to a third party!
- With fmTextDiff (aided by `fmCheckMate`) you can extremely quickly discover what the differences are between two scripts, tables, texts, ... whatever!

`fmTextMultiplier`
- fmTextMultiplier is a neat way of 'multiplying up your code'
- It too is a (also souped-up!) wrapper for the Substitute function, but it generates a result for each substitution rather than applying each substitution sequentially.
- It is best illustrated by example:
  - If you 'multiply' "A→B¶"
  - by "B¶C¶D¶"
  - you get "A→B¶A→C¶A→D¶"
- While this may not seem particularly useful at first sight, if you have some FileMaker code with a specific field, and a list of fields that should be treated the same, ... well, just imagine!

`fmTextSeries`
- fmTextSeries is a tool to produce a sequential list of values
  - It is indeed just a wrapper for the SerialIncrement function
- It is best illustrated with an example:
  - If you generate the series "Day 08 Text..10"
  - you get ""Day 08 Text¶Day 09 Text¶Day 10 Text"
- Again this may not seem so useful at first, but in combination with fmTextMultiplier you can rapidly generate code which operate on a series of fields or with a series of data.

Together with `fmCheckMate`and the  `fmCheckMate-XSLT Library` the Text Tools form a very powerful FileMaker code manipulation engine!

### Clip + Key Tools

The Clip + Key Tools help you deal with your clipboard and keyboard.

`fmPasteMate`
- fmPasteMate is a utility to transfer multiple objects efficiently using copy+paste
- It queues and rotates its contents so you can quickly and easily paste multiple items sequentially into your FileMaker database

`fmClipboardViewer`
- fmClipboardViewer shows you the contents of the clipboard
- and the names of the clipboard flavours

`fmKeyPress`
- fmKeyPress shows you the key and code of the key you pressed
- Great help when writing OnKeypress trigger scripts!

`fmModifierKeys`
- fmModifierKeys shows which modifier keys are currently pressed
- Useful when keys get 'stuck' down on remote machines

### More Utilities

Some really important utilities:

`fmAutoMate`
- fmAutoMate integrates functionality directly into your script workspace
- It can also be considered a core tool of the fmWorkMate toolbox.
- It is, however, developed in a [separate repository][fmAutoMate repo]

`fmLaunchPad`
- is a cheeky little rocket to help start the file you want when you want

`myMateJSON`
- myMateJSON helps you get your JSON straight!
- Explore JSON & write code automatically
- It is an external tool, see the [myMateJSON repository][myMateJSON repo] for more


And some less important utilities:

`fmSimpleCalculator`
- is a really simple little calculator
- with some very useful 

`fmPluginMate`
- fmPluginMate helps you manage your plugins
- Get a list of what is installed
- Install plugins on the fly with drag + drop

`fmKillDefaultFields`
- fmKillDefaultFields gets rid of those annoying standard default fields in a click
- Or locate the file if you wish to change it.

`fmLatencyMeter`
- fmLatencyMeter is a little clock to help show how good/bad the latency is to your remote machine
- Includes an example of how to use fmTextMultiplier to create objects at specific positions on a layout.


# fmWorkMate Settings

On the fmWorkMate setup page

  - Autofocus FileMaker
    - See [Setting up one/more Target FileMakers](#setting-up-autofocus-and-the-target-filemaker-app)
  - Plugins & MBS BYOL
     - See [Setting up MBS Plugin Registration](../README.md#setting-up-mbs-plugin-registration)
  - Simple Caclulator prefs

## Setting up Autofocus and the target FileMaker app

When you convert FileMaker code to and, moreover, back to FileMaker objects, fmWorkmate can focus the FileMaker app for you automatically.

You must

- select the option "AutoFocus FileMaker" in the fmWorkMate settings
- tell fmWorkMate which FileMaker app it should target

Note:

- You can choose multiple instances of FileMaker, and then swap between them from the 'current target Filemaker' indicator on the main page.
- The current target FileMaker app is also the app in which fmSyntaxColorizer, fmAutoMate and fmPluginMate will be opened.


See
- 



# Further sources of Knowledge

Check out the [fmWorkMate homepage][fmWorkMate home]

Watch stuff on the [fmWorkMate YouTube channel][fmWorkMate tube]

---




  

---

[More is coming]




[fmCheckMate-XSLT repo]:https://github.com/mrwatson-de/fmCheckMate

[fmWorkMate discussions]:https://github.com/mrwatson-de/fmWorkMate/discussions

[fmWorkMate home]:https://www.fmworkmate.com/fmWorkMate

[fmWorkMate issues]:https://github.com/mrwatson-de/fmWorkMate/issues

[fmWorkMate logo]:img/fmWorkMate_ICON_200x200_sm.png

[fmWorkMate Tools View]:img/fmWorkMate-long-view-2021-07-27.png

[fmWorkmate tube]:https://www.youtube.com/channel/UCZk3uKObkoUT_x2mOV35Kxw

[myMateJSON repo]:https://github.com/mrwatson-de/myMateJSON


[fmSyntaxColorizer home]:https://www.fmworkmate.com/fmSyntaxColorizer

[Target FileMaker]:#setting-up-autofocus-and-the-target-filemaker-app