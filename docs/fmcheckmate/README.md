![fmCheckMate logo][fmCheckMate logo w100]

# fmCheckMate Documentation

Here you can learn about fmWorkMate´s fmCheckmate Tool.

## What is fmCheckMate?

fmCheckMate is the core tool of the fmWorkMate toolbox.

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

---

## GETTING STARTED with fmCheckMate

You can get started without doing any set up.




### The fmCheckMate Editor

[Pic]


## Setting up fmCheckMate

In the fmCheckMate settings 

- fmCheckMate mode
  - 
- Editor
  - Size & window positioning
  - 
- XML
  - search highlighting
  - syntax highlighting
  - formatting
- Functions
  - 
- File
  - interaction with an external file & editor
  - saving of iDDR ('instant DDR') files


Open the Settings (CMD+9) to choose the mode.

Another CMD+9 takes you to the detailed settings.

There you can

- turn tips on/off
- define window size / behaviour
- etc.


### **Four** Modes of Operation

fmCheckMate has four different modes of operation

1. **Convert/Transfer** Mode
   - which just converts the clipboard, but does not display the XML
2. **Internal Editor** Mode
   - for quick editing & transforming of your XML
   - Choose between small or large editor
3. **External Editor** Mode
   - for power-editing in your preferred editor
4. **Analysis** mode
   - for quickly selecting appropriate analysis functions (for example for focussed Layout Analysis)

The default mode is 'Small Internal Editor' which displays the XML in a small window after conversion.

### Further fmChekMate Settings

[TODO]

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




[fmCheckMate logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,1562x992/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/f751064a-5344-49a0-b891-f838b5318889~110/original?tenant=vbu-digital

[fmCheckMate-XSLT logo w100]:https://imageprocessor.digital.vistaprint.com/crop/0,0,426x365/maxWidth/100/https://uploads.documents.cimpress.io/v1/uploads/135c8327-b2ee-4d68-a1a8-c93d15ed02fa~110/original?tenant=vbu-digital
[fmCheckMate XSLT repo]:https://github.com/mrwatson-de/fmCheckMate
