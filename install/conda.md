# Anaconda, Miniconda, and Miniforge

With respect to the free tools for Data Analysis with Python, [Anaconda Individual Edition](https://www.anaconda.com/products/individual) is the world’s most popular Python distribution platform with over 25 million users worldwide. You have three options:

- [Anaconda Individual](https://www.anaconda.com/products/individual), widely used by novices in Python data science
- [Miniconda](https://docs.conda.io/en/latest/miniconda.html), some experienced data scientists prefer Miniconda to Anaconda
- [Miniforge](https://github.com/conda-forge/miniforge), recommended for data scientists with professional skills in IT

## Anaconda or Miniconda

Here is the excerpt from
[Anaconda or Miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html#anaconda-or-miniconda):

Choose Anaconda if you:
- Are new to conda or Python.
- Like the convenience of having Python and over 1,500 scientific packages automatically installed at once.
- Have the time and disk space---a few minutes and 3 GB.
- Do not want to individually install each of the packages you want to use.
- Wish to use a curated and vetted set of packages.

Choose Miniconda if you:
- Do not mind installing each of the packages you want to use individually.
- Do not have time or disk space to install over 1,500 packages at once.
- Want fast access to Python and the conda commands and you wish to sort out the other programs later.

## Miniforge

The conda team, from Anaconda, Inc., packages a multitude of packages and provides them to all users free of charge in their `default` channel. But what if a package you are looking for is not in the default channel? In the past users only had the option to create an Anaconda Cloud account and create their own channel. This came with a list of disadvantages:

- Locating packages was difficult due to them being scattered over many channels.
- Combining packages across channels was not always possible due to binary incompatibilities.
- Packages were only available for architectures the developer was interested in or had access to.
- Channels were often abandoned, updating required locating new channels.

Miniforge is an effort to provide Miniconda-like installers, with the added feature that [conda-forge](https://conda-forge.org/docs/user/introduction.html) is the default channel. Unlike Miniconda, these support ARMv8 64-bit (formally known as `aarch64`).

- All packages are shared in a single channel named conda-forge.
- Care is taken that all packages are up-to-date.
- Common standards ensure that all packages have compatible versions.
