# AMISR User Manual

This is a short guide for scientific end users of AMISR data.  It will give a broad overview of how to access, plot, and interpret the data.  This guide will attempt to focus on the most important points for most basic scientific analysis rather than a detailed descriptions of all nuances in these datasets.

## How to Use this Guide
This guide is a mix of background information and code examples demonstrating how to do common plotting and analysis tasks.  Although it can be read through in full, you may find it more useful to use the table of contents in the left sidebar to skip to the section most relevant to what you are trying to do.  Cross reference links have been embedded in the content to make it possible to jump easily to more information about particular topics.

Users should adopt a "copy-paste-modify" philosophy with the examples shown in this guide.  For the most part, these examples are intentionally designed to be extremely simple to illustrate the basic steps required to access and plot AMISR data.  Users are encouraged to copy/paste any examples they find helpful into their own code, but will likely have to customize it using normal python and plotting functions to suit their needs.

### Run in Binder

[Binder](https://mybinder.org) is a online service that lets you run jupyter notebooks in the cloud.  Click the button below to run this tutorial in Binder.  Note that it may take several minutes to load.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/amisr/amisr_user_manual/main)

```{warning}
Binder instances are not perminent and have limited computational resources.  This is useful for quickly exploring the AMISR data and learning the basics of working with it, but not for any significant analysis.  If you would like to save your work or perform more subtansive analyses, consider the option to [run locally](local).
```

(local)=
### Run Locally

The tutorial notebooks can be downloaded and run locally.

1. **Install Python**

Python can be downloaded and installed from [python.org](https://www.python.org) for a variety of operating systems.  From the "Downloads" tab select your operating system and download and run the installer.  Alternatively you can install a more comprehensive package manager such as [Anaconda](https://www.anaconda.com/docs/main) or [Miniconda](https://www.anaconda.com/docs/getting-started/miniconda/main).  Any python installation should be fine, so if you have a functional one already you can skip this step.  A recent version of python (at least 3.10) is recommended, but the tutorial may still function with earlier versions.

2. **Clone User Manual Repository**

Open a command prompt and navigate to where on you machine you would like the user manual notebooks saved.  Run the following command to clone the GitHub repo and enter the repository.
```
git clone https://github.com/amisr/amisr_user_manual.git
cd amisr_user_manual
```

3. **Create a Virtual Environment**

A virtual environment will allow you to set up and install the prerequisites required to run the user manual without interfering with other python packages you have installed and use for other work.  This is recommended, but not strictly required.  If you installed python through Anaconda or Miniconda, use the `conda` option, otherwise use `venv`.
`````{tab-set}
````{tab-item} venv
```
python -m venv /path/to/venvs/amisr_user_manual
source /path/to/venvs/amisr_user_manual/bin/activate
```
````

````{tab-item} conda
```
conda create --name amisr_user_manual
conda activate amisr_user_manual
```
````
`````

4. **Install Required Packages**

A requirements is included in the root of the repository.  Use these to install all packages used in the tutorials.
```
pip install -r requirements.txt
```

5. **Start Jupyter Lab**

Run this command from a command prompt to start jupyter lab and open the user manual in your browser.
```
jupyter lab
```
Some IDEs may let you interact with the jupyer notebooks directly.


## Issues and Questions
Any bugs or typos found in this book can be reported through the GitHub button at the top of each page (select "Open Issue" from the drop down options).  Please also open an issue if you have questions or find any content confusing!  Often questions can be answered quickly and highlighting places where the text is unclear will help improve the guide in the future.

## Attribution

### Citation

Please cite this guide as:

Lamarche, L. J. and Kamal, L. (2024).  AMISR User Manual. Retrieved from https://amisr.github.io/amisr_user_manual/intro.html.

### Contributors
The following people have written or contributed to this guide (listed alphabetically).

- Asti Bhatt
- Lara Kamal
- Leslie Lamarche
- Pablo Reyes

### Funding Sources
Contributions to the AMISR User Manual were funded in part by the following sources.

- NSF Cooperative Agreement \#1840962
- NSF Grant \#2027300
- NASA Grant \#80NSSC21K0458

## Table of Contents

```{tableofcontents}
```
