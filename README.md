# Getting Started with Python programming language

## Environment

- **Ubuntu (Linux)** - Operating system, version 22.04 or newer.
- **VS Code** - Code editor.
- **Bash** - Default Linux shell.
- **Python** - Programming language used for machine learning.
- **Miniconda** - Package and environment manager for Python.

## Initialize the environment

Use **Miniconda** to manage **Python** packages and environments. Follow the steps below:

1. Download **Miniconda**:

   ```bash
   cd ~
   wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
   bash Miniconda3-latest-Linux-x86_64.sh
   ```

   _Choose `yes` for all prompts._

   If **Miniconda** is already installed, you can remove the downloaded installer file:

   ```bash
   rm Miniconda3-latest-Linux-x86_64.sh
   ```

2. Reload the shell and verify the installation:

   ```bash
   exec bash
   conda --version
   ```

3. Stay in the project directory and create a new environment:

   ```bash
   conda create -n ml-env python=3.11
   conda activate ml-env
   python --version
   ```

4. Install the required libraries:

   ```bash
   conda install jupyter numpy pandas matplotlib scikit-learn

   # List installed libraries
   pip list
   ```

5. List existing **conda** environments:

   ```bash
   conda env list
   ```

6. Exit and delete the environment:

   To exit the current environment:

   ```bash
   conda deactivate
   ```

   To delete an existing environment:

   ```bash
   conda env remove --name ml-env
   ```

> [!IMPORTANT]
> `ml-env` is the environment I use for learning machine learning, so it is not fixed. However, environment names should be meaningful.
