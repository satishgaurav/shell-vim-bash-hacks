## Setting up DeepChem env in MacOS 
I am using M1 Macbook air 

### first download miniconda and install it. [https://docs.conda.io/en/latest/miniconda.html]

#### Create env with specfic python version requirement 
`conda create -n "deepchem" python=3.7`

#### Install rdkit 
`conda install -c conda-forge rdkit`

#### Install deepchem 
`conda install -c conda-forge deepchem`

#### Install jupyter lab 
`conda install -c conda-forge jupyterlab` 

#### Install tensorflow and also check version of deepchem you are installing 
`pip install tensorflow~=2.4` 


