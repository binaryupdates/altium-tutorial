# ALTIUM Tutorial from YouTube

Download Altium Designer: https://www.altium.com/yt/binaryupdates

Lets design PCB using Altium Designer from start to finish.

# SCHEMATIC Drawing

File--> New --> Project --> PCB Project (Add Schematic and PCB Document)

Open Shcematic file and set Grid to 100 mil while placing components on schematic document. Place components and draw schematic circuit diagram

Annotate Schematic file, Tools--> Annotation -->Annotate Shcematic --> Update changes --> Accept changes

Compile Project, just rught click on project & compile to check for any error (ERC). Also check in message panel

Go to Project --> Project Options --> Class Generation --> Uncheck "generate rooms" & "component class"

Generate PCB Board File, Design --> Update PCB Document --> Execute Changes

Board Properties --> unit (mm) --> Change Grid Manager --> Step X "5mm"

Customize the size and shape, Go to View --> Board Planning Mode --> Now go to Design menu --> Redefine Board Shape --> 60x23mm --> View 2D Layout Mode --> Place Components

Set Origin, Go to Edit --> Origin --> Set --> Select Corner cursor

Set tthe grid, Press "G" on keyboard & select 0.5mm, View --> Fit Board

Design --> Layer Stack Manager --> Dielectric "1.6 mm" (set layer stack) --> Ok

Design --> Rules --> Clearence under Design Rules, Minimum Clearence 0.3mm & Width, Preferred Width 0.5, Min: 0.3 and Max: 1mm, Routing Via Style --> Routing Via Min: 0.6 (Via Diameter) & Via Hole Size 0.3 --> Ok

To Switched OFF Auto Pane--> Gear Icon on Top right corner --> PCB Editor --> General --> Uncheck "Unable Autopane"

Arrange Components and palcements properly on PCB Document and select "Interactive Routing" on Active bar

# ROUTING PROCEDURE

Make sure TOP Layer is selected while drawing routing track on PCB (Via can be tented in option of solder mask expansion)

Select BOTTOM layer, Place --> Polygon Pour --> In Properties select Net to GND --> draw copper pour/polygon pour

Check if any Error (DRC), Tools --> Design Rule Check --> Run Design Rule Check Button

Select PCB Board file --> Open PCB Rules and Violation view --> in popup select all rules

Design --> Rules --> Silk to Solder Mask Clearence under Manufacturing --> 0.1 mm --> ok --> Re-Run Rule Check, Tools --> DRC --. Run DRC --> Check

# GENERATE GERBER, NC DRILL FILES and Pick and Place File








![alt text](https://github.com/binaryupdates/altium-tutorial/blob/main/schematic.png)
