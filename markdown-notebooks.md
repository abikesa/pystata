---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

Let's set up the Stata kernel in Jupyter Notebooks. We will use the `stata_kernel` package, which provides a Jupyter kernel for Stata.

### Step-by-Step Guide to Set Up Stata Kernel in Jupyter Notebooks

#### Step 1: Install Stata Kernel

1. **Activate your virtual environment** (if not already activated):
   ```bash
   source ~/Documents/Athena/myenv/bin/activate
   ```

2. **Install the Stata kernel package**:
   ```bash
   pip install stata_kernel
   ```

#### Step 2: Configure the Stata Kernel

1. **Configure the Stata kernel**:
   ```bash
   python -m stata_kernel.install
   ```

   This command will guide you through setting up the Stata executable path.

2. **Provide the path to the Stata executable** when prompted. This will typically be something like `/Applications/Stata/StataMP.app/Contents/MacOS/stata-mp` for Stata MP, but you need to adjust it based on your specific Stata version and installation path.

#### Step 3: Verify the Installation

1. **Check the installed Jupyter kernels**:
   ```bash
   jupyter kernelspec list
   ```

   You should see an entry for `stata`.

#### Step 4: Test the Stata Kernel in Jupyter Notebook

1. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

2. **Create a New Notebook**:
   - Create a new notebook and select the Stata kernel.

3. **Run a Simple Stata Command**:
   ```stata
   display "Hello, Jupyter with Stata!"
   ```

### Summary

Here is a condensed step-by-step process:

1. **Activate your virtual environment**:
   ```bash
   source ~/Documents/Athena/myenv/bin/activate
   ```

2. **Install Stata Kernel**:
   ```bash
   pip install stata_kernel
   ```

3. **Configure the Stata Kernel**:
   ```bash
   python -m stata_kernel.install
   ```

4. **Provide the path to the Stata executable** during configuration.

5. **Verify the Kernel Installation**:
   ```bash
   jupyter kernelspec list
   ```

6. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

7. **Create a New Notebook and Select the Stata Kernel**.

8. **Run a Simple Stata Command**:
   ```stata
   display "Hello, Jupyter with Stata!"
   ```

### Additional Notes

- Ensure that Stata is installed on your MacBook Pro and that you know the exact path to the Stata executable.
- The virtual environment should be activated whenever you work with Jupyter Notebooks to ensure all kernels are available.
- Restart Jupyter Notebook and VSCode if necessary to recognize new kernels.

By following these steps, you should have a seamless setup for using the Stata kernel in Jupyter Notebooks. If you encounter any specific issues or error messages, please let me know!