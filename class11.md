# What is Jupyter Lab

Jupyter Lab is a Web-based interactive development environment for notebooks, code, and data. You can arrange multiple documents and activities side by side using tabs and splitters. 

- Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook, for example.

- Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

- Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

- Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.

## Numpy Tutorial

Numpy is a data analysis package. Creating a Numpy Array

1. Import the numpy package.
2. Pass the list of lists wines into the array function, which converts it into a NumPy array.
3. Exclude the header row with list slicing.
4. Specify the keyword argument dtype to make sure each element is converted to a float. 

`import csv
with open("winequality-red.csv", 'r') as f:
    wines = list(csv.reader(f, delimiter=";"))
import numpy as np
wines = np.array(wines[1:], dtype=np.float)`

- Numpy to read files: 

1. Use the genfromtxt function to read in the winequality-red.csv file.
2. Specify the keyword argument delimiter=";" so that the fields are parsed properly.
3. Specify the keyword argument skip_header=1 so that the header row is skipped.