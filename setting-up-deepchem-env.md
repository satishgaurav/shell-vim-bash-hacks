## The installtion didnot work on the macOS, Finally i am using wsl on windows. So it only works on Linux 
DeepChem has many depencdency package. Along with installing others you have to install these packages too. 

#### set up the environment with python=3.6  

#### make sure that you have activated the correct env
`pip install -q mdtraj nglview`
`conda install -c omnia openmm`
`conda install -c omnia pdbfixer`
`conda install -c conda-forge networkx`







# Update 
Initially I had installed python version 3.7 however i think it doesnot support python version greater > 3.7, i have python version python 3.7.10 now i have downgrade the python version. 





## Setting up DeepChem env in MacOS 
I am using M1 Macbook air 

### first download miniconda and install it. [https://docs.conda.io/en/latest/miniconda.html]

#### Create env with specfic python version requirement 
`conda create -n "deepchem" python=3.7`

NOTE: Once you have created a new env in this case `deepchem` do not forget to switch from existing env to the newly created env. After that proceed with new package installation. 

#### Install rdkit 
`conda install -c conda-forge rdkit`

#### Install deepchem 
`conda install -c conda-forge deepchem`

#### Install jupyter lab 
`conda install -c conda-forge jupyterlab` 

#### Install tensorflow and also check version of deepchem you are installing 
`pip install tensorflow~=2.4` 


NOTE: It is recommended that you should first install `tensorflow` and then install `deepchem` library. However, in my case i have done the opposite. I am quite sure that this is going to work or not. 


