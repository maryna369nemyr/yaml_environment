# Install miniconda3
You can get an appropriate miniconda version under the url 
(https://docs.conda.io/en/latest/miniconda.html).

If you already have an url of the miniconda's sh file, one can run in the linux terminal:
```
wget 'https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh' -O Miniconda3-latest-Linux-x86_64.sh
```

# Create virtual environment with miniconda3
### Create an environment called "py37"
```
conda create -n py37 python=3.7
```

### Install the necessary packages into the "py37" environment
```
conda install scikit-learn matplotlib jupyter nb_conda -n py37
```

### Activate the environment
```
conda activate py37
```

### Start Jupyter notebook
```
jupyter notebook
```

Note that you can also switch between virtual environments using the Jupyter notebook interface if you have the `nb_conda` package installed.

# Create virtual environment with yaml
The example of how to initialize your environment with yaml file

Once you have a prepared file, please run:
```
conda env create -f path_to/environment.yml
```
It creates a virtual environment in `miniconda3/envs/myenv_yml`.
