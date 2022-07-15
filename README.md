# Growth_analysis
Parse and analyze 96-well plate raw data into growth curves.


Installation requirements
Google drive desktop - https://www.google.com/drive/download/
Python 3.10 and up - https://www.python.org/downloads/
for mac follow these instructions to install python 3: https://docs.python-guide.org/starting/install3/osx/
VScode (https://code.visualstudio.com/download) with the following extensions:
    python
    jupyter
requirements.txt -this installs all the required python libraries in the local environment
PC: use: $py -m pip install -r requirements.txt --user
Mac: use: $ pip3 install -r requirements.txt --user
                


Running the code -= press the play all button and follow the analysis steps. 
There are three steps that require user input:
    1. Loading the result file - a message will pop up asking for the result file followed by a file open dialog box to select the file.
                                The file dialog box is already tuned to the preset Google drive folder.
    2. Loading the plate layout file- a message will pop up asking for the plat layout file followed by a file open dialog box to select the file.
                                      The file dialog box is already tuned to the preset Google drive folder.
    3. Picking columns to remove from the analysis- when the cell after the title 'Select columns to remove from the table' is run, a white interactive table will appear
                                                    showing all the columns in the data table. Each column can be deleted by pressing the trash can icon by the column name.
                                                    After column delteing is done press the button beneath the 'save' button beneath the table. A message saying 'Data processed, continue running notebook' should appear, indicating the new data table is ready for downstream analysis. 

                                                    ## !!! after executing this cell - please continue to run (press the play button) the following cells manually - they will not run automatically in this version 

Note- After executing step 3 in the above list please continue to run the next cells manually.

All the result files will be stored in the '/results_experiment_filename' folder.

All the graphics are saved as svg for easy editing in the '/results_experiment_filename/graphics/' folder.

Each file created while running this code will include the experiment name:

    Example - 'results_experiment_filename/graphics/growth_curves_experiment_filename.svg