# statistics-project
Scripts to recreate the 

`LA-UR-21-23115`

This README serves the SC 2021 Reproducibility Initiative goals.
This recreates figures 1-7 and table 2 in the paper.  Another
README covers the Batsim simulation results.

There are essentially two steps:
1. Setup a python virtual environment with only the packages needed by this notebook.
2. Execute the notebook at the command line, producing all figures in PNG and PDF form.

Note that the notebook (.ipynb) can be inspected to understand
the functions.  A snapshot of this is also provided in HTML for
easier viewing.

## STEP 1 - ENVIRONMENT SETUP - RUN THESE COMMANDS:
```
python3 -m venv sc-2021-ccu-lanl-statistics
source ./sc-2021-ccu-lanl-statistics/bin/activate
pip install --upgrade pip
pip install ipykernel
source ./sc-2021-ccu-lanl-statistics/bin/activate
ipython kernel install --sys-prefix --name=sc-2021-ccu-lanl-statistics
pip install jupyter scipy matplotlib pandas seaborn
```

## STEP 2 - EXECUTE NOTEBOOK - GENERATE PLOTS - RUN THIS COMMAND:
```
ipython --TerminalIPythonApp.file_to_run=./sc-2021-ccu-lanl-statistics_paper_functions.ipynb
```
