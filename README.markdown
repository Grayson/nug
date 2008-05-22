# About

`nug` generates ObjC header files from Nu files.  This is handy when integrating Nu and Objective-C in the same project.  This is based on a [request](http://groups.google.com/group/programming-nu/browse_thread/thread/69264ebe1ced5f1c/6606e0556dca972d#6606e0556dca972d) in the Nu mailing list.

# Compiling

Open the Terminal and navigate to the `nug` directory using the command line.  Then do the following:

1. `nuke`
2. `nuke install`
3. `nuke clobber`

The above should compile `nug`, install it into /usr/local/bin/, and then delete the generated files.  If you'd prefer to compile `nug` by hand, you can do the following:

1. `nubake` the nu file using: `nubake nug.nu -s`
2. Compile into a program using: `gcc nug.m -o nug -framework Cocoa -framework Nu`
3. Install the compiled `nug` where you normally put executables

# Usage

Navigate to a folder with a "nu" folder (but don't go into the "nu" folder) using the Terminal.  Run `nug` in the Terminal.  `nug` will create a "nug" folder (if one doesn't already exist) and create header files based on information found in the nu folder.

# Author

[Grayson Hansard](mailto:info@fromconcentratesoftware.com)  
[From Concentrate Software](http://www.fromconcentratesoftware.com/)