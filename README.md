# Jupyter On Server Guide
_A small simple guide of how to run a jupyter notebook on a server._


### Howto:

0. First time on server: 

    `conda create -n ENV_NAME python=3 jupyter jupyterlab ipykernel [...]` 
    
    `conda activate ENV_NAME` 
    
    `conda ipython kernel install --user --name=KERNEL_NAME` 
    
    Exit server and go back to local machine
 

1. From local machine:

    `ssh -L 8000:localhost:8888 USER@SERVER` 

2. From the server:
    
    `jupyter lab`
    
3. From local machine, in browser:
    
    `http://localhost:8000`
