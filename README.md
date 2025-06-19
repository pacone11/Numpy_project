Progetto - Numpy e librerie Python  

Step 1:  
Basic Organizer Script
A Python script iterates alphabetically through the files inside the files folder.  
Depending on the file type (audio, document, image), it moves each file into the appropriate subfolder.
If the subfolder doesn’t exist, the script automatically creates it.

During the process, the script prints file information: name, type, and size (in bytes).  
Each time a file is moved, a recap.csv file is updated with the same information.

Step 2:  
A standalone Python script called addfile.py (located in the same directory as the notebook) was developed with a command-line interface (CLI).

Its purpose is to move a single file from the files folder into its appropriate subfolder and update recap.csv.

The CLI requires one argument: the exact file name (with extension) to move.
If the file does not exist, the script notifies the user.


Step 3:  
A script scans the img subfolder and generates a summary table using the tabulate library.

For each image, the table includes:

- File name
- Image height (in pixels)
- Image width (in pixels)
- If grayscale: a single grayscale column with the average color value
- If colored: separate columns for average values of RGB (or RGBA) channels
