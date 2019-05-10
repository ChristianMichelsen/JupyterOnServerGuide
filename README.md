# Jupyter On Server Guide
_A small simple guide of how to run a jupyter notebook on a server._


### Howto:

0. First time on server:
  ```	conda create -n ENV_NAME python=3 numpy matplotlib jupyter jupyterlab ipykernel [...]
	conda activate ENV_NAME
	conda ipython kernel install --user --name=KERNEL_NAME
	conda deactivate```

1. From local machine (second line on server)
	ssh -L 8000:localhost:8888 USER@SERVER
	jupyter lab

2. From local machine, in browser:
	http://localhost:8000



