# Things to add to the editor (aka TODO list)

1. Bug with resort and ABCMolecule
2. Add create_centroid from selection?
3. Add generate supercell menu
4. Fix/Finish new molecule lister object and singular update method
    - Make sure it only updates what it needs. Unsure what it is doing rn
5. Think about how to make it more sciency and more like ase
6. Add more settings variables about matplotlib defaults and radius
7. Maybe create menu that edits matplotvisualize data and saves it as a json format?
8. Add coords function with ABCMolecule is not working correctly and not placing molecule in center of unit cell.
9. Create a google form for a bug tracker and bug tracker page.


# From word document

EDITOR NEW THINGS
•	Parrellization
•	Updates when you change settings
•	New environment variable logic is updated
•	One codebase for differences in windows and bash environments.

EDITOR TODO
•	Need to add vasp selective coords again
•	Certain rotate and other functions don’t work atm
•	Unit tests or check to make sure everything works
•	Sort methods and another popup menus.
•	Fix certain conversions.



Whats Left:

[The Chemistry Development Kit (CDK):  An Open-Source Java Library for Chemo- and Bioinformatics | Journal of Chemical Information and Modeling (acs.org)](https://pubs.acs.org/doi/10.1021/ci025584y)

[Avogadro: an advanced semantic chemical editor, visualization, and analysis platform | Journal of Cheminformatics | Full Text (biomedcentral.com)](https://jcheminf.biomedcentral.com/articles/10.1186/1758-2946-4-17)

-CHANGE T and F for freeze and unfreeze
-ADD freeze all but selected atom, unfreeze all but selected atoms
-Fix clause if selected then …
    -DONEadd common oxidaton states on the charge editor- add charge editor possible oxidation states
- DONEadd popup menu for unit cell surfaces method that would change elim, axis and based on chosen sides that I would code in and have a dictionary or just a bunch of if statements.
- DONEadd unit cell deciding logic
    - DONE fix charge atom frame width, needs set value
    -NOT NECCESARY add .vasp to cartesian conversion in scroll text
    - change microsoft copy commands key bindings
    - change settings menus
    -.sh
    -.jav
    -.dmg for
   -NOT NECESSARYsome bugs with adding atom and select atoms
   -DONE to text box needs to have .xyz and .vasp

    -DONE add step size setting for dialog buttons
-DONEarrow popup label colors	
    - DONE have textbox pop up if needed, so you can copy and paste to the terminal
    - DONE add file name to title of editor window
    -DONE change the no atom loaded text on scroll text to something more professional
    - NOT NECESSARY ATM maybe add bool logic to init functions so if return False then something went wrong in the __init__()
    - when I distribute, i will just email the .exe file, settings.json, and README.md, and LICENSE file (might load to git hub)

DONE If curr_atom is emptymolecule, be able to add molecule to nothing
    - DONE choose font for info text that is same width
    -DONE make dialog box slightly less and move info box over


For config file
    - NOT ADDEDdefault bond color,
    - NOT ADDEDdefault unit cell color,
    - NOT ADDEDdefault bond length,
    - DONEif there’s an origin arrow or not**(add to settings)
    - DONEadd logic for if fields exist in config file
    - DONEadd orthographic or prospective for matplotlib setting




BUGS:
    -On absorbent adder, the most positive and negative element doesnt work
    -add if statement if the dialog is zero or the curr atom is Empty
    -add log statements to before every return statement in the functions.
    -add log statements to end of every function class saying completed
    -maybe simplify the function that has 3 returns and a tuple return
    -when you execute command to move, update matplotlib and scroll list coordinates but keep scroll list selected.
    -possibly have button to automatically seperate adsorption model if selected and save into 3 seperate files.
    -another cool functionality would be to be able to switch units on scroll list between pos and cartesian when it is a unit cell.
    - if I want to automate adding adsorbate, I could find center of gravity, I could move to center of unit cell x,y and then z move above highest surface model
    -also when you import a molecule, scroll list will automatically select the new molecule.   
    -DONE If xyz adsorbent file, need to convert to ABCMolecule coords
    -DONE If no adsorbent file is chosen, then have a popup that lists the loaded information and you can
        choose which atoms are the adsorbent.
    -DONE Can acheive the first two by creating an object/class that stores/converts adsorbent to type of
        surface and then you can modify the adsorbent in relation to the surface.
    -DONE Also has an update button/updates the Matplotlib visualizer feed base off of changes from
        the user.
    -DONE Save button to save and writes the current configuration to the textbox in the format of the surface file.
    -NOT_WANTED Close button and then popup that asks do you want to save file with filesave dialog popup
    -MAYBE NEEDED add popup menu when converting xyz to Vasp
    -NOT NEEDED prob not. use typechecker strict for bestcodepractices
    - FOR NEB:
        - have a view where you load a beginning and a final image and then click through each atom 
        to see if it is the same one or different one.
    -KINDA DONE(Only adding 2 vasp files if they have equal unitcelll)
        If Vasp adsorbent file, need to create a function that will take the ABCMolecule object and convert
        it to the different (larger) unitcell with same lattice matrix as the surface
    - make it resizable. Would need a key binding for resizability.
    -NEXT TO DO:::: MAKE SETTINGS SCREEN so that I can start to change settings during the code running.
        - will make sense on where to import new absorbent, color themes, maybe how atoms are rotated,
         rule on moving molecules in vasp greater than 1 or negative, 
    -still need to update on matplot when you check the button on scroll list
    -*create clipboard window. Will need while loop until window is closed to load into editor.
        - popup will have textbox and dropdown with options of full file, vasp coords or xyz coords.
        - have submit button where it will close window and return as Molecule type.
    - DONE When Zero Text, error appears. Might need to make NoneTypeText so no error
    - Theres a bug with validating xdatcar and xyz animation files.
    - Matplotlib visualizer Vasp unit cell
    - The first undo of the file deletes the file and doesn't remember the change (gotta be something with TKINTER)
    - DONE menubar color changes when settings dialog opens
    - DONE with listing in MoleculeLister
    - popup windows are behind parent windows...
    - DONE when import a new file, scroll list needs to be updated also
    - rotate function in .xyz works. Rotate function in .vasp does not really work
    -with comparison of molecules, need to add __eq__ or __str__ or __repr__ in all molecule classes
        in order to compare and know if one has changed or not. right now im not sure what is happening when two 
        molecules are being compared.


 
python -m PyInstaller main.py --onefile --windowed
Dependencies (not from standard library):
    - Matplotlib
    - customtkinter
    - tkinter
    - numpy
    - pyautogui
    - maybe periodictable



 
