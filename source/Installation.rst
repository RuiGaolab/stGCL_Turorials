.. stGCL documentation master file, created by
   sphinx-quickstart on Thu Sep 16 19:43:51 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Installation
============

The stGCL package is developed based on the pytorch framework and can be implemented on both GPU and CPU. 
We recommend running the package on GPU. Please ensure that pytorch and CUDA are installed correctly. To run stGCL, all dependencies included in the file 'requirements.txt' need to be installed.

Please note that the current stGCL version has been tested on the Linux (Ubuntu 20.04) operating system.

Downloading stGCL code from https://github.com/RuiGaolab/stGCL


Now you can install the current release of stGCL by the following three ways:

1. PyPI: Directly install the package from PyPI
-----------------------------------------------

.. code-block:: python

   pip3 install stGCL
   #Note: you need to make sure that the pip is for python3.

2. Github
---------------------

Download the package from Github and install it locally:

.. code-block:: python

   git clone https://github.com/RuiGaolab/stGCL.git
   
   cd stGCL
   
   python setup.py build

   python setup.py install --user

3. Anaconda
------------
For convenience, we suggest using a separate conda environment for running stGCL. Please ensure annaconda3 is installed.

.. code-block:: python

   #create an environment called stGCL
   conda create -n stGCL python=3.7
   
   #activate your environment
   conda activate stGCL
   
   git clone https://github.com/RuiGaolab/stGCL.git
   
   cd stGCL
   
   python setup.py build

   python setup.py install --user

   conda deactivate
   
