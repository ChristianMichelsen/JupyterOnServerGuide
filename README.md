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

    `conda activate ENV_NAME`
    
    `jupyter lab`
    
    Save token (e.g. `a721ba7fab1f8485d80986702bb19c11a3f87b0bf1931fde` in the case of http://localhost:8888/?token=a721ba7fab1f8485d80986702bb19c11a3f87b0bf1931fde)
    
3. From local machine, in browser:
    
    `http://localhost:8000`
    
4. Enter token
