[:fontawesome-solid-house:](../index.md) :fontawesome-solid-angle-right: [Guides](index.md) :fontawesome-solid-angle-right: **Import Append**
# How to add an absorbent molecule to a surface


1. First load the surface (either slab or cluster model) into the editor. This example is an  alumina slab model.

    ![Slab](../images/import_append/import_append_1.jpg)

2. Then open Import - From File (Append). Options for each import absorbent setting:

    ![Absorbent Menu](../images/import_append/import_append_2.jpg)


    ![Annotated Absorbent Menu](../images/import_append/import_append_3.jpg)

    2. Dropdown options are 'Above' and 'Below'. This box designates which direction the new molecule is added in.

    2. Dropdown options are 'x' 'y' or 'z'. This box designates which axis you want to place the new molecule in.

    2. Dialog box is a float of how much distance you want between the reference locations (Boxes 4 and 5) of the surface and new molecule.

    2. Dropdown options select where you want the distance to be measured from the loaded surface. Direction is the axis chosen in dropdown box 2.
        * Options include:
        * Top surface atom (If z axis is chosen for example, the top surface atom is the highest atom of the surface in the chosen axis.)
        * Bottom surface atom
        * Origin
        * Centroid
        * (0.5,0.5,0.5)
        * Most positive Sp (If Most positive H is chosen for example, the most positive H atom is the highest H atom of the surface in the chosen axis.)
        * Most negative Sp

    2. Dropdown options select where you want the distance to be measured from the new molecule. Direction is the axis chosen in dropdown box 2.
        * Options include:
        * Top (axis) atom (If z axis is chosen for example, the top atom is the highest atom of the new molecule in the chosen axis.)
        * Bottom (axis) atom
        * Centroid of new molecule.

    2. Add Molecule button that saves current settings and opens up file dialog to select the new molecule file.

3. Once you have chosen settings you want. Press Add Molecule Button (Annotated as Button 6) and chose the new molecule from the file dialog.

4. New Molecule is added exactly where you designated it to be and is selected automatically. A H2O molecule was added precisely in the middle of the cluster model on the positive z face.

    ![Absorbent Added](../images/import_append/import_append_4.jpg)