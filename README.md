````markdown
# CNN Challenge — Setup and Reproduction

This repository contains the code and checkpoints required to reproduce the CNN Challenge from ITCS 6169. The project was developed in a Jupyter Notebook hosted on a Linux system, so the reproduction steps below assume the use of a Linux environment.

## Required Resources

To reproduce this project, you will need:

- Python
- pip
- Jupyter Notebook
- Git
- data


The project was completed using a Jupyter Notebook running on an `ipykernel` within a Python virtual environment.

## Linux Setup

To reproduce the project, follow these instructions:
0. install all requirments and retireve data from https://drive.google.com/drive/folders/1NWC3TMsXSWN2TeoYMCjhf2N1b-WRDh-M
notebook will describe required data format
 
1. **Clone the repository from GitHub.**

2. **Navigate into the cloned repository** and create a Python virtual environment:

   ```bash
   python3 -m venv CNNvenv
````

You may use a different name for the virtual environment if desired.

3. **Verify that the virtual environment was created successfully:**

   ```bash
   ls -la
   ```

   You should see the `CNNvenv` directory. If the virtual environment was not created successfully, you may need to install the Python `venv` package for your distribution.

4. **Activate the virtual environment:**

   ```bash
   source CNNvenv/bin/activate
   ```

   You will know the environment has been activated successfully when `(CNNvenv)` appears next to your username or command prompt in the terminal.

5. **Install the required Python dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

6. **Register the virtual environment as a Jupyter kernel:**

   ```bash
   python -m ipykernel install --user --name=CNNvenv --display-name "Python (CNNvenv)"
   ```

7. **Launch the Jupyter Notebook:**

   ```bash
   jupyter notebook ITCS_6169_8169_Assignment1_2026_Starter.ipynb
   ```

8. Once Jupyter Notebook has opened, navigate to the **Kernel** menu at the top of the page and select **Change Kernel**.

9. Select:

   ```text
   Python (CNNvenv)
   ```

10. The notebook can now be executed using the installed dependencies. The provided checkpoints in the `checkpoint` folder can also be used to restore previously trained models.


Note for a shorter list of requirements the following can be used for install i fnot using linux more specifically Fedora Linux:

torch
torchvision
numpy
matplotlib
Pillow
jupyter
ipykernel
scikit-learn

```
```

