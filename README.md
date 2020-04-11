<p align="center">
  <img src="https://github.com/bjornbrodtkorb/altium-library/blob/master/graphics/altium_blue.png" width="400">
</p>

# Altium Library

This is a basic Altium library containing most of the files needed for creating a PCB project. This library is based on the ocean blue Altium theme, giving a fresh and minemalistic working atmosphere.

## Eample cover page

<p align="center">
  <img src="https://github.com/bjornbrodtkorb/altium-library/blob/master/graphics/blue_cover.png" width="1000">
</p>

## Example schematic

<p align="center">
  <img src="https://github.com/bjornbrodtkorb/altium-library/blob/master/graphics/blue_circuit.png" width="1000">
</p>

## Features
- Altium settings files
- Component library
- PCB rules
- Graphics
- Font
- Output files
- Templates

## How to use
Below i will describe all the different folders and how to use them.
 
### Altium settings file

This file embeds all the color settings for the schematic and PCB editor. The setting dialog is accessed from Tools->Preferences. In order to import the settings file, press the Load button in the bottom corner.

### Design rules
This part describes how to add the component library
- Copy the github folder e.g. altium-lib to your Altium Designer project folder
- Open your project in Altium Designer
- In the Projects panel, right click on the project name and select "add existing to project"
- Navigate to the component library folder inside altium-lib. Press ctrl-a to select all, and press "open"

Now you should have all the component libraries added to your project. To add the output job file, please follow the same approch.

### Rules 
This part describes how to add the design rules
- Open the PCB document where you want to apply the rules in Altium Designer
- Go to design/Rules
- Right click anywhere in the left panel (where all the rules are listed) and select "import rules"
- A second window will appear. Select all the elements in that list by pressing ctrl-a
- Navigate to altium-lib/design rules, and select the pcb_rules file
- Altium will ask if you want to "clear existing rules prior to import", select yes
- Press apply and ok, and you are good to go

### Add template for more advanced users
If you want to use the templates you should first edit the template files so that it fits you. You do this by simply opening the template files in Altium Designer. Now you can edit the files. Maybe add your own logo. When you are done with editing the template files, you have to add it to the altium template folder.
- Copy the template files xxxx_a4.SchDot and xxxx_a3.SchDot
- Navigate the the folder where altium stores templates, in most cases: "C:\Users\Public\Documents\Altium\AD19\Templates"
- Paste the files here. You should also see a bunch of other template files in the same folder
- Go to tools/preferences/system/new documents defaults
- Right beside "schematic", you can choose which file to upload
- Navigate to "C:\Users\Public\Documents\Altium\AD19\Templates" and select the xxxx_a4.SchDot that you just added

Now when you add a new schematic to you project, Altium will automaticly select your template file. To change the parameters, go to the parameters tab in the properties window. To change between a3 and a4, go to the general tab in the properties window. Here you can select which template to use in the current document.
