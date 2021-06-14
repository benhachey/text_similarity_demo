# Text similarity demo

Use scikit-learn to vectorize and calculate similarity between values in an Excel column.


## Preliminaries

Create a Python virtual environment and install VS Code using the following instructions.


### Install Anaconda

Follow instructions at the following link to install Miniconda for Python version 3.8:

https://conda.io/projects/conda/en/latest/user-guide/install/index.html

Anaconda is a tool for scientific computing using Python. We'll use the Miniconda version to create an isolated virtual environment with the libraries we need for analysis. This avoids altering OS Python configurations if present.


### Create virtual environment

Run the following command to create a virtual environment called `ts38`:

```conda create --name ts38 python=3.8```

Activate the `ts38` virtual environment:

```conda activate ts38```

Install packages:

```conda install scikit-learn```

This will install a number of scientific computing packages as well as `sklearn`, which includes modules for working with text.


### Install VS Code

Follow instructions at the following link to install Visual Studio Code:

https://code.visualstudio.com/download

VS Code is popular source-code editor from Microsoft. Once VS Code is installed, opent it. The remaining work will be completed using VS Code.


### Install Python extensions

VS Code should display a dialog asking whether you want to install the Python extension for Visual Studio Code. Use the dialog to install.

If another dialog appears asking whether to restart VS Code to activate Python, choose yes.


## Run demonstration

Open VS Code if it isn't already then use the instructions below to run the demonstration.


### Select Python interpreter

Press `command+shift+P` to open the command pallette. Type `Python: Select Interpreter` and press enter. Use the dialog to choose the `ts38` conda environment.

Check that the correct Python intepreter is being used. It should be displayed in the lower left of the VS Code window. It should include the name of the conda environment you created, eg, `ts38`.


### Download the demo

Use the following link to download the demo to your project folder or working directory:

https://raw.githubusercontent.com/benhachey/text_similarity_demo/main/text_similarity_demo.ipynb


### Open the demo notebook

Switch back to your VS Code window. Use the "Open" dialog under the "File" menu to open the IPYNB file you exported in the previous step.


### Export the data

Open the spreadsheet in Excel. Activate the worksheet that contains the text data. Use the "Save As" dialog under the "File" menu in Excel to export the worksheet as a comma-separated values (CSV) file. Move this file to your folder or working directory.


### Define input/output

Update the following variables to set the path to the input CSV and the columns to be processed:

```
CSV_PATH = pathlib.Path("list_of_provisions.csv")
ID_COLUMN_NAME = "\ufeffSECTION no"
TEXT_COLUMN_NAME = "TEXT"
```

Update the following variable to set the path to the output CSV:

```
OUT_PATH = pathlib.Path("similarities.csv")
```

### Run notebook cells

Press the play button on each cell in the notebook to run individually. Or press the run all cells button at the top of the VS Code window.
