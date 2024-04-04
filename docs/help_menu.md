===============================================

Hello cool kid Quantum Chemist!!

This is an atom editor for creating molecular files for .xyz programs and VASP.

Developed by Jeremy Schroeder. Version 1.0.2 March-24-2024

===============================================

Different Menus and Functions:

Import:

  - From File (New)

    • Loads file into the editor.
  
  - From File (Append)
  
    • Adds new selected file to currently loaded file meant for adding absorbent ontop of a surface or building  stacks.
  
  - From Textbox
  
    • Textbox opens where you can paste atomic coordinates and press Load Text button to add absorbent or new file.
  
    • Insert Text Button will append the coordinate as they are written to the bottom of the current molecule.

Orient:

  - Any Face [a,a*,b,b*,c,c*]
    
    • Changes orientation of the visulizer to be that face's orientation.

Execute:

   - Move

    • Moves selected coords distance defined in the dialog.

   - Rotate [X or Y or Z]

    • Rotates selected coords in degrees. Settings for how it rotates is in settings menu.

   - Delete

    • Deletes selected coords.

Add Atoms:

    • Opens a menu that will add atom determined above or below selected coords.

    • Useful in hydrating a surface.

Charge Menu:

    • Opens a menu where you can change the charge of each species that will be used in the Total Charge calculation.

    • Common Oxidation States Button - Shows what the common oxidation states for the species you have are.

    • Save Button - Saves the current input and updates the Total Charge in the bottom right Info Panel.

Resort Menu:

    • Change the order of the atoms in the molecule.

Save:

    • Opens a menu that has multiple options on how to save the currently loaded molecule.

Update:

   - Update Scroll List

    • The scroll list should be correct at all times.

   - Update Matplot

    • Needed to update the selected atoms color to visually see what you have selected.

   - Update Info

    • Updates the bottom right Info panel.

   - Undo Operation

   - Redo Operation

   - Clear Editor

    • Deletes current state of editor.

Settings:

   - Rotation Origin

    • Centroid: rotate the selected atoms around their centroid/center of mass.

    • Origin: rotate the selected atoms around the axis at origin location (0,0,0).

   - VASP Coord Limit

    • '0<x<1': If vasp coord reaches max positional coord, error will occur.

    • 'Not Restricted': No limit on vasp coord range.

   - Distance Option

    • Type in the distance showing setting you want. An example of input is (1-C-F),(2-N-H)

     First number is how many distances shown you want.

     Second and third is what elements you want drawn.

     You must use (). You must use '-' to divide inputs as shown. Must use ',' to divide different inputs if you want more than 1.

   - Perspective

    • Changes projection perspective in atom visualizer.

   - Origin Arrow

    • If checked, the origin x,y,z axis arrow will appear. If unchecked no arrow will appear.

   - Move Step

    • Type the amount you want to step by when the coord + - buttons are pressed in the Parameters dialog box.

   - Perspective

    • Type the amount you want to step by when the angle + - buttons are pressed in the Parameters dialog box.

   - Atom Labels

    • Choose what type of atom labels you want if you choose.

Key Bindings:

    Ctrl-o : Import New
    Alt-o : Import Absorbent
    Ctrl-a : Select All
    Ctrl-t : Toggle All
    Ctrl-n : Select None
    Ctrl-z : Undo
    Ctrl-b : Redo
    Alt-a : Add Atom
    Ctrl-e : MoveFunction
    Ctrl-d : DeleteFunction
    Alt-x : ClearFunction
    Ctrl-1 : Rotate x axis
    Ctrl-2 : Rotate y axis
    Ctrl-3 : Rotate z axis
    Ctrl-s : Save Menu
    Ctrl-r : Resort Menu
    Ctrl-q : Charge Menu
    Ctrl-w : Settings Menu

Any feedback or bugs please email jerschro@ttu.edu or jeremynschroeder@gmail.com

Thank you for using this piece of software and I wish good luck to the DFT Gods for you...
