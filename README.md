# bambu-3mf-project-renamer
Takes a given .3mf file, iterates through each plate name, creates 1 file per plate with project Title and Description matching the name of the plate. This lets you have the right project names display on the printer. Helpful if you re-use project files and can't get the name changed. Generated via Grok 3 and tested by me. 

This script does not remove any plates or alter your original .3mf file. It simply clones the original .3mf file, one copy for each plate in the project, and sets the new file name, project description and title to the value of the plate name.  It will skip any Untitled plates. 

## Usage
1. Name your .3mf plates to be descriptive.
2. ./gen_3mf_plates.py "My Project With lots of Plates.3mf"
3. .... Profit

<code>$ ls 
My Project With lots of Plates - Plate 1 full of crap.3mf
My Project With lots of Plates - another plate.3mf
My Project With lots of Plates - hopefully you get it.3mf
My Project With lots of Plates - Now print it and you will see this name on the printer.3mf
</code>

