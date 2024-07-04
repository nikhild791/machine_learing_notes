# General Instruction for creating a project

### conda venv
*create a virtual environment with the help of conda so that all your required files should be placed at one place
```conda create -p venv python==3.10```
```conda activate venv/```
```conda deactivate```

### requirements.txt
*all the packages used in this project will be listed here
```pip install -r requirements.txt```

### Jupyter notebook in vscode
* we need ipykernel to run ipynb
```pip install ipykernel```

## Environment Management

### Creating an environment
- Conda: `conda create -n or -p myenv python=3.12`
- Python venv: `python -m venv myenv`

### Activating an environment
- Conda: `conda activate myenv`
- Python venv: 
  - Unix-like systems: `source myenv/bin/activate`
  - Windows: `myenv\Scripts\activate`

### Deactivating an environment
- Conda: `conda deactivate`
- Python venv: `deactivate`

## Package Management

### Listing installed packages
- Conda: `conda list`
- Python venv: `pip list`

### Exporting installed packages to a file
- Conda: `conda list --export > environment.yml`
- Python venv: `pip freeze > requirements.txt`

### Creating an environment from a file
- Conda: `conda env create -f environment.yml`
- Python venv: `pip install -r requirements.txt` (after creating and activating a virtual environment)
