<img src="images/ICCS_logo.png"  width="355" align="left">

<br><br><br><br><br><br><br>

# Introduction to differentiable programming

![GitHub](https://img.shields.io/github/license/Cambridge-ICCS/differentiable-programming-summer-school-2026)

*This course is currently under development for the
[2026 Summer School](https://iccs.cam.ac.uk/events/institute-computing-climate-science-annual-summer-school-2026)
of the
[Institute of Computing for Climate Science (ICCS)](https://iccs.cam.ac.uk) by
[Joe Wallwork](https://joewallwork.com),
[Sam Avis](https://github.com/sjavis), and
[Adeleke Bankole](https://github.com/AdelekeBankole)*

## Setup

*[Work in progress]*

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
