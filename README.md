SCAD snippets - gedit
=====================

This repository holds a [gedit](http://www.gedit.org) snippets file for `.scad` 
files as used and defined by [OpenSCAD](http://www.openscad.org). While I really 
like the main approach of OpenSCAD to programmatically create 3D models, I was 
not happy with the source code editor provided in the OpenSCAD application. 
Therefore I decided to program the models inside my favorite text editor and use 
OpenSCAD "only" for rendering.

Install
-------

In order to use these snippets, two prequisites need to be fulfilled:

* The mime type definition for `.scad` files to be registered. I did this by
  installing 
  [scad-highlight-gtk](https://github.com/brunogirin/scad-highlight-gtk). This
  also provides nice syntax highlighting.
* The *Snippets plugin* (should be provided be the gedit package by default)
  needs to be activated. This can be done through *Edit* -> *Preferences* -> 
  *Plugins*.

The file `scad.xml` needs to be copied (or better symlinked) usually to 

`~/.config/gedit/snippets` (for only this user)

or

`/usr/share/gedit/plugins/snippets` (for system-wide installation)

Note the the directories might depend on your specific installation.

Contact
-------

Author: Christian Luginbühl <dinkel@pimprecords.com>
Home:   <http://github.com/dinkel/gedit-scad-snippets>

License
-------

See the LICENSE file.

Comments / Bugs
---------------

Suggestions for improvements or bug reports are always welcome! 

* By far not all commands provided by OpenSCAD have a corresponding snippet, but
  only the ones I use most.
* The "tab trigger"s are currently as short as possible (1-2 characters). Time 
  will tell whether this is a good idea or other approches (like 3 characters
  for all snippets) will feel better to me.
* I designed all snippets that provide a "block" to actually have one, although 
  it might be possible to omit them if only one command follows.
* If either a scalar value or a vector is accepted as an input parameter to a
  command, the latter is used inside the snippets.
* If named parameters could be omitted, the actually have been omitted.

**That said: Don't count on anything (be it the triggers or the replacements)
being stable right now!**

It might be a goot idea to fork this project and customize the snippets file to 
your liking.
