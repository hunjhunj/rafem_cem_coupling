# rafem_cem_coupling

Coupling experiment using RAFEM and CEM

# Install Anaconda

If you don't already have Anaconda installed, you'll have to first install
it. If you are using Linux, you can get the installer with:

    $ curl https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh > miniconda.sh

and if you're using Mac,

    $ curl https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh > miniconda.sh

Now run the installer. This will install a minimal version of Anaconda
that contains only a small number of packages. We'll install the rest later.

    $ bash ./miniconda.sh -b -f -p ~/anaconda

Note that the last argument is the location where you want to install
Anaconda. It doesn't really matter where it goes so long as you have
write permission and enough disk space (it will end up being a couple
gigabytes).

Now add the new Anaconda distribution to you path,

    $ export PATH=$HOME/anaconda/bin:$PATH

You may want to also add the above to your .bashrc (or .bash_profile)
file.

# Getting started

Installing `pymt` from the `conda-forge` channel can be achieved by adding
`conda-forge` to your channels with:
 
    $ conda config --add channels conda-forge

Create an empty conda environment to install the software and run
the experiments in.

    $ conda create -n pymt python=3.6
    $ source activate pymt

Install the software needed to run the experiments.

    $ conda install pymt
    $ conda install rafem
    $ conda install pymt_rafemss

# Run the model

Run the model from the command line.

    $ python run_model.pys
