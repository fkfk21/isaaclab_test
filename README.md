# isaaclab installation 

https://isaac-sim.github.io/IsaacLab/source/setup/installation/pip_installation.html


環境: ubuntu 22.04, CUDA 12.1

Prerequires
install poetry
```bash
poetry config virtualenvs.in-project true
```


```bash
poetry install --no-root
source (poetry env info --path)/bin/activate.fish # activate virtual environment
vcs import . < isaaclab.repos
isaaclab/isaaaclab.sh --install  # install packages iteratively through pip
```

## memo
### install version
pytorch 2.4.0 for cuda12.1
isaac sim <- followed isaaclab installation

isaaclab/isaaclab.sh install packages directly







