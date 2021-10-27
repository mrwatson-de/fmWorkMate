# Using fmAutoMate to convert Perform Script from List to Perform Script by Name


I recently changed the script which prepares fmWorkMate for release and used fmAutoMate to automatically convert a hard coded `Perform Script [ "from list" ; ... ]` to a soft coded Perform Script `Perform Script [ "by name" ; ... ]`

The old script to prepare the release of fmWorkMate simply called the Prepare Release Script in every tool:

```
# Developer Tools
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmCheckMate” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmLogAnalyser” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmDBAnalyser” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmSyntaxColorizer” ; Parameter:    ]
# 
# Text Tools
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmTextConverter” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmTextDiff” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmTextMultiplier” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmTextSeries” ; Parameter:    ]
# 
# Clip + Key Tools
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmPasteMate” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmClipboardViewer” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmKeyPress” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmModifierKeys” ; Parameter:    ]
# 
# Utilities
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmLaunchPad” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release and Close” from file: “fmAutoMate” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “myMateJSON” ; Parameter:    ]
# fmSimpleCalculator
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmPluginMate” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmKillDefaultFields” ; Parameter:    ]
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmLatencyMeter” ; Parameter:    ]
# 
# In Dew
Perform Script [ Specified: From list ; “Prepare Release” from file: “fmSetupAssistant” ; Parameter:    ]
# 
# fmWorkMate
Perform Script [ Specified: From list ; “Prepare Release” ; Parameter:    ]

```

Since this script was originally written various tools have been extracted to their own external repositories, so I want to change this 'prepare all' process to a 'prepare only tools in the fmWorkMate repo'.

This new method should use a new flag field in the tool settings to find just the fmWorkMate-repo tools and then run the script in their file using `Perform Sript [ 'by name' ; … ]`

The final script is like this:


