# CINECA/IFAB Practical Quantum Computing School 2021
Pasqal's tutorials for the CINECA/IFAB Practical Quantum Computing School 2021.

## Installation

### Step 0: Clone and enter the repository

We clone the repository with the tutorials (do this inside the folder you desire to place it) and go inside this folder:

```
git clone https://github.com/pasqal-io/tutorial-IEEE-quantum-2024-09-15.git
cd tutorial-IEEE-quantum-2024-09-15
```

### Step 1: Create a clean virtual environment


We create a virtual environment called `.ieee-venv`, using Python's `venv` (recommended):

```
python -m venv .ieee-venv
```

You might have to replace `python` by `python2` or `python3` depending on your Python installation.

### Step 2: Activate the environment

On Windows

```
# In cmd.exe
.ieee-venv\Scripts\activate.bat
# In PowerShell
.ieee-venv\Scripts\Activate.ps1
```
On Linux and MacOS:

```
source .ieee-venv/bin/activate
```

### Step 3: Install packages with `pip`

Install the latest release of `pulser` and other required packages for the jupyter notebooks by running:

```
pip install -r requirements.txt
```

### Step 4: Install Jupyter Notebook

We'll need Jupyter Notebook to run the tutorials, so we run:

```
pip install notebook
```

#### Step 4.1: Adding the new environment to Jupyter notebook

If you created a new virtual environment, you'll need to add it as a new kernel in Jupyter notebook. To do so, we use `ipykernel`:

```
python -m ipykernel install --user --name=.ieee-venv
```
We now have a new kernel called `.ieee-venv` inside of our notebooks.


### Step 5: Executing the tutorials

Finally, we launch Jupyter notebook:

```
jupyter notebook
```

After opening a notebook, make sure the kernel is set to `.ieee-venv`.