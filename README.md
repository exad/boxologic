Boxologic
=========

A set of C programs that calculate the best fit for boxes on a pallet, and visualize the result.

Future Plans
------------
This project uses a fairly old codebase as a launching-off point.  The plan is to modernize it a bit, and then add functionality by allowing the user to specify more than one container to be packed, as well as perhaps library-ifying the main code so that you can wrap your own code around it more easily.  Keep watching this space for details as they emerge.

Caveat Emptor
-------------
### UPDATE
Users can now view output visudat files in their browser by vieweing index.html after running the relevant boxologic command.

This codebase is currently undergoing fairly sweeping changes. While we'll try our very best to always have compile-ready, working code here, no guarantees of any sort are made. Currently the visualizer only runs using the windows-only code & binary supplied by the [project this one was forked from](https://github.com/wknechtel/3d-bin-pack). The visualizer in this fork is slated to be rewritten using OpenGL, and will be cross-platform.

Usage
-----
    USAGE:
      boxologic <option>

    OPTIONS:
      [ -f|--inputfile ] <boxlist text file>   : Perform bin packing analysis
      [ -v|--version ]                         : Print software version
      [ -h|--help ]                            : Print the help screen

Boxlist Format
--------------
The first line of the boxlist file defines the X, Y, and Z dimensions of the pallet in which all the boxes are to be packed. Each successive line begins with a box number, then has the x, y, and z dimensions of the box, and finally how many of this box are to be packed onto the pallet.  A sample boxlist is [provided in the doc directory](https://github.com/exad/boxologic/tree/master/doc).
