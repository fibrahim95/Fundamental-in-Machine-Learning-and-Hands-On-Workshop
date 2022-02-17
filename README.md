Hi Everyone!

In this GitHub, we provided the guidelines the installation of Anaconda and Jupyter-Notebook. Please read carefully and do installation before the day workshop start, so we can avoid the technical stuff. Before we proceed to basic python and machine learning examples, we setting up the conda environment with Python and some libraries are needed in this workshop. Hope you enjoy this workshop. 


# Installation-Anaconda
## Tutorial Installation of Anaconda

This repository will aid you to install Anaconda according to your preferrence operating system (OS). Pleaes choose your Anaconda version that compatible with your OS and follow the instructions in the documentation provided to install Anaconda. Here we provided the documentations to download and install Anaconda:
* [Windows](https://docs.anaconda.com/anaconda/install/windows/)
* [Linux](https://docs.anaconda.com/anaconda/install/linux/)
* [Mac Os](https://docs.anaconda.com/anaconda/install/mac-os/)

## Setting Up the Environment of Python 3
Hooorayyy!!!! your are done the installation of Anaconda. Now open the terminal for linux and macOs and activate `base` environment of anaconda by:

![Terminal](https://user-images.githubusercontent.com/70914271/152668997-60d7a8c5-8395-4309-846c-3a2b83af2d6c.png)

```
source ~/anaconda3/bin/activate
```
For windows, search `anaconda prompt` and double click it.
![windows](https://user-images.githubusercontent.com/70914271/152669025-8f8fe0b2-fe62-40c4-b037-7b7b919bc397.jpeg)


Since we are activated conda `base` environment, let's start to create the environment of Anaconda with python version `3.9`. You can read up more on how Conda environments work [here](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html). Basically, they're just a separate place you can mess around without interupting or corrupting your default setup. 

```
conda create -n myEnv python=3.9
```

Here, myEnv is the conda env we designated. To enter the environment it, just type:

```
conda activate myEnv         # to enter the environment

```

The env you just setup is empty, so you need to install the packages that you want to use, even when the default Conda environment has all of them.

```
conda install ipykernel
conda install notebook
```

The Jupyter Notebooks are designed for Python, so you should have no problems. Some libraries may not be available beforehand, so you should download them, such as Matplotlib, pandas, scikit-learn, and etc. If you have already added conda-forge as a channel, the -c conda-forge is unnecessary. Adding the channel is recommended because it ensures that all of your packages use compatible versions. Here is the [conda-forge docs](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge):

```
conda config --add channels conda-forge
conda update --all
```
## Jupyter-Notebook
The Notebooks will give you a brief tutorial into Python, designed for undergrads that have little to no experience in programming. These notebooks are adapated from previous ones made in Python. Just press the Binder link and let it launch. Learn, enjoy, explore!

Running on Binder requires a good internet connection, but even then it does not guarantee that the kernel would not suddenly die. So, to minimize external factors disrupting your experience to learn, it is better for you to run the Jupyter Notebooks locally on your computer. Follow the steps outlined for contributors, then launch the notebooks from the Conda environment.

To open a notebook, and start developing!
```
jupyter-notebook
```

For windows, search `anaconda navigator` and double click it.

```
anaconda-navigator

```
