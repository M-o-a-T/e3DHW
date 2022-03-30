# e3DHW-make-DIY-electronics-hardware-like-a-professional
 
The evolution of the electronics from the single components to the macro-sets (boards and shields)
was positive, allowing the rapid prototyping of complex projects until a few years ago
unimaginable, thus bringing new audiences of enthusiasts to electronics.

I want to present some ideas to move from an electronic 'prototype' to a more stable and usable
realization, in a simple, quick and economical way.
With the use of a 3D printer and a series of OpenSCAD (https://www.openscad.org/) parametric libraries ready to use.

The use of the 3D printer allows to obtain tailor-made structures without the need of mechanical
workshop machines for cutting, bending or drilling. Also many accessories (ADDONs) such as
terminals, connectors etc. can be inserted into the 3D project by simplifying assembly and wiring.

![Watering Sonoff](images/sonoff400.jpg  "Sonoff watering timer") 

- For the full story, read the e3DHW_HOWTO_en.pdf file (versione italiana e3DHW_HOWTO_it.pdf)
- OpenScad libraries, last stable version, in dir OpenScadLibraries :)
- File help for all libraries: e3DHWref.1.2.chm.
- Also here: https://www.thingiverse.com/thing:2860353

#### Working version: 1.3

 - Added Power Management System (see 'power PMS/e3dhw-pms-intro_en.pdf')
 - Added 'power PMS/e3DHW_addon_batteries.scad'
 - Added 'base/e3DHW_array_utils.scad'
 - File help for working version: e3DHWref.1.3.chm.

# Working version 1.3

All OpenScad libraries are designed to be very easy to use in your projects:

- any library is composed of modules to make containers and boards or ADDON to add things to a main board.
- all modules are fully parameterized, but for the user convenience, many parameters have "reasonable" default values which can
  be ok almost everywhere.
- all parameter values are checked, with specific error messages
- the use of Doxigen gives us the help e3DHWref.1.X.chm, a complete e3DHW library reference, indispensable for the e3DHW users.
- any library as a xxxx_examples.scad file, to show the use. All examples are also with the STL files, to preview the results.

How to use "e3DHW_xxxxxx.scad" libraries? 
- In your OpenSCAD file add on top "include <e3DHW_xxxxxxxxx.x.x.scad>;" for all files you need for your project (see 
documentation and examples files).
- put all required libraries in the same directory as your project.
- create also the dir ./contrib, and copy there all the required files.
- Then you can use all public modules as you like.

How to use e3DHWref.1.X.chm?
- Download it and use a help viewer (MS help viewer, Sumatra PDF, etc) 
- If you see the index, but not the content, it has been because windows security has "blocked" the chm file. To see it try the following:
  - From windows explorer, Right click the dowloated .chm file and select properties.
  - On the General tab, if you see an Unblock button, click it.
  - Close the dialog and open the .chm file.
