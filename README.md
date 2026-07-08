<img src="./images/UCAM_ICCS_Logo.png"  width="600">

# Introduction to differentiable programming

This repository contains documentation, resources, and code for the
`Introduction to differentiable programming` session designed and delivered by
[Joe Wallwork](https://joewallwork.com), [Sam Avis](https://github.com/sjavis),
and [Adeleke Bankole](https://adelekebankole.github.io/) of
[ICCS](https://github.com/Cambridge-ICCS).
All materials, including slides and videos, are available such that individuals can cover the
course in their own time.

A website for this workshop can be found at
[https://cambridge-iccs.github.io/differentiable-programming-summer-school-2026/](https://cambridge-iccs.github.io/differentiable-programming-summer-school-2026/).

## Contents

- [Learning Objectives](#learning-objectives)
- [Teaching materials](#teaching-materials)
- [Preparation and prerequisites](#preparation-and-prerequisites)
- [Installation and setup](#installation-and-setup)
- [License information](#license)
- [Contribution Guidelines and Support](#contribution-guidelines-and-support)
- [Mini-project](mini-project)


## Learning Objectives

The key learning objective from this workshop is to
_Provide participants with an understanding of the fundamentals of
differentiable programming and experience with using related tools_.

More specifically, in session 1 we will:

* Get a brief history of automatic differentiation.
* Learn about the *operator overloading* approach.
* Learn about *forward mode* and *reverse mode* applied to scalar-valued functions.
* Try out the *Autograd* AD tool applied to some test problems.
* Verify the derivatives produced by Autograd both manually and using the
  *Taylor test*.

In session 2 we will:

* Try out the *JAX* differentiable programming framework.
* Learn about *forward mode* and *reverse mode* applied to functions of several
  variables.
* Experiment with JAX in a machine learning example.


## Teaching Materials

### Notebooks
This course uses [Jupyter notebooks](https://jupyter.org/).
The notebooks for this workshop can be viewed here:

* [Session 1](session1.ipynb)
* [Session 2](session2.ipynb)

### Exercises
The exercises for the course can be found in the notebooks.
These are marked by callout boxes and involve adding or modifying notebook
cells.

### Worked Solutions
Worked solutions for all of the exercises can be found in the notebooks.
These are marked by callout boxes with hidden sections that can be revealed with
a click.


## Preparation and prerequisites

### Prerequisites

To get the most out of the session we assume a basic understanding in a few
areas and for you to do some preparation in advance. This expected knowledge is
outlined below.

* Undergraduate level knowledge of linear algebra and calculus.
* We assume attendees are familiar with the basics of Python. This includes:
    * Basic mathematical operations
    * Writing and using functions
    * Working with Jupyter notebooks
* Basic knowledge of Git
  * See the
    [ICCS Summer School Git course](https://www.youtube.com/watch?v=ZrwzK4CnJ3Q)
    for background.

### Preparation

There are two ways to interact with this course:

1. Using GitHub Codespaces
2. On your local machine

If you are using GitHub codespaces then the only tooling requirement is for you
to have a GitHub account.

If you want to work through the course locally then you will need the following:

* A text editor, e.g. Vim/[NeoVim](https://neovim.io/),
  [gedit](https://gedit.en.softonic.com/),
  [VSCode](https://code.visualstudio.com/),
  [sublimetext](https://www.sublimetext.com/) etc. to open and edit code files.
* A terminal emulator, e.g.
  [GNOME Terminal](https://help.gnome.org/users/gnome-terminal/stable/),
  [wezterm](https://wezfurlong.org/wezterm/index.html),
  [Windows Terminal (windows only)](https://learn.microsoft.com/en-us/windows/terminal/),
  [iTerm (Mac only)](https://iterm2.com/)
* A Python 3 installation
* A GitHub account for cloning the repository

If you require assistance or further information with any of these please reach
out to us before the session.

## Installation and setup

### Accessing Codespaces

If you are using GitHub Codespaces, navigate to the
[course repository](https://github.com/Cambridge-ICCS/differentiable-programming-summer-school-2026)
in a web browser, click the green `Code` button, then the `Codespaces` tab, and
finally `Create a codespace on main`. After a few minutes, this will launch an
interactive VSCode session in your web browser.

### Cloning the repo

If you are working through the tutorial locally, obtain a local copy of the
repository by cloning it from a terminal. Then enter the directory:
```sh
git clone https://github.com/Cambridge-ICCS/differentiable-programming-summer-school-2026.git
cd differentiable-programming-summer-school-2026
```

### Setting up a Python virtual environment

If you are using Codespaces then you can skip this step.

Otherwise, set up a Python virtual environment for the course:
```sh
python3 -m venv dp-venv
source dp-venv/bin/activate
```
With your virtual environment active, your terminal prompt should be preceded by
`(dp-venv)` (or similar, depending on the name you chose).

### Install Python dependencies

With your virtual environment active, install the Python dependencies with
```sh
pip install .
```
from the root directory of the repository. This will install the automatic
differentiation tools [Autograd](https://github.com/HIPS/autograd) and
[JAX](https://jax.dev) and the core Python packages [NumPy](https://numpy.org/),
[Jupyter](https://jupyter.org/), [Matplotlib](https://matplotlib.org/), and
[mpltools](https://tonysyu.github.io/mpltools/).

If this doesn't work for some reason, try the following instead:
```sh
pip install -r requirements.txt
```

### Launch the notebook

If you are using Codespaces then simply find the notebook you want to run
(`session1.ipynb` or `session2.ipynb`) in the file explorer on the
left-hand-side and double-click it.

If you are running locally, you can launch the Jupyter environment from the
command line by running
```sh
jupyter notebook
```
from the root directory of the repository. This will launch a browser tab, in
which you can select the notebook you want to run (`session1.ipynb` or
`session2.ipynb`).

### Developer setup

To install developer dependencies, activate a Python virtual environment and run
```sh
pip install .[dev]
```
This will install `pre-commit`, amongst other packages. Run
```sh
pre-commit install
```
to set up Git pre-commit hooks. Notably, the `stripout.sh` script will be added
so that the cells in the Jupyter notebooks get cleared out before commits go
through.


## License

The code materials in this project are licensed under the
[MIT License](LICENSE).

Images in the [`images`](./images) subdirectory are separately licensed under a
[Creative Commons License](https://creativecommons.org/share-your-work/cclicenses/).


## Contribution Guidelines and Support

If you spot an issue with the materials please let us know by
[opening an
issue](https://github.com/Cambridge-ICCS/differentiable-programming-summer-school-2026/issues)
here on GitHub clearly describing the problem.

If you are able to fix an issue that you spot, or an
[existing open issue](https://github.com/Cambridge-ICCS/differentiable-programming-summer-school-2026/issues)
please get in touch by commenting on the issue thread.

Contributions from the community are welcome.
To contribute back to the repository please first
[fork
it](https://github.com/Cambridge-ICCS/differentiable-programming-summer-school-2026/fork),
make the necessary changes to fix the problem, and then open a pull request back to
this repository clearly describing the changes you have made.
We will then preform a review and merge once ready.

If you would like support using these materials, adapting them to your needs, or
delivering them please get in touch either via GitHub or via
[ICCS](https://github.com/Cambridge-ICCS).


## Mini-project

This year's summer school includes a session on Thursday afternoon in which
attendees will form groups to work on one of several predefined mini-projects.
This course has a mini-project associated with it, which is outlined in the
[miniproject](miniproject) subdirectory. Code associated with the mini-project
is provided in that subdirectory.
