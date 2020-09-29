# TowardsTransaparentAI_vGHC2020
This repository contains content shared in Towards Transparent AI: Understanding Text-Based Model Predictions workshop at Grace Hopper Conference 2020.

# Getting Started
This section shows different ways to get setup for the workshop
Use one of the 3 approaches to get started with the content. The recommened way to get setup is to follow the local setup section.

### Python
For best results please setup this repository on your local machine.

1. Clone this repository to access the sample notebook
```bash
    git clone https://github.com/janhavi13/TowardsTransaparentAI_vGHC2020.git
```
2. Easiest way to run the sample notebook is to create a conda environment

```bash
    conda create -n myenv python=3.6.8
    conda activate myenv
    # Find the appropriate torch for your machine from this link: https://pytorch.org/get-started/locally/
    pip install torch===1.6.0 torchvision===0.7.0 -f https://download.pytorch.org/whl/torch_stable.html # for windows
    pip install datasets
    pip install interpret-text
    pip install jupyter
```
Note: If installing packages in requirements.txt one by one, make sure torch and torchvision is installed before the interpret-text package.

3. Run the jupyter notebook using the command from `TowardsTransaparentAI_vGHC2020` location on your laptop/desktop.
```bash 
    jupyter notebook
```

### Docker
Another way to run the repository content easily is via our pre-built Docker container. 
To do so, run the following command:

```bash
docker run -it -p 8888:8888 janhavim13/interprettext:latest
```

Navigate to <http://localhost:8888/> in your web browser to run the sample
notebooks.

The getting started guide on Docker has detailed instructions for setting up Docker on Mac, Linux and Windows.
See the [documentation](docs/docker.md) for more on Docker use.

### Binder
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/janhavi13/TowardsTransaparentAI_vGHC2020.git/master)
<br>
Click on the binder badge above to run the sample notebook in your browser
