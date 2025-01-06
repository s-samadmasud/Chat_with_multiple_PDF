
# README.md

## Project Setup

This document outlines the steps to set up a virtual environment and install the required dependencies for this project.

### Prerequisites

- **Operating System**: While this guide is generally applicable, specific commands may differ slightly between operating systems (Windows, macOS, Linux).
- **Python**: Ensure you have Python 3.10 or a compatible version installed on your system. You can check by running `python --version` or `python3 --version` in your terminal.

### Creating a Virtual Environment (Recommended)

A virtual environment isolates project dependencies, preventing conflicts with other projects on your system. Here's how to create one using `conda`:

1. Open a terminal or command prompt.
2. Navigate to the project directory using the `cd` command.
3. Run the following command, replacing `myvenv` with your desired virtual environment name:

   ```bash
   conda create -n myvenv python==3.10 -y
   ```

   - `conda create`: Creates a new conda environment.
   - `-n myvenv`: Names the virtual environment as `myvenv`. You can choose any name you prefer.
   - `python==3.10`: Specifies that the environment should use Python version 3.10. Adjust this if needed.
   - `-y`: Confirms the creation without prompting for confirmation.

4. Activate the virtual environment:

   ```bash
   conda activate myvenv
   ```

   (Your terminal prompt might now indicate that you're working within the activated environment.)

**Note**: If you encounter issues with `conda`, you can use `venv` from the Python standard library to create a virtual environment. Refer to Python's documentation for details.

### Installing Dependencies

The project relies on dependencies listed in a file named `requirements.txt`. Here's how to install them:

1. Ensure you have activated the virtual environment (as instructed in the previous step).
2. Run the following command in your terminal:

   ```bash
   pip install -r requirements.txt
   ```

   - `pip`: The package installer for Python.
   - `install`: Instructs pip to install packages.
   - `-r requirements.txt`: Specifies that dependencies should be installed from the `requirements.txt` file.

This will download and install all the necessary dependencies listed in the `requirements.txt` file.

### Additional Notes

- If you make changes to the `requirements.txt` file, re-run the installation command to update the dependencies in your environment.
- Deactivate the virtual environment when you're finished working on the project:

  ```bash
  conda deactivate
  ```
